Vendor: Juniper Networks
========================
Product: Juniper Networks Pulse Secure
--------------------------------------
|                                 Use-Case                                  | Activity Types                                                                                                                                                                                                                                                | Event Types/Parsers                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       | MITRE TTP                                                                                                                                                               | Content                    |
|:-------------------------------------------------------------------------:| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------- |
| [Compromised Credentials](../UseCases/usecase_compromised_credentials.md) | - Account Creation and Management<br>- Activity Time  and Type<br>- Application Activity<br>- Asset Logon and Access<br>- Critical System Activity<br>- Email Activity<br>- Network zones and Location Access<br>- Service Account Activity<br>- VPN Activity |  account-deleted<br> -- [s-pulsesecure-account-deleted](../Parsers/parserContent_s-pulsesecure-account-deleted.md)<br><br> app-activity<br> -- [s-juniper-pulse-activity](../Parsers/parserContent_s-juniper-pulse-activity.md)<br> -- [cef-juniper-pulse-activity](../Parsers/parserContent_cef-juniper-pulse-activity.md)<br><br> vpn-login<br> -- [pulsesecure-vpn-login](../Parsers/parserContent_pulsesecure-vpn-login.md)<br> -- [s-pulsesecure-vpn-login](../Parsers/parserContent_s-pulsesecure-vpn-login.md)<br> | T1078 - Valid Accounts<br>T1098 - Account Manipulation<br>T1098.002 - Account Manipulation: Exchange Email Delegate Permissions<br>T1133 - External Remote Services<br> |  - 41 Rules<br> - 5 Models |
|       [Data Exfiltration](../UseCases/usecase_data_exfiltration.md)       | - Email Activity                                                                                                                                                                                                                                              |  account-deleted<br> -- [s-pulsesecure-account-deleted](../Parsers/parserContent_s-pulsesecure-account-deleted.md)<br><br> app-activity<br> -- [s-juniper-pulse-activity](../Parsers/parserContent_s-juniper-pulse-activity.md)<br> -- [cef-juniper-pulse-activity](../Parsers/parserContent_cef-juniper-pulse-activity.md)<br><br> vpn-login<br> -- [pulsesecure-vpn-login](../Parsers/parserContent_pulsesecure-vpn-login.md)<br> -- [s-pulsesecure-vpn-login](../Parsers/parserContent_s-pulsesecure-vpn-login.md)<br> | T1098.002 - Account Manipulation: Exchange Email Delegate Permissions<br>T1114.003 - Email Collection: Email Forwarding Rule<br>                                        |  - 3 Rules<br>             |
|          [Internal Fraud](../UseCases/usecase_internal_fraud.md)          | - Application Activity                                                                                                                                                                                                                                        |  account-deleted<br> -- [s-pulsesecure-account-deleted](../Parsers/parserContent_s-pulsesecure-account-deleted.md)<br><br> app-activity<br> -- [s-juniper-pulse-activity](../Parsers/parserContent_s-juniper-pulse-activity.md)<br> -- [cef-juniper-pulse-activity](../Parsers/parserContent_cef-juniper-pulse-activity.md)<br><br> vpn-login<br> -- [pulsesecure-vpn-login](../Parsers/parserContent_pulsesecure-vpn-login.md)<br> -- [s-pulsesecure-vpn-login](../Parsers/parserContent_s-pulsesecure-vpn-login.md)<br> | T1078 - Valid Accounts<br>                                                                                                                                              |  - 13 Rules<br> - 1 Models |
|        [Lateral Movement](../UseCases/usecase_lateral_movement.md)        | - Activity Time  and Type<br>- Application Activity<br>- Network zones and Location Access                                                                                                                                                                    |  account-deleted<br> -- [s-pulsesecure-account-deleted](../Parsers/parserContent_s-pulsesecure-account-deleted.md)<br><br> app-activity<br> -- [s-juniper-pulse-activity](../Parsers/parserContent_s-juniper-pulse-activity.md)<br> -- [cef-juniper-pulse-activity](../Parsers/parserContent_cef-juniper-pulse-activity.md)<br><br> vpn-login<br> -- [pulsesecure-vpn-login](../Parsers/parserContent_pulsesecure-vpn-login.md)<br> -- [s-pulsesecure-vpn-login](../Parsers/parserContent_s-pulsesecure-vpn-login.md)<br> | T1078 - Valid Accounts<br>T1133 - External Remote Services<br>                                                                                                          |  - 6 Rules<br> - 1 Models  |
|       [Malware Detection](../UseCases/usecase_malware_detection.md)       | - Asset Logon and Access                                                                                                                                                                                                                                      |  account-deleted<br> -- [s-pulsesecure-account-deleted](../Parsers/parserContent_s-pulsesecure-account-deleted.md)<br><br> app-activity<br> -- [s-juniper-pulse-activity](../Parsers/parserContent_s-juniper-pulse-activity.md)<br> -- [cef-juniper-pulse-activity](../Parsers/parserContent_cef-juniper-pulse-activity.md)<br><br> vpn-login<br> -- [pulsesecure-vpn-login](../Parsers/parserContent_pulsesecure-vpn-login.md)<br> -- [s-pulsesecure-vpn-login](../Parsers/parserContent_s-pulsesecure-vpn-login.md)<br> | T1078 - Valid Accounts<br>T1090.003 - Proxy: Multi-hop Proxy<br>                                                                                                        |  - 3 Rules<br>             |
|     [Privileged Activity](../UseCases/usecase_privileged_activity.md)     | - Account Creation and Management<br>- Application Activity<br>- Email Activity<br>- Service Account Activity                                                                                                                                                 |  account-deleted<br> -- [s-pulsesecure-account-deleted](../Parsers/parserContent_s-pulsesecure-account-deleted.md)<br><br> app-activity<br> -- [s-juniper-pulse-activity](../Parsers/parserContent_s-juniper-pulse-activity.md)<br> -- [cef-juniper-pulse-activity](../Parsers/parserContent_cef-juniper-pulse-activity.md)<br><br> vpn-login<br> -- [pulsesecure-vpn-login](../Parsers/parserContent_pulsesecure-vpn-login.md)<br> -- [s-pulsesecure-vpn-login](../Parsers/parserContent_s-pulsesecure-vpn-login.md)<br> | T1078 - Valid Accounts<br>T1098 - Account Manipulation<br>T1098.002 - Account Manipulation: Exchange Email Delegate Permissions<br>                                     |  - 6 Rules<br> - 1 Models  |
|    [Ransomware Detection](../UseCases/usecase_ransomware_detection.md)    | - Asset Logon and Access                                                                                                                                                                                                                                      |  account-deleted<br> -- [s-pulsesecure-account-deleted](../Parsers/parserContent_s-pulsesecure-account-deleted.md)<br><br> app-activity<br> -- [s-juniper-pulse-activity](../Parsers/parserContent_s-juniper-pulse-activity.md)<br> -- [cef-juniper-pulse-activity](../Parsers/parserContent_cef-juniper-pulse-activity.md)<br><br> vpn-login<br> -- [pulsesecure-vpn-login](../Parsers/parserContent_pulsesecure-vpn-login.md)<br> -- [s-pulsesecure-vpn-login](../Parsers/parserContent_s-pulsesecure-vpn-login.md)<br> | T1078 - Valid Accounts<br>T1090.003 - Proxy: Multi-hop Proxy<br>                                                                                                        |  - 3 Rules<br>             |

ATT&CK Matrix for Enterprise
----------------------------
| Initial Access                                                                                                                                   | Execution | Persistence                                                                                                                                                                                                                                                                                                                                 | Privilage escalation                                                | Defense evasion                                                     | Credential Access | Discovery | Lateral Movement | Collection                                                                                                                                                            | Command and Control                                                                                                                       | Exfiltration | Impact |
| ------------------------------------------------------------------------------------------------------------------------------------------------ | --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ----------------- | --------- | ---------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ------------ | ------ |
| [External Remote Services](https://attack.mitre.org/techniques/T1133)<br><br>[Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> |           | [External Remote Services](https://attack.mitre.org/techniques/T1133)<br><br>[Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br>[Account Manipulation](https://attack.mitre.org/techniques/T1098)<br><br>[Account Manipulation: Exchange Email Delegate Permissions](https://attack.mitre.org/techniques/T1098/002)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> |                   |           |                  | [Email Collection](https://attack.mitre.org/techniques/T1114)<br><br>[Email Collection: Email Forwarding Rule](https://attack.mitre.org/techniques/T1114/003)<br><br> | [Proxy: Multi-hop Proxy](https://attack.mitre.org/techniques/T1090/003)<br><br>[Proxy](https://attack.mitre.org/techniques/T1090)<br><br> |              |        |