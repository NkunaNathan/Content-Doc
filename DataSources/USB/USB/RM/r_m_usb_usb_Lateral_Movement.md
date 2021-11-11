Vendor: USB
===========
### Product: [USB](../ds_usb_usb.md)
### Use-Case: [Lateral Movement](../../../../UseCases/uc_lateral_movement.md)

| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|   4   |   2    |     1      |      1      |    1    |

| Event Type          | Rules                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        | Models                                                                                                                                |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| web-activity-denied | <b>T1071.001 - Application Layer Protocol: Web Protocols</b><br> ↳ <b>NETF-HCountry-Outbound-WEB-F</b>: First failed web browsing connection to this country from asset<br> ↳ <b>NETF-HCountry-Outbound-WEB-A</b>: Web browsing connection to abnormal country for asset has failed<br> ↳ <b>NETF-OCountry-Outbound-WEB-F</b>: First failed web browsing connection to this country from organization<br> ↳ <b>NETF-OCountry-Outbound-WEB-A</b>: Web browsing connection to abnormal country for the organization has failed |  • <b>A-NET-OCountry-Outbound</b>: Outbound country per organization<br> • <b>A-NET-HCountry-Outbound</b>: Outbound country per asset |