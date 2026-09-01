# Windows 11 Useful Command Prompt and PowerShell Commands

Windows 11 includes several built-in command-line tools that can help with system information, network troubleshooting, file management, and basic system maintenance.

This guide covers simple and useful commands for everyday Windows 11 users.

## Open Command Prompt

To open Command Prompt:

1. Press `Windows + S`.
2. Type `Command Prompt`.
3. Select the Command Prompt app.

For some commands, you may need to open Command Prompt as an administrator.

## Check System Information

The `systeminfo` command displays detailed information about your Windows installation and computer.

Command: `systeminfo`

It can show information such as:

- Windows version
- System manufacturer
- System model
- Installed memory
- System boot information
- Network information

This command is useful when you need basic details about your computer.

## Check IP Configuration

The `ipconfig` command displays basic network configuration information.

Command: `ipconfig`

For more detailed information, use:

Command: `ipconfig /all`

This can be useful when troubleshooting network connection problems.

## Refresh Your IP Address

Windows provides commands that can help refresh your network configuration.

To release the current IP address:

Command: `ipconfig /release`

Then request a new IP address:

Command: `ipconfig /renew`

These commands are commonly used for basic network troubleshooting.

## Test Your Internet Connection

The `ping` command can test whether your computer can communicate with a network destination.

Example: `ping google.com`

You can use this command to check whether a destination responds to network requests.

## Check Windows System Files

Windows includes the System File Checker tool, also known as SFC.

Open Command Prompt as an administrator and run:

Command: `sfc /scannow`

Windows will scan protected system files and attempt to repair problems when possible.

The scan can take some time, so allow it to finish before closing the Command Prompt window.

## Check the Windows Image

Windows also includes the Deployment Image Servicing and Management tool, commonly called DISM.

To check the health of the Windows image, open Command Prompt as an administrator and run:

Command: `DISM /Online /Cleanup-Image /CheckHealth`

For a more detailed scan, you can use:

Command: `DISM /Online /Cleanup-Image /ScanHealth`

If Windows reports component-store problems, follow Microsoft's recommended repair guidance before making further changes.

## Check a Disk

The `chkdsk` command can check a disk for file-system errors.

For a basic check, use:

Command: `chkdsk`

Additional parameters can perform repairs or other operations. Before using repair-related options, make sure you understand what the command will do.

## View Running Processes

The `tasklist` command displays currently running processes.

Command: `tasklist`

This can help you see which applications and processes are currently running on your computer.

## View Network Connections

The `netstat` command can display active network connections.

Command: `netstat`

For more detailed information, use:

Command: `netstat -ano`

This can be useful when troubleshooting network-related issues.

## Open Windows Settings

You can open the main Windows Settings application directly from Command Prompt.

Command: `start ms-settings:`

This can save time when you are already working in Command Prompt.

## Open Task Manager

Task Manager can be launched from Command Prompt with:

Command: `taskmgr`

Task Manager can help you check:

- Running applications
- Background processes
- CPU usage
- Memory usage
- Startup applications

## Open Device Manager

Device Manager lets you view hardware devices and manage their drivers.

Command: `devmgmt.msc`

This can be useful when troubleshooting hardware or driver-related problems.

## Open Disk Management

Disk Management provides tools for viewing connected storage devices and partitions.

Command: `diskmgmt.msc`

Be careful when making changes to partitions or disks because incorrect changes can result in data loss.

## Use PowerShell for System Information

PowerShell is another command-line environment included with Windows.

To view computer information, use:

Command: `Get-ComputerInfo`

This command can return a large amount of information about the Windows system.

## Quick Command Reference

| Purpose | Command |
|---|---|
| System information | `systeminfo` |
| IP configuration | `ipconfig` |
| Detailed IP configuration | `ipconfig /all` |
| Release IP address | `ipconfig /release` |
| Renew IP address | `ipconfig /renew` |
| Test network connection | `ping` |
| Check system files | `sfc /scannow` |
| Check Windows image | `DISM /Online /Cleanup-Image /CheckHealth` |
| View running processes | `tasklist` |
| View network connections | `netstat` |
| Open Windows Settings | `start ms-settings:` |
| Open Task Manager | `taskmgr` |
| Open Device Manager | `devmgmt.msc` |
| Open Disk Management | `diskmgmt.msc` |

## Important Safety Tips

Command-line tools can access important parts of Windows.

Before running a command:

- Understand what the command does.
- Use administrator mode only when necessary.
- Avoid commands copied from unknown sources.
- Do not delete or modify system files unless you know why.
- Back up important files before performing major system maintenance.
- Be especially careful with commands that can modify disks, partitions, or system settings.

## Conclusion

Windows 11 includes many built-in command-line tools that can help with everyday troubleshooting and system management.

Start with simple commands such as `systeminfo`, `ipconfig`, and `ping`. For system repair tools such as SFC and DISM, allow the process to complete and follow Microsoft's guidance when additional steps are required.

More practical Windows 11 guides will be added to this repository over time.
