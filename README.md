- [Mastering the Windows Command Prompt](#mastering-the-windows-command-prompt)
   * [Section 1: Getting Started with Command Prompt](#section-1-getting-started-with-command-prompt)
      + [1. Understanding and Interpreting Command Prompt](#1-understanding-and-interpreting-command-prompt)
      + [2. Opening the Command Prompt](#2-opening-the-command-prompt)
      + [3. Running as an Administrator](#3-running-as-an-administrator)
      + [4. `whoami`: Determining the Logged-in User](#4-whoami-determining-the-logged-in-user)
      + [5. `cd`: Changing Directories and Navigating the File System](#5-cd-changing-directories-and-navigating-the-file-system)
      + [6. Using the Up and Down Arrow Keys for Navigating](#6-using-the-up-and-down-arrow-keys-for-navigating)
      + [7. Changing a Drive in Command Prompt](#7-changing-a-drive-in-command-prompt)
      + [8. Tab Completion](#8-tab-completion)
      + [9. Wildcards](#9-wildcards)
   * [Section 2: Basic Command Prompt Operations](#section-2-basic-command-prompt-operations)
      + [1. `mkdir`: Creating Directories](#1-mkdir-creating-directories)
      + [2. `cls`: Clearing the Screen](#2-cls-clearing-the-screen)
      + [3. `echo`: Displaying Messages and Output](#3-echo-displaying-messages-and-output)
      + [4. `copy`: Copying Files](#4-copy-copying-files)
      + [5. `move`: Moving Files](#5-move-moving-files)
      + [6. `rename`: Renaming Files](#6-rename-renaming-files)
      + [7. Command Prompt Basics: Navigating and Essential Commands Quiz](#7-command-prompt-basics-navigating-and-essential-commands-quiz)
   * [Section 3: Advanced Directory Navigation and File Management](#section-3-advanced-directory-navigation-and-file-management)
      + [1. `dir`: Listing Contents of a Directory](#1-dir-listing-contents-of-a-directory)
      + [2. Reading `dir` Outputs](#2-reading-dir-outputs)
      + [3. Creating and Editing Files](#3-creating-and-editing-files)
      + [4. `rmdir`: Removing Directories](#4-rmdir-removing-directories)
      + [5. `help`: Accessing Built-in Documentation](#5-help-accessing-built-in-documentation)
      + [6. `%username%`: Understanding Environmental Variables](#6-username-understanding-environmental-variables)
      + [7. `explorer`: Opening Directories and Files with Windows Explorer](#7-explorer-opening-directories-and-files-with-windows-explorer)
      + [8. Section 3 Assessment: Advanced Directory Navigation and Command Functions](#8-section-3-assessment-advanced-directory-navigation-and-command-functions)
   * [Section 4: Command Prompt Navigation Tips and Tricks](#section-4-command-prompt-navigation-tips-and-tricks)
      + [1. Navigating Command History Using the Up and Down Arrows](#1-navigating-command-history-using-the-up-and-down-arrows)
      + [2. Copying and Pasting Within the CMD](#2-copying-and-pasting-within-the-cmd)
      + [3. `doskey`: Creating Command Aliases](#3-doskey-creating-command-aliases)
   * [Section 5: Network Commands and Utilities](#section-5-network-commands-and-utilities)
      + [1. `netsh wlan show profile`: Viewing Wireless Profiles](#1-netsh-wlan-show-profile-viewing-wireless-profiles)
      + [2. `netsh`: Revealing Saved Network Passwords](#2-netsh-revealing-saved-network-passwords)
      + [3. `ipconfig`: Viewing and Managing IP Configurations](#3-ipconfig-viewing-and-managing-ip-configurations)
      + [4. `ipconfig/all`: Listing All Configurations](#4-ipconfigall-listing-all-configurations)
      + [5. `ping`: Testing Network Connectivity](#5-ping-testing-network-connectivity)
      + [6. `tracert`: Tracing the Route of Packets to a Destination](#6-tracert-tracing-the-route-of-packets-to-a-destination)
      + [7. `tasklist`: Viewing Currently Running Tasks and Processes](#7-tasklist-viewing-currently-running-tasks-and-processes)
      + [8. `netstat`: Displaying Active Network Connections](#8-netstat-displaying-active-network-connections)
      + [9. `nslookup`: Querying Domain Name Servers to Obtain Domain Names](#9-nslookup-querying-domain-name-servers-to-obtain-domain-names)
      + [10. Command Prompt Essentials: Section 5 Quiz](#10-command-prompt-essentials-section-5-quiz)
   * [Section 6: Disk and File System Management](#section-6-disk-and-file-system-management)
      + [1. `diskpart`: Managing Partitions on a Hard Drive](#1-diskpart-managing-partitions-on-a-hard-drive)
      + [2. `robocopy`: A Robust File Copying Tool, Especially for Network Operations](#2-robocopy-a-robust-file-copying-tool-especially-for-network-operations)
      + [3. `fsutil`: A Versatile Tool for Performing Many NTFS and FAT File System Tasks](#3-fsutil-a-versatile-tool-for-performing-many-ntfs-and-fat-file-system-tasks)
      + [4. `fsutil`: Special Focus on How to Check Drive Types](#4-fsutil-special-focus-on-how-to-check-drive-types)
      + [5. `convert`: Converting a Volume's File System](#5-convert-converting-a-volumes-file-system)
      + [6. `format`: Formatting a Disk for Use](#6-format-formatting-a-disk-for-use)
      + [7. `sfc`: Scanning and Fixing System Files](#7-sfc-scanning-and-fixing-system-files)
      + [8. `defrag`: Defragmenting and Optimizing Drives](#8-defrag-defragmenting-and-optimizing-drives)
   * [Section 7: Advanced Text and Network Commands](#section-7-advanced-text-and-network-commands)
      + [1. `findstr`: Advanced Text Searching with Support for Regular Expressions](#1-findstr-advanced-text-searching-with-support-for-regular-expressions)
      + [2. `net view`: Displaying a List of Computers and Resources Shared on the Network](#2-net-view-displaying-a-list-of-computers-and-resources-shared-on-the-network)
      + [3. `fc`: Comparing Two Files or Sets of Files and Displaying Differences](#3-fc-comparing-two-files-or-sets-of-files-and-displaying-differences)
      + [4. `restrui`: Launching the System Restore Utility](#4-restrui-launching-the-system-restore-utility)
      + [5. `shutdown`: Shutting Down or Restarting a Computer with Various Options](#5-shutdown-shutting-down-or-restarting-a-computer-with-various-options)
      + [6. `pathping`: Combining the Functionalities of Ping and Tracert](#6-pathping-combining-the-functionalities-of-ping-and-tracert)
      + [7. `driverquery`: Listing All Installed Device Drivers and Their Properties](#7-driverquery-listing-all-installed-device-drivers-and-their-properties)
      + [8. `wevtutil`: Querying and Managing Event Logs](#8-wevtutil-querying-and-managing-event-logs)
      + [9. `cipher`: Encrypting or Decrypting Files and Folders on NTFS Volumes](#9-cipher-encrypting-or-decrypting-files-and-folders-on-ntfs-volumes)
      + [10. `lodctr`: Updating Registry Values Associated with Windows Performance Counters](#10-lodctr-updating-registry-values-associated-with-windows-performance-counters)
      + [11. `wbadmin`: Command-line Backup Utility, Focusing on the Backup Command](#11-wbadmin-command-line-backup-utility-focusing-on-the-backup-command)
      + [12. `runas`: Executing a Tool with Different User Credentials](#12-runas-executing-a-tool-with-different-user-credentials)
   * [Section 8: Batch File Programming](#section-8-batch-file-programming)
      + [1. How to Set Name in Batch Files](#1-how-to-set-name-in-batch-files)
      + [2. Creating Batch Files](#2-creating-batch-files)
      + [3. Writing Batch Files](#3-writing-batch-files)
      + [4. User Input](#4-user-input)
      + [5. If-Else Statements](#5-if-else-statements)
      + [6. For Loops](#6-for-loops)
      + [7. While Loops](#7-while-loops)
      + [8. Functions](#8-functions)
   * [Section 8: Batch with C#](#section-8-batch-with-c)
      + [1. Create a .NET Solution](#1-create-a-net-solution)
      + [2. Add a WPF Project to the Solution](#2-add-a-wpf-project-to-the-solution)
      + [3. Add a Console Project to the Solution](#3-add-a-console-project-to-the-solution)
      + [4. Add a NuGet Package (CSV Helper)](#4-add-a-nuget-package-csv-helper)
      + [5. Clean the Solution](#5-clean-the-solution)
      + [6. Restore the NuGet Packages](#6-restore-the-nuget-packages)
      + [7. Build the Solution](#7-build-the-solution)
      + [8. Clear the NuGet Cache and Restore Again](#8-clear-the-nuget-cache-and-restore-again)
      + [9. Rebuild the Solution as x86 or x64](#9-rebuild-the-solution-as-x86-or-x64)
      + [10. Logging the Build Process](#10-logging-the-build-process)
      + [11. Zip for Distribution](#11-zip-for-distribution)
      + [12. Using 7-Zip for Distribution on Windows](#12-using-7-zip-for-distribution-on-windows)
         - [1. Install 7-Zip](#1-install-7-zip)
         - [2. Build the Solution](#2-build-the-solution)
         - [3. Zip the Output Using 7-Zip](#3-zip-the-output-using-7-zip)
         - [4. Specify the Output Path](#4-specify-the-output-path)
         - [Additional Tips](#additional-tips)
      + [13. Create a Self-Signed Certificate](#13-create-a-self-signed-certificate)
      + [14. Link Self-Signed Certificate with Projects](#14-link-self-signed-certificate-with-projects)
      + [15. Generate XML Documentation for Swagger](#15-generate-xml-documentation-for-swagger)
   * [Section 9: Advanced Batch File Automation with External Tools and Web APIs](#section-9-advanced-batch-file-automation-with-external-tools-and-web-apis)
      + [1. Using External Tools: Incorporating `curl`](#1-using-external-tools-incorporating-curl)
      + [2. Integrating Batch Files with Web APIs](#2-integrating-batch-files-with-web-apis)
      + [3. Security Considerations](#3-security-considerations)
   * [Section 10: CMD Secret Tricks](#section-10-cmd-secret-tricks)
      + [1. **Command History Navigation**](#1-command-history-navigation)
      + [2. **Redirecting Output to Clipboard**](#2-redirecting-output-to-clipboard)
      + [3. **Using Command Aliases**](#3-using-command-aliases)
      + [4. **Running Multiple Commands**](#4-running-multiple-commands)
      + [5. **Command Substitution**](#5-command-substitution)
      + [6. **Running CMD as Administrator Automatically**](#6-running-cmd-as-administrator-automatically)
      + [7. **Using `tasklist` and `taskkill`**](#7-using-tasklist-and-taskkill)
      + [8. **Finding Files with `where`**](#8-finding-files-with-where)
      + [9. **Scheduling Tasks**](#9-scheduling-tasks)
      + [10. **Redirecting Output to Multiple Files**](#10-redirecting-output-to-multiple-files)
      + [11. **Using Environment Variables**](#11-using-environment-variables)
      + [12. **Creating a Batch Script for Common Tasks**](#12-creating-a-batch-script-for-common-tasks)

<!-- TOC end -->

# Mastering the Windows Command Prompt

Mastering these advanced Command Prompt commands and batch file programming techniques will significantly enhance your productivity and ability to automate tasks in Windows. Experiment with these commands and incorporate them into your workflow to harness their full potential.

> **Note:** Use the command prompt with caution, as some commands can recursively delete files and folders or cause irreparable damage to your PC.

<!-- TOC --><a name="section-1-getting-started-with-command-prompt"></a>
## Section 1: Getting Started with Command Prompt

<!-- TOC --><a name="1-understanding-and-interpreting-command-prompt"></a>
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

<!-- TOC --><a name="2-opening-the-command-prompt"></a>
### 2. Opening the Command Prompt

- **Example 1**: Use Run dialog (Win + R) and type `cmd`.
- **Example 2**: Search "Command Prompt" in Start Menu and select it.

<!-- TOC --><a name="3-running-as-an-administrator"></a>
### 3. Running as an Administrator

- **Example 1**: Right-click on "Command Prompt" in Start Menu and select "Run as administrator."
- **Example 2**: Use Run dialog (Win + R), type `cmd`, and press Ctrl + Shift + Enter.

<!-- TOC --><a name="4-whoami-determining-the-logged-in-user"></a>
### 4. `whoami`: Determining the Logged-in User

- **Example 1**: Type `whoami` in Command Prompt.
- **Example 2**: Use `whoami /user` for detailed information.

<!-- TOC --><a name="5-cd-changing-directories-and-navigating-the-file-system"></a>
### 5. `cd`: Changing Directories and Navigating the File System

- **Example 1**: Navigate to root directory with `cd \`.
- **Example 2**: Move to a specific directory, e.g., `cd C:\Users\YourUsername\Documents`.

<!-- TOC --><a name="6-using-the-up-and-down-arrow-keys-for-navigating"></a>
### 6. Using the Up and Down Arrow Keys for Navigating

- **Example 1**: Use Up arrow to recall last command.
- **Example 2**: Use Down arrow to navigate through command history.

<!-- TOC --><a name="7-changing-a-drive-in-command-prompt"></a>
### 7. Changing a Drive in Command Prompt

- **Example**: Switch from C: to D:
  ```shell
  D:
  ```

<!-- TOC --><a name="8-tab-completion"></a>
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

<!-- TOC --><a name="9-wildcards"></a>
### 9. Wildcards

1. **Asterisk (*)**: Matches any number of characters.
   - Example: `*.txt` matches all `.txt` files.
2. **Question Mark (?)**: Matches a single character.
   - Example: `file?.txt` matches `file1.txt`, `fileA.txt`, but not `file10.txt`.

<!-- TOC --><a name="section-2-basic-command-prompt-operations"></a>
## Section 2: Basic Command Prompt Operations

<!-- TOC --><a name="1-mkdir-creating-directories"></a>
### 1. `mkdir`: Creating Directories
- **Example 1:** Create a single directory: `mkdir NewFolder`.
- **Example 2:** Create nested directories: `mkdir ParentFolder\ChildFolder`.

<!-- TOC --><a name="2-cls-clearing-the-screen"></a>
### 2. `cls`: Clearing the Screen
- **Example 1:** Type `cls` to clear the current Command Prompt screen.
- **Example 2:** Create a batch file to clear the screen: `echo cls > clear.bat`.

<!-- TOC --><a name="3-echo-displaying-messages-and-output"></a>
### 3. `echo`: Displaying Messages and Output
- **Example 1:** Display a simple message: `echo Hello, World!`.
- **Example 2:** Write output to a file: `echo This is a test > testfile.txt`.

<!-- TOC --><a name="4-copy-copying-files"></a>
### 4. `copy`: Copying Files
- **Example 1:** Copy a file to another location: `copy file.txt C:\NewFolder`.
- **Example 2:** Copy multiple files using wildcards: `copy *.txt C:\NewFolder`.

<!-- TOC --><a name="5-move-moving-files"></a>
### 5. `move`: Moving Files
- **Example 1:** Move a file to a new location: `move file.txt C:\NewFolder`.
- **Example 2:** Move all files of a specific type: `move *.txt C:\NewFolder`.

<!-- TOC --><a name="6-rename-renaming-files"></a>
### 6. `rename`: Renaming Files
- **Example 1:** Rename a single file: `rename oldfile.txt newfile.txt`.
- **Example 2:** Rename multiple files with a pattern: `rename *.txt *.bak`.

<!-- TOC --><a name="7-command-prompt-basics-navigating-and-essential-commands-quiz"></a>
### 7. Command Prompt Basics: Navigating and Essential Commands Quiz
   - **Question 1:** How do you create a new directory?
   - **Question 2:** What command clears the Command Prompt screen?
   - **Question 3:** How do you display a message in Command Prompt?

<!-- TOC --><a name="section-3-advanced-directory-navigation-and-file-management"></a>
## Section 3: Advanced Directory Navigation and File Management

<!-- TOC --><a name="1-dir-listing-contents-of-a-directory"></a>
### 1. `dir`: Listing Contents of a Directory
- **Example 1:** List all files and directories: `dir`.
- **Example 2:** List hidden files and directories: `dir /a`.

<!-- TOC --><a name="2-reading-dir-outputs"></a>
### 2. Reading `dir` Outputs
- **Example 1:** Interpret file attributes and sizes.
- **Example 2:** Use `dir /s` to list directory contents recursively.

<!-- TOC --><a name="3-creating-and-editing-files"></a>
### 3. Creating and Editing Files
- **Example 1:** Create a file using `echo`: `echo Hello > hello.txt`.
- **Example 2:** Edit a file with `notepad`: `notepad hello.txt`.

<!-- TOC --><a name="4-rmdir-removing-directories"></a>
### 4. `rmdir`: Removing Directories
- **Example 1:** Remove an empty directory: `rmdir EmptyFolder`.
- **Example 2:** Remove a directory and its contents: `rmdir /s /q FolderToRemove`.

<!-- TOC --><a name="5-help-accessing-built-in-documentation"></a>
### 5. `help`: Accessing Built-in Documentation
- **Example 1:** View help for a specific command: `help copy`.
- **Example 2:** Get detailed command syntax: `copy /?`.

<!-- TOC --><a name="6-username-understanding-environmental-variables"></a>
### 6. `%username%`: Understanding Environmental Variables
- **Example 1:** Display the current username: `echo %username%`.
- **Example 2:** Use environmental variables in paths: `cd C:\Users\%username%\Documents`.

<!-- TOC --><a name="7-explorer-opening-directories-and-files-with-windows-explorer"></a>
### 7. `explorer`: Opening Directories and Files with Windows Explorer
- **Example 1:** Open a directory: `explorer C:\NewFolder`.
- **Example 2:** Open a specific file: `explorer C:\NewFolder\file.txt`.

<!-- TOC --><a name="8-section-3-assessment-advanced-directory-navigation-and-command-functions"></a>
### 8. Section 3 Assessment: Advanced Directory Navigation and Command Functions
   - **Question 1:** How do you list all files, including hidden ones?
   - **Question 2:** What command removes a directory and its contents?
   - **Question 3:** How do you view help for the `copy` command?
   - **Question 4:** How do you open a directory with Windows Explorer?

<!-- TOC --><a name="section-4-command-prompt-navigation-tips-and-tricks"></a>
## Section 4: Command Prompt Navigation Tips and Tricks

<!-- TOC --><a name="1-navigating-command-history-using-the-up-and-down-arrows"></a>
### 1. Navigating Command History Using the Up and Down Arrows
- **Example 1:** Use the Up arrow to recall previous commands.
- **Example 2:** Use the Down arrow to navigate through the command history.

<!-- TOC --><a name="2-copying-and-pasting-within-the-cmd"></a>
### 2. Copying and Pasting Within the CMD
- **Example 1:** Enable QuickEdit Mode for easier copy-pasting.
- **Example 2:** Use Ctrl + C to copy and Ctrl + V to paste.

<!-- TOC --><a name="3-doskey-creating-command-aliases"></a>
### 3. `doskey`: Creating Command Aliases
- **Example 1:** Create an alias for a command: `doskey ll=dir`.
- **Example 2:** Create a macro with parameters: `doskey gdrive=cd /d D:\GoogleDrive\ $*`.

<!-- TOC --><a name="section-5-network-commands-and-utilities"></a>
## Section 5: Network Commands and Utilities

<!-- TOC --><a name="1-netsh-wlan-show-profile-viewing-wireless-profiles"></a>
### 1. `netsh wlan show profile`: Viewing Wireless Profiles
- **Example 1:** List all wireless profiles: `netsh wlan show profiles`.
- **Example 2:** View details of a specific profile: `netsh wlan show profile name="ProfileName"`.

<!-- TOC --><a name="2-netsh-revealing-saved-network-passwords"></a>
### 2. `netsh`: Revealing Saved Network Passwords
Ensure the Folder Exists: The folder specified in the command must already exist. Create the folder C:\WiFiProfiles if it doesn’t exist before running the command.
- **Example 1:** Display the password of a saved network: `netsh wlan show profile name="ProfileName" key=clear`.
- **Example 2:** Export wireless profiles: `netsh wlan export profile folder=C:\WiFiProfiles`.

<!-- TOC --><a name="3-ipconfig-viewing-and-managing-ip-configurations"></a>
### 3. `ipconfig`: Viewing and Managing IP Configurations
- **Example 1:** Display IP configuration: `ipconfig`.
- **Example 2:** Release and renew IP addresses: `ipconfig /release` and `ipconfig /renew`.

<!-- TOC --><a name="4-ipconfigall-listing-all-configurations"></a>
### 4. `ipconfig/all`: Listing All Configurations
- **Example 1:** View detailed IP configuration: `ipconfig /all`.
- **Example 2:** Save the output to a file: `ipconfig /all > ipconfig.txt`.

<!-- TOC --><a name="5-ping-testing-network-connectivity"></a>
### 5. `ping`: Testing Network Connectivity
- **Example 1:** Ping a website: `ping google.com`.
- **Example 2:** Ping with a specific number of requests: `ping google.com -n 10`.

<!-- TOC --><a name="6-tracert-tracing-the-route-of-packets-to-a-destination"></a>
### 6. `tracert`: Tracing the Route of Packets to a Destination
- **Example 1:** Trace the route to a website: `tracert google.com`.
- **Example 2:** Save the route information to a file: `tracert google.com > tracert.txt`.

<!-- TOC --><a name="7-tasklist-viewing-currently-running-tasks-and-processes"></a>
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

<!-- TOC --><a name="8-netstat-displaying-active-network-connections"></a>
### 8. `netstat`: Displaying Active Network Connections
- **Example 1:** View all active connections: `netstat`.
- **Example 2:** Display network statistics: `netstat -e`.

<!-- TOC --><a name="9-nslookup-querying-domain-name-servers-to-obtain-domain-names"></a>
### 9. `nslookup`: Querying Domain Name Servers to Obtain Domain Names
- **Example 1:** Find the IP address of a domain: `nslookup google.com`.
- **Example 2:** Query a specific DNS server: `nslookup google.com 8.8.8.8`.

<!-- TOC --><a name="10-command-prompt-essentials-section-5-quiz"></a>
### 10. Command Prompt Essentials: Section 5 Quiz
   - **Question 1:** How do you view wireless profiles?
   - **Question 2:** What command reveals saved network passwords?
   - **Question 3:** How do you list all IP configurations?
   - **Question 4:** What command tests network connectivity?

<!-- TOC --><a name="section-6-disk-and-file-system-management"></a>
## Section 6: Disk and File System Management

<!-- TOC --><a name="1-diskpart-managing-partitions-on-a-hard-drive"></a>
### 1. `diskpart`: Managing Partitions on a Hard Drive
- **Example 1:** List all disks: `diskpart` followed by `list disk`.
- **Example 2:** Create a new partition: `diskpart` followed by `create partition primary`.

<!-- TOC --><a name="2-robocopy-a-robust-file-copying-tool-especially-for-network-operations"></a>
### 2. `robocopy`: A Robust File Copying Tool, Especially for Network Operations
- **Example 1:** Copy files with attributes: `robocopy C:\Source C
:\Destination /COPY:DAT`.
- **Example 2:** Mirror directories: `robocopy C:\Source C:\Destination /MIR`.

<!-- TOC --><a name="3-fsutil-a-versatile-tool-for-performing-many-ntfs-and-fat-file-system-tasks"></a>
### 3. `fsutil`: A Versatile Tool for Performing Many NTFS and FAT File System Tasks
- **Example 1:** Check drive type: `fsutil fsinfo drivetype C:`.
- **Example 2:** Create a hard link: `fsutil hardlink create newfile.txt existingfile.txt`.

<!-- TOC --><a name="4-fsutil-special-focus-on-how-to-check-drive-types"></a>
### 4. `fsutil`: Special Focus on How to Check Drive Types
- **Example 1:** Verify if a drive is a fixed drive: `fsutil fsinfo drivetype C:`.
- **Example 2:** Check if a drive is removable: `fsutil fsinfo drivetype D:`.

<!-- TOC --><a name="5-convert-converting-a-volumes-file-system"></a>
### 5. `convert`: Converting a Volume's File System
- **Example 1:** Convert FAT32 to NTFS: `convert C: /FS:NTFS`.
- **Example 2:** Convert a volume with parameters: `convert E: /FS:NTFS /V`.

<!-- TOC --><a name="6-format-formatting-a-disk-for-use"></a>
### 6. `format`: Formatting a Disk for Use
- **Example 1:** Quick format a drive: `format E: /Q /FS:NTFS`.
- **Example 2:** Format with a specific allocation unit size: `format F: /A:4096`.

<!-- TOC --><a name="7-sfc-scanning-and-fixing-system-files"></a>
### 7. `sfc`: Scanning and Fixing System Files
- **Example 1:** Scan and repair system files: `sfc /scannow`.
- **Example 2:** Verify only (without repairing): `sfc /verifyonly`.

<!-- TOC --><a name="8-defrag-defragmenting-and-optimizing-drives"></a>
### 8. `defrag`: Defragmenting and Optimizing Drives
- **Example 1:** Defragment a drive: `defrag C: /O`.
- **Example 2:** Analyze a drive before defragmenting: `defrag D: /A`.

<!-- TOC --><a name="section-7-advanced-text-and-network-commands"></a>
## Section 7: Advanced Text and Network Commands

<!-- TOC --><a name="1-findstr-advanced-text-searching-with-support-for-regular-expressions"></a>
### 1. `findstr`: Advanced Text Searching with Support for Regular Expressions
- **Example 1:** Search for a specific string in files: `findstr "search text" *.txt`.
- **Example 2:** Use regular expressions: `findstr /R "regex_pattern" file.txt`.

<!-- TOC --><a name="2-net-view-displaying-a-list-of-computers-and-resources-shared-on-the-network"></a>
### 2. `net view`: Displaying a List of Computers and Resources Shared on the Network
- **Example 1:** List all computers on the network: `net view`.
- **Example 2:** View shared resources of a specific computer: `net view \\ComputerName`.

<!-- TOC --><a name="3-fc-comparing-two-files-or-sets-of-files-and-displaying-differences"></a>
### 3. `fc`: Comparing Two Files or Sets of Files and Displaying Differences
- **Example 1:** Compare two text files: `fc file1.txt file2.txt`.
- **Example 2:** Compare binary files: `fc /b file1.exe file2.exe`.

<!-- TOC --><a name="4-restrui-launching-the-system-restore-utility"></a>
### 4. `restrui`: Launching the System Restore Utility
- **Example 1:** Open System Restore interface: `restrui`.
- **Example 2:** Start System Restore with a specific restore point: `restrui /offline:C:\windows=active`.

<!-- TOC --><a name="5-shutdown-shutting-down-or-restarting-a-computer-with-various-options"></a>
### 5. `shutdown`: Shutting Down or Restarting a Computer with Various Options
- **Example 1:** Shutdown the computer: `shutdown /s /f /t 0`.
- **Example 2:** Restart the computer: `shutdown /r /f /t 0`.

<!-- TOC --><a name="6-pathping-combining-the-functionalities-of-ping-and-tracert"></a>
### 6. `pathping`: Combining the Functionalities of Ping and Tracert
- **Example 1:** Perform a pathping to a website: `pathping google.com`.
- **Example 2:** Save pathping results to a file: `pathping google.com > pathping.txt`.

<!-- TOC --><a name="7-driverquery-listing-all-installed-device-drivers-and-their-properties"></a>
### 7. `driverquery`: Listing All Installed Device Drivers and Their Properties
- **Example 1:** List all drivers: `driverquery`.
- **Example 2:** Export driver list to a CSV file: `driverquery /fo csv /v > drivers.csv`.

<!-- TOC --><a name="8-wevtutil-querying-and-managing-event-logs"></a>
### 8. `wevtutil`: Querying and Managing Event Logs
- **Example 1:** List all event logs: `wevtutil el`.
- **Example 2:** Export a specific event log: `wevtutil epl System systemlog.evtx`.

<!-- TOC --><a name="9-cipher-encrypting-or-decrypting-files-and-folders-on-ntfs-volumes"></a>
### 9. `cipher`: Encrypting or Decrypting Files and Folders on NTFS Volumes
- **Example 1:** Encrypt a folder: `cipher /e /s:C:\EncryptedFolder`.
- **Example 2:** Decrypt a file: `cipher /d C:\EncryptedFolder\file.txt`.

<!-- TOC --><a name="10-lodctr-updating-registry-values-associated-with-windows-performance-counters"></a>
### 10. `lodctr`: Updating Registry Values Associated with Windows Performance Counters
- **Example 1:** Update performance counters: `lodctr /R`.
- **Example 2:** Backup performance counter settings: `lodctr /S:backup.ini`.

<!-- TOC --><a name="11-wbadmin-command-line-backup-utility-focusing-on-the-backup-command"></a>
### 11. `wbadmin`: Command-line Backup Utility, Focusing on the Backup Command
- **Example 1:** Create a backup of the C: drive: `wbadmin start backup -backupTarget:D: -include:C: -quiet`.
- **Example 2:** List details of backups: `wbadmin get versions`.

<!-- TOC --><a name="12-runas-executing-a-tool-with-different-user-credentials"></a>
### 12. `runas`: Executing a Tool with Different User Credentials
- **Example 1:** Run a program as another user: `runas /user:domain\username "program.exe"`.
- **Example 2:** Run a program with elevated privileges: `runas /noprofile /user:Administrator cmd`.

<!-- TOC --><a name="section-8-batch-file-programming"></a>
## Section 8: Batch File Programming

<!-- TOC --><a name="1-how-to-set-name-in-batch-files"></a>
### 1. How to Set Name in Batch Files
- **Example 1:** Set and display a variable: `set name=John & echo %name%`.
- **Example 2:** Use variables in a script: 
  ```batch
  @echo off
  set name=John
  echo Hello, %name%
  ```

<!-- TOC --><a name="2-creating-batch-files"></a>
### 2. Creating Batch Files
- **Example 1:** Create a simple batch file: `echo echo Hello > hello.bat`.
- **Example 2:** Create a batch file to automate tasks: 
  ```batch
  @echo off
  mkdir NewFolder
  cd NewFolder
  echo This is a test file > testfile.txt
  ```

<!-- TOC --><a name="3-writing-batch-files"></a>
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

<!-- TOC --><a name="4-user-input"></a>
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

<!-- TOC --><a name="5-if-else-statements"></a>
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

<!-- TOC --><a name="6-for-loops"></a>
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

<!-- TOC --><a name="7-while-loops"></a>
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

<!-- TOC --><a name="8-functions"></a>
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

<!-- TOC --><a name="section-8-batch-with-c"></a>
## Section 8: Batch with C#

<!-- TOC --><a name="1-create-a-net-solution"></a>
### 1. Create a .NET Solution
**Steps to create a new .NET solution using the Command Prompt:**
- Open Command Prompt.
- Navigate to the desired directory.
- Run the following command:
  ```bash
  dotnet new sln -n MySolution
  ```
  This creates a new solution named `MySolution`.

<!-- TOC --><a name="2-add-a-wpf-project-to-the-solution"></a>
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

<!-- TOC --><a name="3-add-a-console-project-to-the-solution"></a>
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

<!-- TOC --><a name="4-add-a-nuget-package-csv-helper"></a>
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

<!-- TOC --><a name="5-clean-the-solution"></a>
### 5. Clean the Solution
**Steps to clean the solution using Command Prompt:**
- Run the following command to clean the solution:
  ```bash
  dotnet clean MySolution.sln
  ```
- **Importance:** Cleaning the solution helps remove any build artifacts and ensures a fresh build environment.

<!-- TOC --><a name="6-restore-the-nuget-packages"></a>
### 6. Restore the NuGet Packages
**How to restore the NuGet packages for the projects:**
- Run the following command to restore packages:
  ```bash
  dotnet restore MySolution.sln
  ```

<!-- TOC --><a name="7-build-the-solution"></a>
### 7. Build the Solution
**Steps to build the solution using Command Prompt:**
- Run the following command to build the solution:
  ```bash
  dotnet build MySolution.sln
  ```

<!-- TOC --><a name="8-clear-the-nuget-cache-and-restore-again"></a>
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

<!-- TOC --><a name="9-rebuild-the-solution-as-x86-or-x64"></a>
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

<!-- TOC --><a name="10-logging-the-build-process"></a>
### 10. Logging the Build Process
**Methods to log the build process output:**
- Use the following command to log the build process:
  ```bash
  dotnet build MySolution.sln > build.log
  ```
  This logs the build output to `build.log`.

<!-- TOC --><a name="11-zip-for-distribution"></a>
### 11. Zip for Distribution
**Steps to zip the built solution for distribution:**
- Use the following command to zip the output, including date, time, and version:
  ```bash
  tar -cvzf MySolution_$(date +%Y%m%d_%H%M%S)_v1.0.0.tar.gz MySolution/bin/Release
  ```
  Specify the output path as needed.
  
<!-- TOC --><a name="12-using-7-zip-for-distribution-on-windows"></a>
### 12. Using 7-Zip for Distribution on Windows

If `zip` is not available, you can use 7-Zip to create zip files. Here’s how to zip your built solution for distribution using 7-Zip on Windows:

<!-- TOC --><a name="1-install-7-zip"></a>
#### 1. Install 7-Zip

1. Download and install [7-Zip](https://www.7-zip.org/).

<!-- TOC --><a name="2-build-the-solution"></a>
#### 2. Build the Solution

Ensure your .NET solution is built and the output is available in the specified directory (e.g., `MySolution\bin\Release`).

<!-- TOC --><a name="3-zip-the-output-using-7-zip"></a>
#### 3. Zip the Output Using 7-Zip

1. Open Command Prompt.

2. Use the following command to create a zip file with the date, time, and version in the filename:

   ```cmd
   "C:\Program Files\7-Zip\7z.exe" a -tzip MySolution_%date:~10,4%%date:~4,2%%date:~7,2%_%time:~0,2%%time:~3,2%_v1.0.0.zip MySolution\bin\Release
   ```

   - `a`: Add files to the archive.
   - `-tzip`: Specify the zip format.

<!-- TOC --><a name="4-specify-the-output-path"></a>
#### 4. Specify the Output Path

To specify a different output path, include the full path in the filename:

```cmd
"C:\Program Files\7-Zip\7z.exe" a -tzip C:\path\to\output\MySolution_%date:~10,4%%date:~4,2%%date:~7,2%_%time:~0,2%%time:~3,2%_v1.0.0.zip C:\path\to\MySolution\bin\Release
```

<!-- TOC --><a name="additional-tips"></a>
#### Additional Tips

- **Date and Time Format**: Adjust the date and time format in `%date%` and `%time%` as needed.
- **Versioning**: Update the version number (`v1.0.0`) to reflect the version of your solution.

<!-- TOC --><a name="13-create-a-self-signed-certificate"></a>
### 13. Create a Self-Signed Certificate
**Instructions to create a self-signed certificate:**
- Run the following command:
  ```bash
  dotnet dev-certs https -ep ./MyCert.pfx -p password
  ```

<!-- TOC --><a name="14-link-self-signed-certificate-with-projects"></a>
### 14. Link Self-Signed Certificate with Projects
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

<!-- TOC --><a name="15-generate-xml-documentation-for-swagger"></a>
### 15. Generate XML Documentation for Swagger
**Instructions to generate XML documentation for Swagger:**
- Update the project files (`.csproj`) to generate XML documentation:
  ```xml
  <PropertyGroup>
    <GenerateDocumentationFile>true</GenerateDocumentationFile>
  </PropertyGroup>
  ```
- Build the project to generate the XML documentation.

<!-- TOC --><a name="section-9-advanced-batch-file-automation-with-external-tools-and-web-apis"></a>
## Section 9: Advanced Batch File Automation with External Tools and Web APIs

By combining batch files with external tools like `curl` and integrating them with web APIs, you can automate complex tasks and handle HTTP requests efficiently. Incorporating error handling, debugging, and scheduling enhances the robustness and flexibility of your automation workflows. For more advanced scenarios, leveraging PowerShell for additional processing can significantly extend the capabilities of your batch file automation.

<!-- TOC --><a name="1-using-external-tools-incorporating-curl"></a>
### 1. Using External Tools: Incorporating `curl`

**`curl`** is a command-line tool for making HTTP requests. It allows batch files to interact with web APIs for fetching, sending, and processing data.

**Basic API Requests:**

- **Fetch Data:**
  ```bat
  @echo off
  curl -X GET "https://api.example.com/data" -o response.json
  echo Data fetched and saved to response.json
  ```

- **Post Data:**
  ```bat
  @echo off
  curl -X POST "https://api.example.com/submit" -H "Content-Type: application/json" -d "{\"key\":\"value\"}" -o response.json
  echo Data posted and response saved to response.json
  ```

**Handling API Responses:**

- **Read Response:**
  ```bat
  @echo off
  curl -X GET "https://api.example.com/data" -o response.json
  type response.json
  ```

- **Process JSON with `jq`:**
  ```bat
  @echo off
  curl -X GET "https://api.example.com/data" -o response.json
  jq ".key" response.json
  ```

**Error Handling:**
```bat
@echo off
curl -X GET "https://api.example.com/data" -o response.json
if %ERRORLEVEL% NEQ 0 (
    echo Error occurred
    exit /b %ERRORLEVEL%
)
echo Data fetched successfully
```

**Debugging:**
```bat
@echo off
curl -v -X GET "https://api.example.com/data"
```

<!-- TOC --><a name="2-integrating-batch-files-with-web-apis"></a>
### 2. Integrating Batch Files with Web APIs

Batch files can automate web API interactions, enabling you to schedule tasks and process data seamlessly.

**Automating Tasks:**

- **Schedule Batch Files:** Use Task Scheduler to automate the execution of batch files.
  - Open **Task Scheduler** and create a new task.
  - Set triggers (e.g., daily) and actions (e.g., run your batch file).

**Example Scheduled Task:**

Create a batch file `fetch_data.bat`:
```bat
@echo off
curl -X GET "https://api.example.com/data" -o response.json
```

Schedule it using Task Scheduler for daily execution.

**Combining with PowerShell:**

For advanced processing, batch files can call PowerShell scripts:
```bat
@echo off
curl -X GET "https://api.example.com/data" -o response.json
powershell -File process_data.ps1
```

**Example PowerShell Script (`process_data.ps1`):**
```powershell
$response = Get-Content response.json | ConvertFrom-Json
$response.key
```

<!-- TOC --><a name="3-security-considerations"></a>
### 3. Security Considerations

**Handling Sensitive Data:**

- Use environment variables to manage API keys and sensitive information.
- Example with environment variables:
  ```bat
  @echo off
  set API_KEY=%MY_API_KEY%
  curl -X GET "https://api.example.com/data?api_key=%API_KEY%" -o response.json
  ```

Ensure proper permissions and avoid hardcoding sensitive information directly into your scripts.

<!-- TOC --><a name="section-10-cmd-secret-tricks"></a>
## Section 10: CMD Secret Tricks

The Windows Command Prompt (CMD) is packed with hidden gems and secret tricks that can significantly enhance your productivity. This section explores some of these advanced features, providing practical examples to help you leverage CMD to its fullest.

<!-- TOC --><a name="1-command-history-navigation"></a>
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

<!-- TOC --><a name="2-redirecting-output-to-clipboard"></a>
### 2. **Redirecting Output to Clipboard**

You can quickly copy the output of a command to the clipboard using the `clip` command.

**Example:**

```cmd
C:\>dir | clip
```

This command copies the directory listing to the clipboard. You can paste it into a document or an email.

<!-- TOC --><a name="3-using-command-aliases"></a>
### 3. **Using Command Aliases**

CMD allows you to create aliases for long commands using `doskey`.

**Example:**

```cmd
C:\>doskey ll=dir /w /p
```

Now, typing `ll` will execute `dir /w /p`, which lists the directory in wide format with pagination.

<!-- TOC --><a name="4-running-multiple-commands"></a>
### 4. **Running Multiple Commands**

You can execute multiple commands in a single line using `&&` (execute next command only if the previous succeeds) or `||` (execute next command only if the previous fails).

**Example:**

```cmd
C:\>mkdir TestFolder && cd TestFolder && echo Hello > hello.txt
```

This creates a folder, navigates into it, and creates a file with content in one line.

<!-- TOC --><a name="5-command-substitution"></a>
### 5. **Command Substitution**

You can use the `for` loop to execute a command and use its output in another command.

**Example:**

```cmd
C:\>for /f "tokens=*" %i in ('date /t') do echo Today is %i
```

This command captures the output of `date /t` and uses it to print "Today is" followed by the current date.

<!-- TOC --><a name="6-running-cmd-as-administrator-automatically"></a>
### 6. **Running CMD as Administrator Automatically**

Create a shortcut to CMD that always runs as an administrator:

1. Right-click on the desktop and select "New > Shortcut."
2. Enter `cmd.exe` and click "Next."
3. Name the shortcut and click "Finish."
4. Right-click the new shortcut, select "Properties."
5. Click on "Advanced" and check "Run as administrator."

<!-- TOC --><a name="7-using-tasklist-and-taskkill"></a>
### 7. **Using `tasklist` and `taskkill`**

You can list and terminate processes directly from CMD.

**Example:**

```cmd
C:\>tasklist
C:\>taskkill /im notepad.exe /f
```

The first command lists all running processes, and the second command forcefully terminates Notepad.

<!-- TOC --><a name="8-finding-files-with-where"></a>
### 8. **Finding Files with `where`**

The `where` command helps locate files in your directories.

**Example:**

```cmd
C:\>where python
```

This command finds the path of the `python` executable.

<!-- TOC --><a name="9-scheduling-tasks"></a>
### 9. **Scheduling Tasks**

Use `schtasks` to schedule tasks to run at specific times.

**Example:**

```cmd
C:\>schtasks /create /tn "Backup" /tr "C:\Backup.bat" /sc daily /st 14:00
```

This schedules a task named "Backup" to run `C:\Backup.bat` daily at 2 PM.

<!-- TOC --><a name="10-redirecting-output-to-multiple-files"></a>
### 10. **Redirecting Output to Multiple Files**

You can redirect output to multiple files using `tee`.

**Example:**

```cmd
C:\>dir | tee file1.txt | tee file2.txt
```

This command writes the output of `dir` to both `file1.txt` and `file2.txt`.

<!-- TOC --><a name="11-using-environment-variables"></a>
### 11. **Using Environment Variables**

Environment variables can be set and used within CMD.

**Example:**

```cmd
C:\>set MYVAR=HelloWorld
C:\>echo %MYVAR%
HelloWorld
```

This sets a variable `MYVAR` and then prints its value.

<!-- TOC --><a name="12-creating-a-batch-script-for-common-tasks"></a>
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

