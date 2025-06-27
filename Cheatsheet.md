### 1. ADMINISTRATOR COMMANDS
#### 1.1 Open CMD as Admin
- `Win + R` → type `cmd` → `Ctrl+Shift+Enter`

#### 1.2 Run Command as Admin
```cmd
runas /user:Administrator <command>
```

#### 1.3 Multiple Commands
```cmd
command1 & command2      # Run sequentially
command1 && command2     # Run second only if first succeeds
command1 || command2     # Run second only if first fails
```

#### 1.4 Windows Package Manager
```cmd
pkgmgr /iu:"TelnetClient"
telnet localhost 1433
```

### 2. ADVANCED COMMANDS
#### 2.1 Output Redirection
```cmd
dir > output.txt      # Overwrite
dir >> output.txt     # Append
```

#### 2.2 Pipe Output
```cmd
dir | find "txt"
```

#### 2.3 Clipboard
```cmd
dir | clip
```

#### 2.4 Command History
```cmd
doskey /history
```

#### 2.5 Echo
```cmd
echo [%DATE% %TIME%] Running backup... >> script.log
```

#### 2.6 Silent Execution
```cmd
yourcommand >nul 2>&1
```

### 3. DIRECTORY COMMANDS
| Command | Description |
|---------|-------------|
| `dir /w` | Wide list format |
| `dir /p` | Pause after each screen |
| `dir /a` | Show hidden/system files |
| `dir /s` | Recursive listing |
| `dir /b` | Bare filenames only |
| `cd ..` | Go up one level |
| `cd \` | Go to root |
| `cd /d "D:\Projects"` | Change drive+directory |
| `C:\Users\%username%\Desktop` | Go to desktop |
| `cd %USERPROFILE%\Desktop` | Go to desktop |

### 4. FILE & FOLDER OPERATIONS
#### 4.1 Create Directory
```cmd
mkdir NewFolder
```

#### 4.2 Move Folder (Recursive)
```cmd
xcopy "C:\Source" "D:\Dest" /E /I /H
```

#### 4.3 Combine Files
```cmd
copy /b file1.txt + file2.txt combined.txt
```

#### 4.4 Recursive Delete
```cmd
del /s *.log           # Delete files
rmdir /s /q FolderName # Delete folder
```

#### 4.5 File Operations
```cmd
type nul > file.txt            # Create blank file
echo Hello > file.txt          # Create with content
rename old.txt new.txt         # Rename
attrib +h +r file.txt          # Hide + read-only
icacls "Folder" /grant User:F  # Permissions (F=Full)
```

### 5. ENVIRONMENT VARIABLES
#### Temporary:
```cmd
set MYVAR=Hello
echo %MYVAR%
if "%MYVAR%"=="HelloWorld" echo It's working
```

#### Permanent:
```cmd
setx MYVAR "Hello"
```

### 6. SCHEDULING
```cmd
schtasks /create /tn "Backup" /tr "C:\backup.bat" /sc daily /st 14:00
```

### 7. PROCESS MANAGEMENT
```cmd
tasklist | more                         # List processes
taskkill /F /IM chrome.exe              # Force kill
whoami /user                            # Current user
net start/stop <Service Name>           # Start/Stop service
```

### 8. SYSTEM COMMANDS
```cmd
hostname                          # Computer name
shutdown /r /t 0                  # Immediate restart
net statistics workstation        # Check uptime
time 14:30:00                     # Set system time
```

### 9. NETWORK COMMANDS
#### 9.1 Basic Networking
```cmd
ping -t google.com                # Continuous ping
ping google.com -n 5              # Numbered ping
ipconfig /all                     # Network config
ipconfig /release && ipconfig /renew # Refresh IP
```

#### 9.2 Port Management
```cmd
netstat -ano | findstr ":443"     # Find port usage
tasklist /fi "pid eq 1234"        # Find process by PID
```

#### 9.3 Release & Renew IP
```cmd
ipconfig /flushdns
ipconfig /release
ipconfig /renew
ipconfig /all
```

#### 9.4 WiFi Passwords
```cmd
netsh wlan show profiles
netsh wlan show profile name="SSID" key=clear
```

#### 9.5 HTTP Requests
```cmd
curl -X GET "https://api.example.com" -o response.json
```
