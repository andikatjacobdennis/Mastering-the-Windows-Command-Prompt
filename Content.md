# Mastering the Windows Command Prompt

## Section 1: Getting Started with Command Prompt

### 1. Opening the Command Prompt
- **Example 1:** Use the Run dialog (Win + R) and type `cmd` to open Command Prompt.
- **Example 2:** Search for "Command Prompt" in the Start Menu and select it to open.

### 2. Running as an Administrator
- **Example 1:** Right-click on "Command Prompt" in the Start Menu and select "Run as administrator."
- **Example 2:** Use the Run dialog (Win + R), type `cmd`, and press Ctrl + Shift + Enter.

### 3. `whoami`: Determining the Logged-in User
- **Example 1:** Open Command Prompt and type `whoami` to see the current user.
- **Example 2:** Use `whoami /user` to get detailed information about the user.

### 4. `cd`: Changing Directories and Navigating the File System
- **Example 1:** Navigate to the root directory with `cd \`.
- **Example 2:** Move to a specific directory, e.g., `cd C:\Users\YourUsername\Documents`.

### 5. How to Read Command Prompt
- **Example 1:** Understand the prompt structure (e.g., `C:\Users\YourUsername>`).
- **Example 2:** Learn to interpret common error messages, like "Access is denied."

### 6. Using the Up and Down Arrow Keys for Navigating
- **Example 1:** Use the Up arrow to recall the last command.
- **Example 2:** Use the Down arrow to navigate through the command history.

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

## Conclusion
Mastering these advanced Command Prompt commands and batch file programming techniques will significantly enhance your productivity and ability to automate tasks in Windows. Experiment with these commands and incorporate them into your workflow to harness their full potential.
