#### Parser Content
```Java
{
Name = cef-sentinelone-activity
 Product = SentinelOne
 Vendor = SentinelOne
 Lms = Direct
 TimeFormat = "epoch"
 DataType = "app-activity"
 Conditions = [ """CEF:""", """destinationServiceName=""", """SentinelOne""" ]
 Fields = [
   """exabeam_host=([^=]+@\s*)?({host}\S+)""",
   """CEF:\d+\|([^\|]+\|){4}({activity}[^\|]+)""",
   """destinationServiceName=({app}[^\s]+)""",
   """timestamp\s\{\\n\s*millisecondsSinceEpoch:\s({time}\d+)""",
   """commandLine:\s*"+\\*({command_line}[^"]+)""",
   """pid:\s*({pid}\d+)""",
   """user\s*\{\\n\s+name:\s+"*({domain}[^\\]+)\\+({user}[^\s"]+)""",
   """user\s*\{\\n.+?sid:\s+"+({user_sid}[^"]+)""",
   """msg=({additional_info}.+?)\s+\w+=""",
   """fname=({object}.+?)\s+\w+=""",
   """path:\s+"+({process}({directory}[^."]+)\\({process_name}[^"]+))""",
 ]
}
{
  Name = netscope-dlp-alert-activity
  Vendor = Netskope
  Product = Netskope Active Platform
  Lms = Direct
  DataType = "dlp-alert"
  TimeFormat = "yyyy-MM-dd'T'HH:mm:ss.SSSZ"
  Conditions = [ """SkyFormation Cloud Apps Security""","""destinationServiceName=Netskope""","""alert_type""","""DLP"""]
  Fields =[  
      """({time}\d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\d.\d+Z),""",
      """exabeam_host=([^=]+@\s*)?({host}[^\s]+)""",
      """"dstip"+:"+({dest_ip}[^"]+)"""",
      """"file_type"+:"+({file_type}[^"]+)"""",
      """"app"+:"+({app}[^"]+)"""",
      """"device"+:"+({device_type}[^"]+)"""",
      """"alert_type"+:"+({alert_type}[^"]+)"""",
      """"hostname"+:"+({host}[^"]+)"""",
      """"policy"+:"+({alert_name}[^"]+)"""",
      """"action"+:"+({action}[^"]+)"""",
      """"referer"+:"+({referrer}[^"]+)"""",
      """"user"+:"+({user}[^"]+)"""",
      """"srcip"+:"+({src_ip}[^"]+)"""",
      """"category"+:"+({category}[^"]+)""""
      """"+activity"+:"+({activity}[^"]+)"+""",
      """"object"+:"+({file_name}[^"]+)"""",
      """"+ccl"+:"+({alert_severity}[^"]+)"+""",
      """"+md5"+:"+({md5}[^"]+)"+""",
      """"+request_id"+:({alert_id}[^,]+)""",
      """proto=({protocol}[^"]+)\srequestClientApplication""",
      """outcome=({outcome}[^ ]+)""",
      """ext_url=({full_url}[^ ]+)"""
    ]
}
${WatchGuardSParserTemplates.watch-guard-events}{
  Name = watchguard-event-1
  DataType = "network-connection"
  Conditions = [ """msg_id=""", """3000-0148""", """firewall:""" ]
}
```