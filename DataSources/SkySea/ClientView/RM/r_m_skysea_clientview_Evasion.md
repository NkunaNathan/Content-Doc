Vendor: SkySea
==============
### Product: [ClientView](../ds_skysea_clientview.md)
### Use-Case: [Evasion](../../../../UseCases/uc_evasion.md)

| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|  71   |   3    |     33     |     15      |   15    |

| Event Type      | Rules    | Models    |
| ---- | ---- | ---- |
| process-created | <b>T1059 - Command and Scripting Interperter</b><br> ↳ <b>A-TasksFolder-Evasion</b>: The 'tasks' directory was observed in a file creation command on this asset<br> ↳ <b>A-ETW-Trace-Disable</b>: Event tracing has been disabled, possible logging evasion on this asset<br> ↳ <b>A-RASdial-Activity</b>: Process was executed on this asset with rasdial as a command line argument.<br> ↳ <b>TasksFolder-Evasion</b>: The 'tasks' directory was observed in a file creation command<br> ↳ <b>ETW-Trace-Disable</b>: Event tracing has been disabled, possible logging evasion<br> ↳ <b>RASdial-Activity</b>: Process was executed with rasdial as a command line argument.<br><br><b>T1218.008 - T1218.008</b><br> ↳ <b>A-Odbcconf-DLL-Load</b>: DLL loaded on this asset via odbcconf.exe execution.<br> ↳ <b>Odbcconf-DLL-Load</b>: DLL loaded via odbcconf.exe execution.<br><br><b>T1218.010 - Signed Binary Proxy Execution: Regsvr32</b><br> ↳ <b>Odbcconf-DLL-Load</b>: DLL loaded via odbcconf.exe execution.<br><br><b>T1218.011 - Signed Binary Proxy Execution: Rundll32</b><br> ↳ <b>A-EPA-Rundll-FTP-F</b>: First rundll activity for FTP firewall port blocking/unblocking on the asset.<br> ↳ <b>A-EPA-Rundll-FTP-A</b>: Abnormal rundll activity for FTP firewall port blocking/unblocking<br> ↳ <b>Odbcconf-DLL-Load</b>: DLL loaded via odbcconf.exe execution.<br><br><b>T1218 - Signed Binary Proxy Execution</b><br> ↳ <b>A-Applocker-Bypass</b>: Execution of executables that can be used to bypass Applocker on this asset<br> ↳ <b>A-Bginfo-App-Whitelisting</b>: VBscript referenced in a .bgi file was executed on this asset.<br> ↳ <b>A-DNX-App-Whitelisting</b>: C# code located in consoleapp folder was executed on this asset.<br> ↳ <b>A-Dxcap-Possible-Subprocess</b>: Dxcap.exe was executed on this asset.<br> ↳ <b>Applocker-Bypass</b>: Execution of executables that can be used to bypass Applocker<br> ↳ <b>Bginfo-App-Whitelisting</b>: VBscript referenced in a .bgi file was executed.<br> ↳ <b>DNX-App-Whitelisting</b>: C# code located in consoleapp folder was executed.<br> ↳ <b>Dxcap-Possible-Subprocess</b>: Dxcap.exe was executed.<br><br><b>T1027.004 - Obfuscated Files or Information: Compile After Delivery</b><br> ↳ <b>A-DNX-App-Whitelisting</b>: C# code located in consoleapp folder was executed on this asset.<br> ↳ <b>DNX-App-Whitelisting</b>: C# code located in consoleapp folder was executed.<br><br><b>T1027 - Obfuscated Files or Information</b><br> ↳ <b>A-Ping-Hex-IP</b>: A ping command used a hex decoded IP address on this asset.<br> ↳ <b>A-Certutil-Encode</b>: Certutil commands to encode files were used on this asset.<br> ↳ <b>EXPERT-POWERSHELL-ENCRYPTED</b>: Encrypted argument in a Powershell command detected<br> ↳ <b>Ping-Hex-IP</b>: A ping command used a hex decoded IP address<br> ↳ <b>Sus-Encoded-PS-CmdLine</b>: Suspicious Powershell process was started with base64 encoded commands.<br> ↳ <b>Base64-Powershell-CmdLine-Keywords</b>: Base64 encoded strings were found in hidden malicious Powershell command lines<br> ↳ <b>Certutil-Encode</b>: Certutil commands to encode files were used.<br><br><b>T1059.005 - T1059.005</b><br> ↳ <b>A-Bginfo-App-Whitelisting</b>: VBscript referenced in a .bgi file was executed on this asset.<br> ↳ <b>Bginfo-App-Whitelisting</b>: VBscript referenced in a .bgi file was executed.<br><br><b>T1070 - Indicator Removal on Host</b><br> ↳ <b>A-ETW-Trace-Disable</b>: Event tracing has been disabled, possible logging evasion on this asset<br> ↳ <b>A-Unauthorized-MBR-Mods</b>: Bcdedit.exe has signs of malicious unauthorized usage on this asset.<br> ↳ <b>ETW-Trace-Disable</b>: Event tracing has been disabled, possible logging evasion<br> ↳ <b>Unauthorized-MBR-Mods</b>: Bcdedit.exe has signs of malicious unauthorized usage.<br><br><b>T1542.003 - T1542.003</b><br> ↳ <b>A-Unauthorized-MBR-Mods</b>: Bcdedit.exe has signs of malicious unauthorized usage on this asset.<br> ↳ <b>Unauthorized-MBR-Mods</b>: Bcdedit.exe has signs of malicious unauthorized usage.<br><br><b>T1197 - BITS Jobs</b><br> ↳ <b>A-BITS-Suspicious-Service</b>: First abnormal BITS job created on the asset.<br> ↳ <b>BITS-Suspicious-Service</b>: First abnormal BITS jobs created on the endpoint<br><br><b>T1562.006 - T1562.006</b><br> ↳ <b>A-ETW-Trace-Disable</b>: Event tracing has been disabled, possible logging evasion on this asset<br> ↳ <b>ETW-Trace-Disable</b>: Event tracing has been disabled, possible logging evasion<br> ↳ <b>Sysmon-Driver-Unload</b>: Possible Sysmon driver unloaded.<br><br><b>T1562.004 - Impair Defenses: Disable or Modify System Firewall</b><br> ↳ <b>A-Firewall-Disabled-Netsh</b>: Windows firewall was turned off using netsh commands on this asset.<br> ↳ <b>A-Netsh-Connections-Win-Firewall</b>: Netsh commands were used to allow incoming connections by Port or Application on Windows Firewall on this asset.<br> ↳ <b>A-EPA-Rundll-FTP-F</b>: First rundll activity for FTP firewall port blocking/unblocking on the asset.<br> ↳ <b>A-EPA-Rundll-FTP-A</b>: Abnormal rundll activity for FTP firewall port blocking/unblocking<br> ↳ <b>Firewall-Disabled-Netsh</b>: Windows firewall was turned off using netsh commands.<br> ↳ <b>Netsh-Connections-Win-Firewall</b>: Netsh commands were used to allow incoming connections by Port or Application on Windows Firewall.<br><br><b>T1036 - Masquerading</b><br> ↳ <b>A-Winword-Uncommon-Process</b>: 'MicroScMgmt' executable run by 'WinWord.exe' on this asset<br> ↳ <b>A-Taskmgr-Local-System</b>: A taskmgr.exe process was executed in the context of LOCAL_SYSTEM<br> ↳ <b>A-Sys-File-Exec-Anomaly</b>: A Windows program executable was started in a suspicious folder on this asset.<br> ↳ <b>A-Taskmgr-as-Parent</b>: A process was created from Windows task manager on this asset.<br> ↳ <b>Winword-Uncommon-Process</b>: 'MicroScMgmt' executable run by 'WinWord.exe'<br> ↳ <b>Sys-File-Exec-Anomaly</b>: A Windows program executable was started in a suspicious folder.<br> ↳ <b>Taskmgr-as-Parent</b>: A process was created from Windows task manager.<br> ↳ <b>Sus-Double-Extension</b>: An .exe extension was used after a different non-executable file extension.<br><br><b>T1059.001 - Command and Scripting Interperter: PowerShell</b><br> ↳ <b>A-Base64-CommandLine</b>: Base64 string in command line execution on this asset<br> ↳ <b>A-Powershell-AMSI-Bypass-NET</b>: Request to amsiInitFailed that can be used to disable AMSI Scanning was found on this asset.<br> ↳ <b>A-Sus-Powershell-Param</b>: Powershell was invoked with a suspicious parameter substring on this asset.<br> ↳ <b>EXPERT-POWERSHELL-ENCRYPTED</b>: Encrypted argument in a Powershell command detected<br> ↳ <b>Base64-CommandLine</b>: Base64 string in command line<br> ↳ <b>Powershell-AMSI-Bypass-NET</b>: Request to amsiInitFailed that can be used to disable AMSI Scanning was found.<br> ↳ <b>Sus-Powershell-Param</b>: Powershell was invoked with a suspicious parameter substring<br> ↳ <b>Sus-Encoded-PS-CmdLine</b>: Suspicious Powershell process was started with base64 encoded commands.<br> ↳ <b>Base64-Powershell-CmdLine-Keywords</b>: Base64 encoded strings were found in hidden malicious Powershell command lines<br><br><b>T1562.001 - T1562.001</b><br> ↳ <b>A-Powershell-AMSI-Bypass-NET</b>: Request to amsiInitFailed that can be used to disable AMSI Scanning was found on this asset.<br> ↳ <b>Powershell-AMSI-Bypass-NET</b>: Request to amsiInitFailed that can be used to disable AMSI Scanning was found.<br><br><b>T1574 - Hijack Execution Flow</b><br> ↳ <b>A-TasksFolder-Evasion</b>: The 'tasks' directory was observed in a file creation command on this asset<br> ↳ <b>TasksFolder-Evasion</b>: The 'tasks' directory was observed in a file creation command<br><br><b>T1036.005 - Masquerading: Match Legitimate Name or Location</b><br> ↳ <b>A-Sus-MsiExec-Directory</b>: Suspicious msiexec process started in an uncommon directory on this asset.<br> ↳ <b>A-Sus-Svchost-Process</b>: A suspicious svchost process was started on this asset.<br> ↳ <b>A-Win-Proc-Sus-Parent</b>: A suspicious parent process of well-known Windows processes was detected on this asset.<br> ↳ <b>Sus-MsiExec-Directory</b>: Suspicious msiexec process started in an uncommon directory.<br> ↳ <b>Sus-Svchost-Process</b>: A suspicious svchost process was started.<br> ↳ <b>Win-Proc-Sus-Parent</b>: A suspicious parent process of well-known Windows processes was detected.<br><br><b>T1127.001 - Trusted Developer Utilities Proxy Execution: MSBuild</b><br> ↳ <b>A-Applocker-Bypass</b>: Execution of executables that can be used to bypass Applocker on this asset<br> ↳ <b>Applocker-Bypass</b>: Execution of executables that can be used to bypass Applocker<br><br><b>T1218.004 - Signed Binary Proxy Execution: InstallUtil</b><br> ↳ <b>A-Applocker-Bypass</b>: Execution of executables that can be used to bypass Applocker on this asset<br> ↳ <b>Applocker-Bypass</b>: Execution of executables that can be used to bypass Applocker<br><br><b>T1218.009 - Signed Binary Proxy Execution: Regsvcs/Regasm</b><br> ↳ <b>A-Applocker-Bypass</b>: Execution of executables that can be used to bypass Applocker on this asset<br> ↳ <b>Applocker-Bypass</b>: Execution of executables that can be used to bypass Applocker<br><br><b>T1202 - Indirect Command Execution</b><br> ↳ <b>A-Indirect-Cmd-Exec</b>: An indirect command was executed via Program Compatibility Assistant pcalua.exe or forfiles.exe on this asset.<br> ↳ <b>Indirect-Cmd-Exec</b>: An indirect command was executed via Program Compatibility Assistant pcalua.exe or forfiles.exe.<br><br><b>T1140 - Deobfuscate/Decode Files or Information</b><br> ↳ <b>A-Base64-CommandLine</b>: Base64 string in command line execution on this asset<br> ↳ <b>A-CertUtil-Suspicious-Usage</b>: The 'certutil' Windows utility was used with known suspicious command line flags on this asset<br> ↳ <b>Base64-CommandLine</b>: Base64 string in command line<br> ↳ <b>CertUtil-Suspicious-Usage</b>: The 'certutil' Windows utility was used with known suspicious command line flags<br> ↳ <b>Ping-Hex-IP</b>: A ping command used a hex decoded IP address<br><br><b>T1070.001 - Indicator Removal on Host: Clear Windows Event Logs</b><br> ↳ <b>A-EventLog-Tamper</b>: EventLog has been tampered with on this asset<br> ↳ <b>EventLog-Tamper</b>: EventLog has been tampered with<br><br><b>T1105 - Ingress Tool Transfer</b><br> ↳ <b>A-CertUtil-Suspicious-Usage</b>: The 'certutil' Windows utility was used with known suspicious command line flags on this asset<br> ↳ <b>CertUtil-Suspicious-Usage</b>: The 'certutil' Windows utility was used with known suspicious command line flags<br><br><b>T1564.004 - Hide Artifacts: NTFS File Attributes</b><br> ↳ <b>A-Powershell-ADS</b>: Powershell invoked using 'Alternate Data Stream' on this asset<br> ↳ <b>Powershell-ADS</b>: Powershell invoked using 'Alternate Data Stream'<br><br><b>T1036.003 - Masquerading: Rename System Utilities</b><br> ↳ <b>A-PSExec-Rename</b>: PS Exec used on this asset<br> ↳ <b>PSExec-Rename</b>: PS Exec used<br><br><b>T1203 - Exploitation for Client Execution</b><br> ↳ <b>A-EquationEditor-Droppers</b>: Possible 'Eqnetd32.exe' exploit usage on this asset<br> ↳ <b>EquationEditor-Droppers</b>: Possible 'Eqnetd32.exe' exploit usage<br><br><b>T1484.001 - T1484.001</b><br> ↳ <b>OG-SYSVOL-F</b>: Suspicious SYSVOL Domain Group Policy Access for the first time for this peer group<br> ↳ <b>OG-SYSVOL-A</b>: Abnormal SYSVOL Domain Group Policy Access for thjis peer group<br><br><b>T1552.006 - T1552.006</b><br> ↳ <b>OG-SYSVOL-F</b>: Suspicious SYSVOL Domain Group Policy Access for the first time for this peer group<br> ↳ <b>OG-SYSVOL-A</b>: Abnormal SYSVOL Domain Group Policy Access for thjis peer group<br><br><b>T1543.003 - Create or Modify System Process: Windows Service</b><br> ↳ <b>EPA-RANDOM-SERVICE</b>: Random service name for the user<br><br><b>T1218.002 - Signed Binary Proxy Execution: Control Panel</b><br> ↳ <b>EPA-CtrlPnl-A</b>: First control panel function usage for peer group<br><br><b>T1562 - Impair Defenses</b><br> ↳ <b>A-Sysmon-Driver-Unload</b>: Possible Sysmon driver unloaded on this asset. |  • <b>EPA-OG-SYSVOL</b>: SYSVOL domain group policy access by group in the organization<br> • <b>EPA-CntrlPnl</b>: Control Panel actions for peer group<br> • <b>A-EPA-Rundll-FTP</b>: Rundll actions for FTP port blocking/unblocking on the asset |