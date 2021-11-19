#### Parser Content
```Java
{
Name = cef-carbonblack-network-connection-successful-2
  DataType = "network-connection"
  Conditions = [ """CEF:""", """threatIndicators""" , """|security-threat-detected""", """act=connect""" ]
  Fields = ${CarbonBlackParserTemplates.cef-carbonblack-events-1.Fields} [
    """({outcome}successful)""",
  ]

cef-carbonblack-events-1 {
  Vendor = VMware
  Product = Carbon Black Cloud Endpoint Standard
  Lms = ArcSight
  TimeFormat = "epoch"
  Fields = [
    """exabeam_host=([^=]{1,2000}@\s{0,100})?({host}[\w\-.]{1,2000})""",
    """eventTime=({time}\d{1,100})""",
    """deviceIpAddress=({src_ip}[A-Fa-f:\d.]{1,2000})""",
    """src=({src_ip}[A-Fa-f:\d.]{1,2000})""",
    """deviceName =(({domain}[^\\\s"]{1,2000})\\+)?({src_host}[^\\\s"]{1,2000})"?""",
    """email=(({domain}[^\\\s"]{1,2000})\\+)?(HiveStreamingService|SYSTEM|({user}[^\s"@]{1,2000}))"""",
    """\Wsuser=(({domain}[^\\\/=]{1,2000})[\\\/]{1,2000})?(HiveStreamingService|SYSTEM|({user}[^=\s"@]{1,2000}?))(\s{1,100}\w+=|\s{0,100}$)""",
    """flexString1=({alert_name}[^\s]{1,2000})\s\w+=""",
    """eventType=({alert_name}[^\s]{1,2000})\s\w+="?""",
    """applicationName =({process_name}[^\s]{1,2000})\s\w+="""",
    """targetPriorityType=({alert_severity}[^\s]{1,2000})\s\w+="?""",
    """\Wmsg=({additional_info}[^=]{1,2000})\s{1,100}(\w+=|$)""",
    """flexString1=({alert_type}[^\s]{1,2000})""",
    """threatIndicators[^":].+?=({alert_type}[^\s"]{1,2000})""",
    """applicationPath=({process}(({directory}[^"=,]{1,2000})\\)?({process_name}[^\s\\]{1,2000}))\s\w+=""",
    """dhost=({web_domain}[^\s]{1,2000}\.[^\s]{1,2000})""",
    """dst=({dest_ip}[^\s]{1,2000})""",
    """fname=\s{0,100}({file_path}(\w:|\\\\)[^\s]{1,2000})\s{1,100}""",
    """fname=\s{0,100}({file_name}[^\\\/"]{1,2000}?)\s{1,100}(\w+=|$)""",
    """fname=\s{0,100}({file_parent}(\w:|\\\\).+?)\\+(?:[^\\=]{1,2000}?)\s{1,100}""",
    """fname=\s{0,100}(|([^\/,]{1,2000}?(\.({file_ext}[^\/,\.]{1,2000}?))?))\s{1,100}(\w+=|$)""",
    """>\s{0,100}({file_name}[^<"']{1,2000}?)<\/link><\/share>"{0,20}\s{0,100}was created by the application""",
    """fname=\s{0,100}({file_path}(({file_parent}\w+:[^"].+?)\\+)\s{0,100}({file_name}[^"\\,:]{1,2000}?))\s{1,100}\w+=""",
    """act=({accesses}[^=]{1,2000})\s{1,100}(\w+=|$)""",
    """"eventId":"({alert_id}[^"]{1,2000})"""",
    """"parentApp":\{[^}]{1,2000}"md5Hash":"({parent_md5hash}[^"]{1,2000})""",
    """"parentApp":\{[^}]{1,2000}"sha256Hash":"({parent_sha256}[^"]{1,2000})"""",
    """"targetApp":\{[^}]{1,2000}"sha256Hash":"({target_sha256}[^"]{1,2000})"""",
    """"targetApp":\{[^}]{1,2000}"md5Hash":"({target_md5hash}[^"]{1,2000})"""",
    """"selectedApp":\{[^}]{1,2000}"md5Hash":"({selected_md5hash}[^"]{1,2000})"""",
    """"selectedApp":\{[^}]{1,2000}"sha256Hash":"({selected_sha256}[^"]{1,2000})"""",
  ]
  DupFields = [ "directory->process_directory" 
}
```