# Mastering the Windows Command Prompt

Mastering these advanced Command Prompt commands and batch file programming techniques will significantly enhance your productivity and ability to automate tasks in Windows. Experiment with these commands and incorporate them into your workflow to harness their full potential.

> **Note:** Use the command prompt with caution, as some commands can recursively delete files and folders or cause irreparable damage to your PC.

## Section 1: Getting Started with Command Prompt

### 1. Understanding and Interpreting Command Prompt

**Prompt Structure**:

- **Structure**: `C:\Users\YourUsername>`
  - **Drive Letter (C:)**: Current drive.
  - **Path (`\Users\YourUsername`)**: Current directory.
  - **Prompt Symbol (`>`)**: Indicates readiness for input.

**Using It**:

1. **Navigating Directories**: Use `cd` (Change Directory).
   ```shell
   cd Documents
   ```
2. **Listing Files**: Use `dir` to list files and directories.
   ```shell
   dir
   ```
3. **Executing Programs**: Run executable files or scripts.
   ```shell
   example.exe
   ```

**Interpreting Common Error Messages**:

- **"Access is denied"**:
  - **Meaning**: Insufficient permissions.
  - **Troubleshoot**:
    1. **Check Permissions**: Run as administrator.
    2. **Verify Path**: Ensure correct path and existence of file/directory.
    3. **Modify Permissions**: Use `icacls` to grant permissions.
      ```shell
      icacls "path\to\file" /grant YourUsername:(F)
      ```

### 2. Opening the Command Prompt

- **Example 1**: Use Run dialog (Win + R) and type `cmd`.
- **Example 2**: Search "Command Prompt" in Start Menu and select it.

### 3. Running as an Administrator

- **Example 1**: Right-click on "Command Prompt" in Start Menu and select "Run as administrator."
- **Example 2**: Use Run dialog (Win + R), type `cmd`, and press Ctrl + Shift + Enter.

### 4. `whoami`: Determining the Logged-in User

- **Example 1**: Type `whoami` in Command Prompt.
- **Example 2**: Use `whoami /user` for detailed information.

### 5. `cd`: Changing Directories and Navigating the File System

- **Example 1**: Navigate to root directory with `cd \`.
- **Example 2**: Move to a specific directory, e.g., `cd C:\Users\YourUsername\Documents`.

### 6. Using the Up and Down Arrow Keys for Navigating

- **Example 1**: Use Up arrow to recall last command.
- **Example 2**: Use Down arrow to navigate through command history.

### 7. Changing a Drive in Command Prompt

- **Example**: Switch from C: to D:
  ```shell
  D:
  ```

### 8. Tab Completion

**How to Use**:

- **Auto-Completing File and Directory Names**:
  1. **Start with Partial Name**: Type initial characters.
     ```shell
     cd Doc
     ```
  2. **Press Tab**: Auto-complete name.
     ```shell
     cd Documents
     ```
  3. **Cycle Through Matches**: Press Tab repeatedly.

- **Configuring Tab Completion Behavior**:
  - Enable via registry: `CompletionChar` and `PathCompletionChar`.

### 9. Wildcards

1. **Asterisk (*)**: Matches any number of characters.
   - Example: `*.txt` matches all `.txt` files.
2. **Question Mark (?)**: Matches a single character.
   - Example: `file?.txt` matches `file1.txt`, `fileA.txt`, but not `file10.txt`.

- **Additional Tips**:
  - **Escaping Wildcards**: Use caret (`^`) to escape.
    ```shell
    echo file^*.txt
    ```
## Section 2: Basic Command Prompt Operations

### 1. `mkdir`: Creating Directories
- **Example 1:** Create a single directory: `mkdir NewFolder`.
- **Example 2:** Create nested directories: `mkdir ParentFolder\ChildFolder`.

### 2. `cls`: Clearing the Screen
- **Example 1:** Type `cls` to clear the current Command Prompt screen.
- **Example 2:** Create a batch file to clear the screen: `echo cls > clear.bat`.

### 3. `echo`: Displaying Messages and Output
- **Example 1:** Display a simple message: `echo Hello, World!`.
- **Example 2:** Write output to a file: `echo This is a test > testfile.txt`.

### 4. `copy`: Copying Files
- **Example 1:** Copy a file to another location: `copy file.txt C:\NewFolder`.
- **Example 2:** Copy multiple files using wildcards: `copy *.txt C:\NewFolder`.

### 5. `move`: Moving Files
- **Example 1:** Move a file to a new location: `move file.txt C:\NewFolder`.
- **Example 2:** Move all files of a specific type: `move *.txt C:\NewFolder`.

### 6. `rename`: Renaming Files
- **Example 1:** Rename a single file: `rename oldfile.txt newfile.txt`.
- **Example 2:** Rename multiple files with a pattern: `rename *.txt *.bak`.

### 7. Command Prompt Basics: Navigating and Essential Commands Quiz
   - **Question 1:** How do you create a new directory?
   - **Question 2:** What command clears the Command Prompt screen?
   - **Question 3:** How do you display a message in Command Prompt?

## Section 3: Advanced Directory Navigation and File Management

### 1. `dir`: Listing Contents of a Directory
- **Example 1:** List all files and directories: `dir`.
- **Example 2:** List hidden files and directories: `dir /a`.

### 2. Reading `dir` Outputs
- **Example 1:** Interpret file attributes and sizes.
- **Example 2:** Use `dir /s` to list directory contents recursively.

### 3. Creating and Editing Files
- **Example 1:** Create a file using `echo`: `echo Hello > hello.txt`.
- **Example 2:** Edit a file with `notepad`: `notepad hello.txt`.

### 4. `rmdir`: Removing Directories
- **Example 1:** Remove an empty directory: `rmdir EmptyFolder`.
- **Example 2:** Remove a directory and its contents: `rmdir /s /q FolderToRemove`.

### 5. `help`: Accessing Built-in Documentation
- **Example 1:** View help for a specific command: `help copy`.
- **Example 2:** Get detailed command syntax: `copy /?`.

### 6. `%username%`: Understanding Environmental Variables
- **Example 1:** Display the current username: `echo %username%`.
- **Example 2:** Use environmental variables in paths: `cd C:\Users\%username%\Documents`.

### 7. `explorer`: Opening Directories and Files with Windows Explorer
- **Example 1:** Open a directory: `explorer C:\NewFolder`.
- **Example 2:** Open a specific file: `explorer C:\NewFolder\file.txt`.

### 8. Section 3 Assessment: Advanced Directory Navigation and Command Functions
   - **Question 1:** How do you list all files, including hidden ones?
   - **Question 2:** What command removes a directory and its contents?
   - **Question 3:** How do you view help for the `copy` command?
   - **Question 4:** How do you open a directory with Windows Explorer?

## Section 4: Command Prompt Navigation Tips and Tricks

### 1. Navigating Command History Using the Up and Down Arrows
- **Example 1:** Use the Up arrow to recall previous commands.
- **Example 2:** Use the Down arrow to navigate through the command history.

### 2. Copying and Pasting Within the CMD
- **Example 1:** Enable QuickEdit Mode for easier copy-pasting.
- **Example 2:** Use Ctrl + C to copy and Ctrl + V to paste.

### 3. `doskey`: Creating Command Aliases
- **Example 1:** Create an alias for a command: `doskey ll=dir`.
- **Example 2:** Create a macro with parameters: `doskey gdrive=cd /d D:\GoogleDrive\ $*`.

## Section 5: Network Commands and Utilities

### 1. `netsh wlan show profile`: Viewing Wireless Profiles
- **Example 1:** List all wireless profiles: `netsh wlan show profiles`.
- **Example 2:** View details of a specific profile: `netsh wlan show profile name="ProfileName"`.

### 2. `netsh`: Revealing Saved Network Passwords
Ensure the Folder Exists: The folder specified in the command must already exist. Create the folder C:\WiFiProfiles if it doesn’t exist before running the command.
- **Example 1:** Display the password of a saved network: `netsh wlan show profile name="ProfileName" key=clear`.
- **Example 2:** Export wireless profiles: `netsh wlan export profile folder=C:\WiFiProfiles`.

### 3. `ipconfig`: Viewing and Managing IP Configurations
- **Example 1:** Display IP configuration: `ipconfig`.
- **Example 2:** Release and renew IP addresses: `ipconfig /release` and `ipconfig /renew`.

### 4. `ipconfig/all`: Listing All Configurations
- **Example 1:** View detailed IP configuration: `ipconfig /all`.
- **Example 2:** Save the output to a file: `ipconfig /all > ipconfig.txt`.

### 5. `ping`: Testing Network Connectivity
- **Example 1:** Ping a website: `ping google.com`.
- **Example 2:** Ping with a specific number of requests: `ping google.com -n 10`.

### 6. `tracert`: Tracing the Route of Packets to a Destination
- **Example 1:** Trace the route to a website: `tracert google.com`.
- **Example 2:** Save the route information to a file: `tracert google.com > tracert.txt`.

### 7. `tasklist`: Viewing Currently Running Tasks and Processes
- **Example 1:** List all running tasks: `tasklist`.
- **Example 2:** List tasks with specific attributes: `tasklist /fi "STATUS eq running"`.
- **Example 3:** To kill all Chrome processes in the Task List using Command Prompt, you can use the `taskkill` command. Here's the command to do it:

```cmd
taskkill /F /IM chrome.exe /T
```

Explanation:
- `/F` forces the termination of the processes.
- `/IM` specifies the image name (in this case, `chrome.exe`).
- `/T` terminates the specified process and any child processes started by it.

Running this command will close all Chrome instances and any related processes. Make sure to save any work in Chrome before executing this command as it will forcefully close the browser without saving open tabs.

### 8. `netstat`: Displaying Active Network Connections
- **Example 1:** View all active connections: `netstat`.
- **Example 2:** Display network statistics: `netstat -e`.

### 9. `nslookup`: Querying Domain Name Servers to Obtain Domain Names
- **Example 1:** Find the IP address of a domain: `nslookup google.com`.
- **Example 2:** Query a specific DNS server: `nslookup google.com 8.8.8.8`.

### 10. Command Prompt Essentials: Section 5 Quiz
   - **Question 1:** How do you view wireless profiles?
   - **Question 2:** What command reveals saved network passwords?
   - **Question 3:** How do you list all IP configurations?
   - **Question 4:** What command tests network connectivity?

## Section 6: Disk and File System Management

### 1. `diskpart`: Managing Partitions on a Hard Drive
- **Example 1:** List all disks: `diskpart` followed by `list disk`.
- **Example 2:** Create a new partition: `diskpart` followed by `create partition primary`.

### 2. `robocopy`: A Robust File Copying Tool, Especially for Network Operations
- **Example 1:** Copy files with attributes: `robocopy C:\Source C
:\Destination /COPY:DAT`.
- **Example 2:** Mirror directories: `robocopy C:\Source C:\Destination /MIR`.

### 3. `fsutil`: A Versatile Tool for Performing Many NTFS and FAT File System Tasks
- **Example 1:** Check drive type: `fsutil fsinfo drivetype C:`.
- **Example 2:** Create a hard link: `fsutil hardlink create newfile.txt existingfile.txt`.

### 4. `fsutil`: Special Focus on How to Check Drive Types
- **Example 1:** Verify if a drive is a fixed drive: `fsutil fsinfo drivetype C:`.
- **Example 2:** Check if a drive is removable: `fsutil fsinfo drivetype D:`.

### 5. `convert`: Converting a Volume's File System
- **Example 1:** Convert FAT32 to NTFS: `convert C: /FS:NTFS`.
- **Example 2:** Convert a volume with parameters: `convert E: /FS:NTFS /V`.

### 6. `format`: Formatting a Disk for Use
- **Example 1:** Quick format a drive: `format E: /Q /FS:NTFS`.
- **Example 2:** Format with a specific allocation unit size: `format F: /A:4096`.

### 7. `sfc`: Scanning and Fixing System Files
- **Example 1:** Scan and repair system files: `sfc /scannow`.
- **Example 2:** Verify only (without repairing): `sfc /verifyonly`.

### 8. `defrag`: Defragmenting and Optimizing Drives
- **Example 1:** Defragment a drive: `defrag C: /O`.
- **Example 2:** Analyze a drive before defragmenting: `defrag D: /A`.

## Section 7: Advanced Text and Network Commands

### 1. `findstr`: Advanced Text Searching with Support for Regular Expressions
- **Example 1:** Search for a specific string in files: `findstr "search text" *.txt`.
- **Example 2:** Use regular expressions: `findstr /R "regex_pattern" file.txt`.

### 2. `net view`: Displaying a List of Computers and Resources Shared on the Network
- **Example 1:** List all computers on the network: `net view`.
- **Example 2:** View shared resources of a specific computer: `net view \\ComputerName`.

### 3. `fc`: Comparing Two Files or Sets of Files and Displaying Differences
- **Example 1:** Compare two text files: `fc file1.txt file2.txt`.
- **Example 2:** Compare binary files: `fc /b file1.exe file2.exe`.

### 4. `restrui`: Launching the System Restore Utility
- **Example 1:** Open System Restore interface: `restrui`.
- **Example 2:** Start System Restore with a specific restore point: `restrui /offline:C:\windows=active`.

### 5. `shutdown`: Shutting Down or Restarting a Computer with Various Options
- **Example 1:** Shutdown the computer: `shutdown /s /f /t 0`.
- **Example 2:** Restart the computer: `shutdown /r /f /t 0`.

### 6. `pathping`: Combining the Functionalities of Ping and Tracert
- **Example 1:** Perform a pathping to a website: `pathping google.com`.
- **Example 2:** Save pathping results to a file: `pathping google.com > pathping.txt`.

### 7. `driverquery`: Listing All Installed Device Drivers and Their Properties
- **Example 1:** List all drivers: `driverquery`.
- **Example 2:** Export driver list to a CSV file: `driverquery /fo csv /v > drivers.csv`.

### 8. `wevtutil`: Querying and Managing Event Logs
- **Example 1:** List all event logs: `wevtutil el`.
- **Example 2:** Export a specific event log: `wevtutil epl System systemlog.evtx`.

### 9. `cipher`: Encrypting or Decrypting Files and Folders on NTFS Volumes
- **Example 1:** Encrypt a folder: `cipher /e /s:C:\EncryptedFolder`.
- **Example 2:** Decrypt a file: `cipher /d C:\EncryptedFolder\file.txt`.

### 10. `lodctr`: Updating Registry Values Associated with Windows Performance Counters
- **Example 1:** Update performance counters: `lodctr /R`.
- **Example 2:** Backup performance counter settings: `lodctr /S:backup.ini`.

### 11. `wbadmin`: Command-line Backup Utility, Focusing on the Backup Command
- **Example 1:** Create a backup of the C: drive: `wbadmin start backup -backupTarget:D: -include:C: -quiet`.
- **Example 2:** List details of backups: `wbadmin get versions`.

### 12. `runas`: Executing a Tool with Different User Credentials
- **Example 1:** Run a program as another user: `runas /user:domain\username "program.exe"`.
- **Example 2:** Run a program with elevated privileges: `runas /noprofile /user:Administrator cmd`.

## Section 8: Batch File Programming

### 1. How to Set Name in Batch Files
- **Example 1:** Set and display a variable: `set name=John & echo %name%`.
- **Example 2:** Use variables in a script: 
  ```batch
  @echo off
  set name=John
  echo Hello, %name%
  ```

### 2. Creating Batch Files
- **Example 1:** Create a simple batch file: `echo echo Hello > hello.bat`.
- **Example 2:** Create a batch file to automate tasks: 
  ```batch
  @echo off
  mkdir NewFolder
  cd NewFolder
  echo This is a test file > testfile.txt
  ```

### 3. Writing Batch Files
- **Example 1:** Write a batch file with multiple commands: 
  ```batch
  @echo off
  echo Starting process...
  mkdir Backup
  xcopy C:\Data\* C:\Backup\
  echo Process completed.
  ```
- **Example 2:** Create a batch file with conditional statements: 
  ```batch
  @echo off
  if exist "C:\Backup\*.*" (
    echo Backup already exists.
  ) else (
    mkdir Backup
    xcopy C:\Data\* C:\Backup\
    echo Backup created.
  )
  ```

### 4. User Input
- **Example 1:** Prompt for user input: 
  ```batch
  @echo off
  set /p name=Enter your name: 
  echo Hello, %name%.
  ```
- **Example 2:** Use input in a conditional statement: 
  ```batch
  @echo off
  set /p answer=Do you want to continue? (y/n): 
  if %answer%==y (
    echo Continuing...
  ) else (
    echo Exiting...
    exit
  )
  ```

### 5. If-Else Statements
- **Example 1:** Basic if-else statement: 
  ```batch
  @echo off
  set /p number=Enter a number: 
  if %number% gtr 10 (
    echo The number is greater than 10.
  ) else (
    echo The number is 10 or less.
  )
  ```
- **Example 2:** Nested if-else statements: 
  ```batch
  @echo off
  set /p age=Enter your age: 
  if %age% lss 13 (
    echo You are a child.
  ) else if %age% lss 20 (
    echo You are a teenager.
  ) else (
    echo You are an adult.
  )
  ```

### 6. For Loops
- **Example 1:** Loop through a set of numbers: 
  ```batch
  @echo off
  for /l %%i in (1,1,5) do (
    echo Number %%i
  )
  ```
- **Example 2:** Loop through files in a directory: 
  ```batch
  @echo off
  for %%f in (*.txt) do (
    echo File: %%f
  )
  ```

### 7. While Loops
- **Example 1:** Simulate a while loop: 
  ```batch
  @echo off
  set /a count=0
  :loop
  if %count% lss 5 (
    echo Count: %count%
    set /a count+=1
    goto loop
  )
  ```
- **Example 2:** Use a while loop with user input: 
  ```batch
  @echo off
  set /a count=0
  :loop
  set /p answer=Do you want to continue? (y/n): 
  if %answer%==y (
    set /a count+=1
    echo Count: %count%
    goto loop
  )
  echo Exiting...
  ```

### 8. Functions
- **Example 1:** Define and call a function: 
  ```batch
  @echo off
  call :greet
  exit /b

  :greet
  echo Hello, World!
  exit /b
  ```


- **Example 2:** Function with parameters: 
  ```batch
  @echo off
  call :add 5 10
  exit /b

  :add
  set /a sum=%1 + %2
  echo Sum: %sum%
  exit /b
  ```

## Section 8: Batch with C#

### 1. Create a .NET Solution
**Steps to create a new .NET solution using the Command Prompt:**
- Open Command Prompt.
- Navigate to the desired directory.
- Run the following command:
  ```bash
  dotnet new sln -n MySolution
  ```
  This creates a new solution named `MySolution`.

### 2. Add a WPF Project to the Solution
**Instructions on how to add a WPF project to the existing solution:**
- Navigate to the solution directory:
  ```bash
  cd MySolution
  ```
- Add a new WPF project:
  ```bash
  dotnet new wpf -n MyWpfApp
  ```
- Add the WPF project to the solution:
  ```bash
  dotnet sln add MyWpfApp/MyWpfApp.csproj
  ```

### 3. Add a Console Project to the Solution
**Process for adding a console project to the solution:**
- Add a new console project:
  ```bash
  dotnet new console -n MyConsoleApp
  ```
- Add the console project to the solution:
  ```bash
  dotnet sln add MyConsoleApp/MyConsoleApp.csproj
  ```

### 4. Add a NuGet Package (CSV Helper)
**How to add the CSV Helper NuGet package to both the WPF and console projects:**
- Add CSV Helper to the WPF project:
  ```bash
  dotnet add MyWpfApp/MyWpfApp.csproj package CsvHelper
  ```
- Add CSV Helper to the console project:
  ```bash
  dotnet add MyConsoleApp/MyConsoleApp.csproj package CsvHelper
  ```

### 5. Clean the Solution
**Steps to clean the solution using Command Prompt:**
- Run the following command to clean the solution:
  ```bash
  dotnet clean MySolution.sln
  ```
- **Importance:** Cleaning the solution helps remove any build artifacts and ensures a fresh build environment.

### 6. Restore the NuGet Packages
**How to restore the NuGet packages for the projects:**
- Run the following command to restore packages:
  ```bash
  dotnet restore MySolution.sln
  ```

### 7. Build the Solution
**Steps to build the solution using Command Prompt:**
- Run the following command to build the solution:
  ```bash
  dotnet build MySolution.sln
  ```

### 8. Clear the NuGet Cache and Restore Again
**Instructions on how to clear the NuGet cache:**
- Clear the NuGet cache:
  ```bash
  dotnet nuget locals all --clear
  ```
- Restore the packages again:
  ```bash
  dotnet restore MySolution.sln
  ```

### 9. Rebuild the Solution as x86 or x64
**Process for rebuilding the solution targeting x86 or x64:**
- For x86:
  ```bash
  dotnet build MySolution.sln -r win-x86
  ```
- For x64:
  ```bash
  dotnet build MySolution.sln -r win-x64
  ```

### 10. Logging the Build Process
**Methods to log the build process output:**
- Use the following command to log the build process:
  ```bash
  dotnet build MySolution.sln > build.log
  ```
  This logs the build output to `build.log`.

### 11. Zip for Distribution
**Steps to zip the built solution for distribution:**
- Use the following command to zip the output, including date, time, and version:
  ```bash
  tar -cvzf MySolution_$(date +%Y%m%d_%H%M%S)_v1.0.0.tar.gz MySolution/bin/Release
  ```
  Specify the output path as needed.

### 12. Create a Self-Signed Certificate
**Instructions to create a self-signed certificate:**
- Run the following command:
  ```bash
  dotnet dev-certs https -ep ./MyCert.pfx -p password
  ```

### 13. Link Self-Signed Certificate with Projects
**Steps to link the self-signed certificate with the WPF and console projects:**
- Update the project files (`.csproj`) to include the certificate:
  ```xml
  <ItemGroup>
    <None Update="MyCert.pfx">
      <CopyToOutputDirectory>PreserveNewest</CopyToOutputDirectory>
    </None>
  </ItemGroup>
  ```
- Configure the projects to use the certificate.

### 14. Generate XML Documentation for Swagger
**Instructions to generate XML documentation for Swagger:**
- Update the project files (`.csproj`) to generate XML documentation:
  ```xml
  <PropertyGroup>
    <GenerateDocumentationFile>true</GenerateDocumentationFile>
  </PropertyGroup>
  ```
- Build the project to generate the XML documentation.

Here's a section on "CMD Secret Tricks" for your course on mastering the Windows Command Prompt. This section will cover some advanced and lesser-known CMD tricks with practical examples:

## Section 9: CMD Secret Tricks

The Windows Command Prompt (CMD) is packed with hidden gems and secret tricks that can significantly enhance your productivity. This section explores some of these advanced features, providing practical examples to help you leverage CMD to its fullest.

### 1. **Command History Navigation**

CMD keeps a history of commands you’ve entered, and you can easily navigate through this history.

- **Up/Down Arrow Keys**: Press the `Up` and `Down` arrow keys to cycle through previously entered commands.
- **F7 Key**: Press `F7` to display a graphical history menu of commands.

**Example:**

```plaintext
C:\>dir
C:\>cd Documents
C:\>dir
C:\>F7
```

### 2. **Redirecting Output to Clipboard**

You can quickly copy the output of a command to the clipboard using the `clip` command.

**Example:**

```cmd
C:\>dir | clip
```

This command copies the directory listing to the clipboard. You can paste it into a document or an email.

### 3. **Using Command Aliases**

CMD allows you to create aliases for long commands using `doskey`.

**Example:**

```cmd
C:\>doskey ll=dir /w /p
```

Now, typing `ll` will execute `dir /w /p`, which lists the directory in wide format with pagination.

### 4. **Running Multiple Commands**

You can execute multiple commands in a single line using `&&` (execute next command only if the previous succeeds) or `||` (execute next command only if the previous fails).

**Example:**

```cmd
C:\>mkdir TestFolder && cd TestFolder && echo Hello > hello.txt
```

This creates a folder, navigates into it, and creates a file with content in one line.

### 5. **Command Substitution**

You can use the `for` loop to execute a command and use its output in another command.

**Example:**

```cmd
C:\>for /f "tokens=*" %i in ('date /t') do echo Today is %i
```

This command captures the output of `date /t` and uses it to print "Today is" followed by the current date.

### 6. **Running CMD as Administrator Automatically**

Create a shortcut to CMD that always runs as an administrator:

1. Right-click on the desktop and select "New > Shortcut."
2. Enter `cmd.exe` and click "Next."
3. Name the shortcut and click "Finish."
4. Right-click the new shortcut, select "Properties."
5. Click on "Advanced" and check "Run as administrator."

### 7. **Using `tasklist` and `taskkill`**

You can list and terminate processes directly from CMD.

**Example:**

```cmd
C:\>tasklist
C:\>taskkill /im notepad.exe /f
```

The first command lists all running processes, and the second command forcefully terminates Notepad.

### 8. **Finding Files with `where`**

The `where` command helps locate files in your directories.

**Example:**

```cmd
C:\>where python
```

This command finds the path of the `python` executable.

### 9. **Scheduling Tasks**

Use `schtasks` to schedule tasks to run at specific times.

**Example:**

```cmd
C:\>schtasks /create /tn "Backup" /tr "C:\Backup.bat" /sc daily /st 14:00
```

This schedules a task named "Backup" to run `C:\Backup.bat` daily at 2 PM.

### 10. **Redirecting Output to Multiple Files**

You can redirect output to multiple files using `tee`.

**Example:**

```cmd
C:\>dir | tee file1.txt | tee file2.txt
```

This command writes the output of `dir` to both `file1.txt` and `file2.txt`.

### 11. **Using Environment Variables**

Environment variables can be set and used within CMD.

**Example:**

```cmd
C:\>set MYVAR=HelloWorld
C:\>echo %MYVAR%
HelloWorld
```

This sets a variable `MYVAR` and then prints its value.

### 12. **Creating a Batch Script for Common Tasks**

You can automate repetitive tasks by writing batch scripts.

**Example:**

Create a file named `cleanup.bat` with the following content:

```cmd
@echo off
del /q "C:\Temp\*"
echo Temporary files deleted.
```

Running `cleanup.bat` will delete all files in the `C:\Temp\` folder and display a confirmation message.

