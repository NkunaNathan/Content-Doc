Vendor: GoAnywhere
==================
Product: GoAnywhere MFT
-----------------------
| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|   8   |   7    |     2      |      3      |    3    |

|                                  Use-Case                                  | Event Types/Parsers                                                                                                                                                                                                                                                                                                                                                                                                                                                                        | MITRE TTP                                                          | Content                                                                                                                      |
|:--------------------------------------------------------------------------:| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------- |
| [Compromised Credentials](../../../UseCases/uc_compromised_credentials.md) |  file-delete<br> ↳ [goanywhere-file-delete](Parsers/parserContent_goanywhere-file-delete.md)<br><br> file-download<br> ↳ [goanywhere-file-download](Parsers/parserContent_goanywhere-file-download.md)<br> ↳ [goanywhere-file-download-1](Parsers/parserContent_goanywhere-file-download-1.md)<br><br> file-upload<br> ↳ [goanywhere-file-upload-1](Parsers/parserContent_goanywhere-file-upload-1.md)<br> ↳ [goanywhere-file-upload](Parsers/parserContent_goanywhere-file-upload.md)<br> | T1083 - File and Directory Discovery<br>                           | [<ul><li>6 Rules</li></ul><ul><li>6 Models</li></ul>](Rules_Models/r_m_goanywhere_goanywhere_mft_Compromised_Credentials.md) |
|             [Data Access](../../../UseCases/uc_data_access.md)             |  file-delete<br> ↳ [goanywhere-file-delete](Parsers/parserContent_goanywhere-file-delete.md)<br><br> file-download<br> ↳ [goanywhere-file-download](Parsers/parserContent_goanywhere-file-download.md)<br> ↳ [goanywhere-file-download-1](Parsers/parserContent_goanywhere-file-download-1.md)<br><br> file-upload<br> ↳ [goanywhere-file-upload-1](Parsers/parserContent_goanywhere-file-upload-1.md)<br> ↳ [goanywhere-file-upload](Parsers/parserContent_goanywhere-file-upload.md)<br> | T1083 - File and Directory Discovery<br>                           | [<ul><li>6 Rules</li></ul><ul><li>6 Models</li></ul>](Rules_Models/r_m_goanywhere_goanywhere_mft_Data_Access.md)             |
|         [Privilege Abuse](../../../UseCases/uc_privilege_abuse.md)         |  file-delete<br> ↳ [goanywhere-file-delete](Parsers/parserContent_goanywhere-file-delete.md)<br><br> file-download<br> ↳ [goanywhere-file-download](Parsers/parserContent_goanywhere-file-download.md)<br> ↳ [goanywhere-file-download-1](Parsers/parserContent_goanywhere-file-download-1.md)<br><br> file-upload<br> ↳ [goanywhere-file-upload-1](Parsers/parserContent_goanywhere-file-upload-1.md)<br> ↳ [goanywhere-file-upload](Parsers/parserContent_goanywhere-file-upload.md)<br> | T1078 - Valid Accounts<br>T1083 - File and Directory Discovery<br> | [<ul><li>2 Rules</li></ul><ul><li>1 Models</li></ul>](Rules_Models/r_m_goanywhere_goanywhere_mft_Privilege_Abuse.md)         |
|     [Privileged Activity](../../../UseCases/uc_privileged_activity.md)     |  file-delete<br> ↳ [goanywhere-file-delete](Parsers/parserContent_goanywhere-file-delete.md)<br><br> file-download<br> ↳ [goanywhere-file-download](Parsers/parserContent_goanywhere-file-download.md)<br> ↳ [goanywhere-file-download-1](Parsers/parserContent_goanywhere-file-download-1.md)<br><br> file-upload<br> ↳ [goanywhere-file-upload-1](Parsers/parserContent_goanywhere-file-upload-1.md)<br> ↳ [goanywhere-file-upload](Parsers/parserContent_goanywhere-file-upload.md)<br> | T1078 - Valid Accounts<br>                                         | [<ul><li>1 Rules</li></ul>](Rules_Models/r_m_goanywhere_goanywhere_mft_Privileged_Activity.md)                               |

ATT&CK Matrix for Enterprise
----------------------------
| Initial Access                                                      | Execution | Persistence                                                         | Privilege Escalation                                                | Defense Evasion                                                     | Credential Access | Discovery                                                                         | Lateral Movement | Collection | Command and Control | Exfiltration | Impact |
| ------------------------------------------------------------------- | --------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ----------------- | --------------------------------------------------------------------------------- | ---------------- | ---------- | ------------------- | ------------ | ------ |
| [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> |           | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> |                   | [File and Directory Discovery](https://attack.mitre.org/techniques/T1083)<br><br> |                  |            |                     |              |        |