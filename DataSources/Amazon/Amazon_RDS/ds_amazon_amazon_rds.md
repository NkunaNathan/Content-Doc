Vendor: Amazon
==============
Product: Amazon RDS
-------------------
| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|  18   |   10   |     1      |      3      |    3    |

|    Use-Case    | Event Types/Parsers    | MITRE TTP    | Content    |
|:----:| ---- | ---- | ---- |
| [Compromised Credentials](../../../UseCases/uc_compromised_credentials.md) |  database-login<br> ↳[amazon-rds-database-login](Ps/pC_amazonrdsdatabaselogin.md)<br><br> database-query<br> ↳[amazon-rds-database-operation-1](Ps/pC_amazonrdsdatabaseoperation1.md)<br> ↳[amazon-rds-database-operation](Ps/pC_amazonrdsdatabaseoperation.md)<br><br> database-update<br> ↳[amazon-rds-database-operation-1](Ps/pC_amazonrdsdatabaseoperation1.md)<br> ↳[amazon-rds-database-operation](Ps/pC_amazonrdsdatabaseoperation.md)<br> | T1213 - Data from Information Repositories<br> | [<ul><li>18 Rules</li></ul><ul><li>10 Models</li></ul>](RM/r_m_amazon_amazon_rds_Compromised_Credentials.md) |
|    [Data Access](../../../UseCases/uc_data_access.md)    |  database-login<br> ↳[amazon-rds-database-login](Ps/pC_amazonrdsdatabaselogin.md)<br><br> database-query<br> ↳[amazon-rds-database-operation-1](Ps/pC_amazonrdsdatabaseoperation1.md)<br> ↳[amazon-rds-database-operation](Ps/pC_amazonrdsdatabaseoperation.md)<br><br> database-update<br> ↳[amazon-rds-database-operation-1](Ps/pC_amazonrdsdatabaseoperation1.md)<br> ↳[amazon-rds-database-operation](Ps/pC_amazonrdsdatabaseoperation.md)<br> | T1213 - Data from Information Repositories<br> | [<ul><li>18 Rules</li></ul><ul><li>10 Models</li></ul>](RM/r_m_amazon_amazon_rds_Data_Access.md)    |

ATT&CK Matrix for Enterprise
----------------------------
| Initial Access | Execution | Persistence | Privilege Escalation | Defense Evasion | Credential Access | Discovery | Lateral Movement | Collection                                                                              | Command and Control | Exfiltration | Impact |
| -------------- | --------- | ----------- | -------------------- | --------------- | ----------------- | --------- | ---------------- | --------------------------------------------------------------------------------------- | ------------------- | ------------ | ------ |
|                |           |             |                      |                 |                   |           |                  | [Data from Information Repositories](https://attack.mitre.org/techniques/T1213)<br><br> |                     |              |        |