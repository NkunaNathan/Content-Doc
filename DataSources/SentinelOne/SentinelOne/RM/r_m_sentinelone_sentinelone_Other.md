Vendor: SentinelOne
===================
### Product: [SentinelOne](../ds_sentinelone_sentinelone.md)
### Use-Case: [Other](../../../../UseCases/uc_other.md)

| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|  119  |   6    |     0      |     14      |   14    |

| Event Type                    | Rules | Models                                                                                                                                                                                                                                         |
| ----------------------------- | ----- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| file-alert                    |       |  • <b>A-EPA-UP-TEMP</b>: Processes executed from TEMP directories on this asset                                                                                                                                                                |
| file-write                    |       |  • <b>A-FW-ProcessName-FileName</b>: File creations for process<br> • <b>A-EPA-UP-TEMP</b>: Processes executed from TEMP directories on this asset                                                                                             |
| network-alert                 |       |  • <b>A-EPA-UP-TEMP</b>: Processes executed from TEMP directories on this asset                                                                                                                                                                |
| network-connection-failed     |       |  • <b>A-NET-OdPort-Outbound</b>: Outbound destination ports per organization<br> • <b>A-NET-HdPort-Outbound</b>: Outbound destination ports per asset                                                                                          |
| network-connection-successful |       |  • <b>A-NET-OdPort-Outbound</b>: Outbound destination ports per organization<br> • <b>A-NET-HdPort-Outbound</b>: Outbound destination ports per asset                                                                                          |
| process-created               |       |  • <b>A-PC-Process-Hash</b>: Hashes used to create processes on the asset.<br> • <b>A-PC-ParentName-ProcessName</b>: Processes for parent parent processes.<br> • <b>A-EPA-UP-TEMP</b>: Processes executed from TEMP directories on this asset |
| security-alert                |       |  • <b>A-EPA-UP-TEMP</b>: Processes executed from TEMP directories on this asset                                                                                                                                                                |
| task-created                  |       |  • <b>A-EPA-UP-TEMP</b>: Processes executed from TEMP directories on this asset                                                                                                                                                                |