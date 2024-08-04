Certainly! Below is a practical CMD batch file that performs all the tasks you've mentioned. This batch file takes various inputs as parameters and executes the necessary commands for each step.

```batch
@echo off
setlocal

REM Check if the correct number of parameters are passed
if "%~1"=="" (
    echo Usage: %0 SolutionName WpfProjectName ConsoleProjectName Version
    exit /b 1
)

REM Parameters
set SOLUTION_NAME=%~1
set WPF_PROJECT_NAME=%~2
set CONSOLE_PROJECT_NAME=%~3
set VERSION=%~4

REM 1. Create a .NET Solution
dotnet new sln -n %SOLUTION_NAME%
cd %SOLUTION_NAME%

REM 2. Add a WPF Project to the Solution
dotnet new wpf -n %WPF_PROJECT_NAME%
dotnet sln add %WPF_PROJECT_NAME%\%WPF_PROJECT_NAME%.csproj

REM 3. Add a Console Project to the Solution
dotnet new console -n %CONSOLE_PROJECT_NAME%
dotnet sln add %CONSOLE_PROJECT_NAME%\%CONSOLE_PROJECT_NAME%.csproj

REM 4. Add a NuGet Package (CSV Helper)
dotnet add %WPF_PROJECT_NAME%\%WPF_PROJECT_NAME%.csproj package CsvHelper
dotnet add %CONSOLE_PROJECT_NAME%\%CONSOLE_PROJECT_NAME%.csproj package CsvHelper

REM 5. Clean the Solution
dotnet clean %SOLUTION_NAME%.sln

REM 6. Restore the NuGet Packages
dotnet restore %SOLUTION_NAME%.sln

REM 7. Build the Solution
dotnet build %SOLUTION_NAME%.sln

REM 8. Clear the NuGet Cache and Restore Again
dotnet nuget locals all --clear
dotnet restore %SOLUTION_NAME%.sln

REM 9. Rebuild the Solution as x86 and x64
dotnet build %SOLUTION_NAME%.sln -r win-x86
dotnet build %SOLUTION_NAME%.sln -r win-x64

REM 10. Logging the Build Process
dotnet build %SOLUTION_NAME%.sln > build.log

REM 11. Zip for Distribution
set ZIP_NAME=%SOLUTION_NAME%_%DATE:~10,4%%DATE:~4,2%%DATE:~7,2%_%TIME:~0,2%%TIME:~3,2%%TIME:~6,2%_v%VERSION%.tar.gz
tar -cvzf %ZIP_NAME% %SOLUTION_NAME%\bin\Release

REM 12. Create a Self-Signed Certificate
dotnet dev-certs https -ep ./MyCert.pfx -p password

REM 13. Link Self-Signed Certificate with Projects
for %%i in (%WPF_PROJECT_NAME% %CONSOLE_PROJECT_NAME%) do (
    echo ^<ItemGroup^> >> %%i\%%i.csproj
    echo ^<None Update="MyCert.pfx"^> >> %%i\%%i.csproj
    echo ^<CopyToOutputDirectory^>PreserveNewest^</CopyToOutputDirectory^> >> %%i\%%i.csproj
    echo ^</None^> >> %%i\%%i.csproj
    echo ^</ItemGroup^> >> %%i\%%i.csproj
)

REM 14. Generate XML Documentation for Swagger
for %%i in (%WPF_PROJECT_NAME% %CONSOLE_PROJECT_NAME%) do (
    echo ^<PropertyGroup^> >> %%i\%%i.csproj
    echo ^<GenerateDocumentationFile^>true^</GenerateDocumentationFile^> >> %%i\%%i.csproj
    echo ^</PropertyGroup^> >> %%i\%%i.csproj
)

dotnet build %SOLUTION_NAME%.sln

endlocal
echo Done.
pause
```

**Usage:**
```
MyBatchFile.bat MySolution MyWpfApp MyConsoleApp 1.0.0
```

This batch file does the following:
1. Creates a new .NET solution.
2. Adds a WPF project to the solution.
3. Adds a console project to the solution.
4. Adds the CSV Helper NuGet package to both projects.
5. Cleans the solution.
6. Restores the NuGet packages.
7. Builds the solution.
8. Clears the NuGet cache and restores the packages again.
9. Rebuilds the solution targeting both x86 and x64.
10. Logs the build process.
11. Zips the build output for distribution.
12. Creates a self-signed certificate.
13. Links the self-signed certificate with both projects.
14. Configures the projects to generate XML documentation for Swagger.
