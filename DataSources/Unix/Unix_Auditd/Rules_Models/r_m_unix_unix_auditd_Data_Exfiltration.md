Vendor: Unix
============
### Product: [Unix Auditd](../ds_unix_unix_auditd.md)
### Use-Case: [Data Exfiltration](../../../../UseCases/uc_data_exfiltration.md)

| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|   9   |   3    |     4      |     16      |   16    |

| Event Type      | Rules                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | Models                                                                                                                                                                   |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| file-read       | <b>T1083 - File and Directory Discovery</b><br> ↳ <b>FA-FG-F</b>: First access to folder for group<br> ↳ <b>FA-OG-A</b>: Abnormal access to source code files for user in the peer group<br> ↳ <b>FA-SFU-F</b>: First access to folder containing source code by user                                                                                                                                                                                                                                                                                                                                                                                                              |  • <b>FA-SFU</b>: Source code folder access by users<br> • <b>FA-OG</b>: Users accessing source code files in the peer group<br> • <b>FA-FG</b>: Folder access by groups |
| file-write      | <b>T1083 - File and Directory Discovery</b><br> ↳ <b>FA-FG-F</b>: First access to folder for group<br> ↳ <b>FA-OG-A</b>: Abnormal access to source code files for user in the peer group<br> ↳ <b>FA-SFU-F</b>: First access to folder containing source code by user                                                                                                                                                                                                                                                                                                                                                                                                              |  • <b>FA-SFU</b>: Source code folder access by users<br> • <b>FA-OG</b>: Users accessing source code files in the peer group<br> • <b>FA-FG</b>: Folder access by groups |
| process-created | <b>T1020 - Automated Exfiltration</b><br> ↳ <b>Exfil-Tunnel-Tools-Exec</b>: Tools known for data exfiltration and tunneling were executed.<br> ↳ <b>Exfil-Tunneling-Tools-Exec</b>: Well-known exfiltration and tunneling tools were executed.<br><br><b>T1048 - Exfiltration Over Alternative Protocol</b><br> ↳ <b>A-Tap-Installer</b>: TAP software was installed on this asset.<br> ↳ <b>DNS-Exfiltration-Tools-Exec</b>: Well-known DNS Exfiltration tools were executed.<br> ↳ <b>Tap-Installer</b>: TAP software was installed.<br><br><b>T1175 - T1175</b><br> ↳ <b>MMC-Spawn-Win-Shell</b>: MMC (Microsoft Management Console) started a Windows command line executable. |                                                                                                                                                                          |