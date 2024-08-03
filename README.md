# Cmdprompt
Command list
Here is the extensive list of commands for cmdprompt CLI only.

## System Information and Management

- **Get system information:**
  ```cmd
  systeminfo
  ```

- **List all running processes:**
  ```cmd
  tasklist
  ```

- **Get detailed information about a specific process:**
  ```cmd
  tasklist /v /fi "imagename eq processname.exe"
  ```

- **List all installed programs:**
  ```cmd
  wmic product get name,version
  ```

- **Check system disk usage:**
  ```cmd
  chkdsk
  ```

- **Check disk space:**
  ```cmd
  dir
  ```

- **Check network configuration:**
  ```cmd
  ipconfig /all
  ```

- **List all network connections and listening ports:**
  ```cmd
  netstat -an
  ```

- **View current active connections:**
  ```cmd
  netstat -a
  ```

## File and Directory Management

- **List files and directories in the current directory:**
  ```cmd
  dir
  ```

- **Create a new directory:**
  ```cmd
  mkdir directoryname
  ```

- **Delete a directory:**
  ```cmd
  rmdir /s /q directoryname
  ```

- **Copy files:**
  ```cmd
  copy sourcefile destinationfile
  ```

- **Move files:**
  ```cmd
  move sourcefile destinationfile
  ```

- **Delete files:**
  ```cmd
  del filename
  ```

- **Search for files:**
  ```cmd
  dir /s /b filename
  ```

- **Find files containing specific text:**
  ```cmd
  findstr /s /i "searchtext" *.*
  ```

## Network Commands

- **Ping a host:**
  ```cmd
  ping hostname
  ```

- **Trace route to a host:**
  ```cmd
  tracert hostname
  ```

- **Test network connection to a port:**
  ```cmd
  telnet hostname port
  ```

- **View routing table:**
  ```cmd
  route print
  ```

- **Flush DNS cache:**
  ```cmd
  ipconfig /flushdns
  ```

- **Display network shares:**
  ```cmd
  net share
  ```

## User and Group Management

- **List all users:**
  ```cmd
  net user
  ```

- **Add a new user:**
  ```cmd
  net user username password /add
  ```

- **Delete a user:**
  ```cmd
  net user username /delete
  ```

- **Add a user to a group:**
  ```cmd
  net localgroup groupname username /add
  ```

- **Remove a user from a group:**
  ```cmd
  net localgroup groupname username /delete
  ```

## Security and Permissions

- **Check file permissions:**
  ```cmd
  icacls filename
  ```

- **Change file permissions:**
  ```cmd
  icacls filename /grant username:(permissions)
  ```

- **View active network connections:**
  ```cmd
  netstat -ano
  ```

- **Stop a process by PID:**
  ```cmd
  taskkill /PID pidnumber
  ```

- **Start a process:**
  ```cmd
  start processname.exe
  ```

## System and Application Logs

- **View Windows Event Logs:**
  ```cmd
  eventvwr
  ```

- **Export Event Log to a file:**
  ```cmd
  wevtutil epl "logname" "filename.evtx"
  ```

- **View specific log entries:**
  ```cmd
  wevtutil qe "logname" /q:"*[System[(EventID=number)]]" /f:text
  ```

## System Maintenance

- **Run system file checker:**
  ```cmd
  sfc /scannow
  ```

- **Check for Windows updates:**
  ```cmd
  wuauclt /detectnow
  ```

- **Clean temporary files:**
  ```cmd
  del /q /f %temp%\*
  ```

- **Update Windows Defender:**
  ```cmd
  MpCmdRun.exe -SignatureUpdate
  ```

## Summary

This list covers a broad range of `cmd` commands for system administration, security, file management, network diagnostics, and more. Commands are organized by category to facilitate efficient use in various administrative and troubleshooting tasks. Always ensure to run commands with the appropriate privileges and follow best practices for system management.
```
