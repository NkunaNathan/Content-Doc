Vendor: Zeek
============
### Product: [Zeek Network Security Monitor](../ds_zeek_zeek_network_security_monitor.md)
### Use-Case: [Other](../../../../UseCases/uc_other.md)

| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|  39   |   7    |     0      |     24      |   24    |

| Event Type                    | Rules | Models                                                                                                                                                                                                                                                                            |
| ----------------------------- | ----- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| file-write                    |       |  • <b>A-FW-ProcessName-FileName</b>: File creations for process<br> • <b>A-EPA-UP-TEMP</b>: Processes executed from TEMP directories on this asset                                                                                                                                |
| kerberos-logon                |       |  • <b>A-KL-UToE</b>: Ticket options and encryption type combination for asset<br> • <b>A-AL-DhU</b>: Users per Host                                                                                                                                                               |
| network-alert                 |       |  • <b>A-EPA-UP-TEMP</b>: Processes executed from TEMP directories on this asset                                                                                                                                                                                                   |
| network-connection-failed     |       |  • <b>A-NET-OdPort-Outbound</b>: Outbound destination ports per organization<br> • <b>A-NET-HdPort-Outbound</b>: Outbound destination ports per asset                                                                                                                             |
| network-connection-successful |       |  • <b>A-NET-OdPort-Outbound</b>: Outbound destination ports per organization<br> • <b>A-NET-HdPort-Outbound</b>: Outbound destination ports per asset                                                                                                                             |
| ntlm-logon                    |       |  • <b>A-AL-DhU</b>: Users per Host                                                                                                                                                                                                                                                |
| remote-access                 |       |  • <b>A-EPA-UP-TEMP</b>: Processes executed from TEMP directories on this asset<br> • <b>A-KL-UToE</b>: Ticket options and encryption type combination for asset<br> • <b>A-AE-NTLM</b>: Models the NTLM hostnames seen in the organization                                       |
| remote-logon                  |       |  • <b>A-EPA-UP-TEMP</b>: Processes executed from TEMP directories on this asset<br> • <b>A-KL-UToE</b>: Ticket options and encryption type combination for asset<br> • <b>A-AE-NTLM</b>: Models the NTLM hostnames seen in the organization<br> • <b>A-AL-DhU</b>: Users per Host |