Vendor: Amazon
==============
### Product: [AWS GuardDuty](../ds_amazon_aws_guardduty.md)
### Use-Case: [Privilege Abuse](../../../../UseCases/uc_privilege_abuse.md)

| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|  14   |   9    |     6      |      1      |    1    |

| Event Type      | Rules                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | Models                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| process-created | <b>T1047 - Windows Management Instrumentation</b><br> ↳ <b>WMIC-EXE-RENAME-ORG-F</b>: First time WMIC.exe has been used to rename a user account by this user.<br> ↳ <b>EXE-RENAME-GRP-ORG-F</b>: First time WMIC.exe has been used to rename a group by this user.<br> ↳ <b>WMIC-EXE-RENAME-ORG-A</b>: Abnormal usage of WMIC.exe to rename a group by this user.<br><br><b>T1098 - Account Manipulation</b><br> ↳ <b>EXE-ADD-GRP-ORG-F</b>: First time net.exe has been used to create/add to a group by this user.<br> ↳ <b>EXE-ADD-GRP-ORG-A</b>: Abnormal usage of net.exe to create/add to a group by this user.<br> ↳ <b>NET-EXE-ACTIVE-ORG-F</b>: First time net.exe has been used to disable/enable a user account by this user.<br> ↳ <b>NET-EXE-ACTIVE-ORG-A</b>: Abnormal usage of net.exe to disable/enable a user account by this user.<br> ↳ <b>NET-EXE-DELETE-ORG-F</b>: First time net.exe has been used to delete a user account by this user.<br> ↳ <b>NET-EXE-DELETE-ORG-A</b>: Abnormal usage of net.exe to delete a user account by this user.<br> ↳ <b>WMIC-EXE-RENAME-ORG-F</b>: First time WMIC.exe has been used to rename a user account by this user.<br> ↳ <b>EXE-RENAME-GRP-ORG-F</b>: First time WMIC.exe has been used to rename a group by this user.<br> ↳ <b>WMIC-EXE-RENAME-ORG-A</b>: Abnormal usage of WMIC.exe to rename a group by this user.<br><br><b>T1531 - Account Access Removal</b><br> ↳ <b>NET-EXE-DELETE-ORG-F</b>: First time net.exe has been used to delete a user account by this user.<br> ↳ <b>NET-EXE-DELETE-ORG-A</b>: Abnormal usage of net.exe to delete a user account by this user.<br><br><b>T1078 - Valid Accounts</b><br> ↳ <b>EXE-ADD-GRP-ORG-F</b>: First time net.exe has been used to create/add to a group by this user.<br> ↳ <b>EXE-ADD-GRP-ORG-A</b>: Abnormal usage of net.exe to create/add to a group by this user.<br> ↳ <b>NET-EXE-ACTIVE-ORG-F</b>: First time net.exe has been used to disable/enable a user account by this user.<br> ↳ <b>NET-EXE-ACTIVE-ORG-A</b>: Abnormal usage of net.exe to disable/enable a user account by this user.<br><br><b>T1136 - Create Account</b><br> ↳ <b>EXE-ADD-GRP-ORG-F</b>: First time net.exe has been used to create/add to a group by this user.<br> ↳ <b>EXE-ADD-GRP-ORG-A</b>: Abnormal usage of net.exe to create/add to a group by this user.<br><br><b>T1136.001 - Create Account: Create: Local Account</b><br> ↳ <b>AC-OZ-CLI-F</b>: First zone on which account was created using CLI command<br> ↳ <b>AC-OH-CLI-F</b>: First host on which account was created using CLI command<br> ↳ <b>AC-OU-CLI-F</b>: First user on which account was created using CLI command<br> ↳ <b>NET-EXE-ADD-ORG-F</b>: First time net.exe has been used to create a user account by this user.<br> ↳ <b>NET-EXE-ADD-ORG-A</b>: Abnormal usage of net.exe to create a user account by this user. |  • <b>WMIC-EXE-RENAME-GRP-ORG</b>: Using WMIC.exe to rename a group<br> • <b>WMIC-EXE-RENAME-ORG</b>: Using WMIC.exe to rename a user account<br> • <b>NET-EXE-DELETE-ORG</b>: Using net.exe to delete a user account<br> • <b>NET-EXE-ACTIVE-ORG</b>: Using net.exe to disable/enable a user account<br> • <b>NET-EXE-ADD-GRP-ORG</b>: Using net.exe to add a group account<br> • <b>NET-EXE-ADD-ORG</b>: Using net.exe to add a user account<br> • <b>AC-OU-CLI</b>: Users on which account was created using CLI command<br> • <b>AC-OH-CLI</b>: Hosts on which account was created using CLI command<br> • <b>AC-OZ-CLI</b>: Zones on which account was created using CLI command |