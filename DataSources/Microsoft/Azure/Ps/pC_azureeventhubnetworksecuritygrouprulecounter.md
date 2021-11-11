#### Parser Content
```Java
{
Name = azure-event-hub-network-security-group-rule-counter
  DataType = "network-connection"
  Conditions = ["""ext_category=NetworkSecurityGroupRuleCounter""" ]
  Fields = ${MSParserTemplates.cef-azure-event-hub.Fields}[
     """\WrequestClientApplication=(|({app}.+?))(\s{1,100}\w+=|\s{0,100}$)""",
    """category":"({activity}.*?[^\\])"""",
    """type":"({outcome}.*?[^\\])"""",
    """rule":"({ruleName}.*?[^\\])"""",
    """primaryIPv4Address":"({src_ip}.*?[^\\])"""",
    """ruleName":"({rule}.*?[^\\])"""",
    """direction":"({direction}.*?[^\\])"""",
  ]
}
cef-azure-event-hub = {
  Vendor = Microsoft
  Product = Azure
  Lms = Direct 
  TimeFormat = "yyyy-MM-dd'T'HH:mm:ss"
  Fields = [
      """({time}\d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\d)\.\d{1,100}Z [\w\-.]{1,2000} Skyformation""",
      """"time":"({time}\d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\d)"""
      """\Wdvc=({host}\S+)""",
      """\Wdvchost=({host}[\w\-.]{1,2000})""",
      """exabeam_host=([^=]{1,2000}@\s{0,100})?({host}\S+)""",
      """\Wact=({activity}[^=]{1,2000})\s{1,100}(\w+=|$)""",
      """([^\|]{0,2000}\|){5}({activity}[^\|]{1,2000})""",
      """\WflexString1=({activity}[^=]{1,2000})\s{1,100}(\w+=|$)""",
      """\WdestinationServiceName =({app}[^=]{1,2000})\s{1,100}(\w+=|$)""",
      """\Wfname=({object}[^=]{1,2000})\s{1,100}(\w+=|$)""",
      """\Wmsg=({additional_info}[^=]{1,2000})\s{1,100}(\w+=|$)""",
      """\Wduser=(anonymous|({user_email}[^@=]{1,2000}@[^@=]{1,2000}?)|({user}.+?))(\s{1,100}[\S]=|\s{0,100}$)""",
      """\Wsuser=(anonymous|({user_email}[^@=]{1,2000}@[^@=]{1,2000}?)|({user}.+?))(\s{1,100}[\S]{1,2000}=|\s{0,100}$)""",
      """\Wsuid=(anonymous|({user_email}[^@=]{1,2000}@[^@=]{1,2000}?)|({user}.+?))(\s{1,100}[\S]{1,2000}=|\s{0,100}$)""",
      """\Woutcome=({outcome}[^=]{1,2000})\s{1,100}(\w+=|$)""",
      """\Wsrc=({src_ip}\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})""",
      """\Wshost=(|--|({src_host}[^=]{1,2000}))(\s{1,100}\w+=|\s{0,100}$)""",
      """"description":"({additional_info}[^"]{1,2000})""",
      """\Wext_identity_claims_name=(|({user}[^=]{1,2000}))(\s{1,100}\w+=|\s{0,100}$)""",
      """\Wext_callerIpAddress=({src_ip}[a-fA-F\d.:]{1,2000})""",
      """Namespace:\s{0,100}(|({event_hub_namespace}[^\]]{1,2000}?))\s{0,100}[\];]""",
      """EventHub name:\s{0,100}(|({event_hub_name}[^\]]{1,2000}?))\s{0,100}\]""",
      """\[Namespace:\s{0,100}({host}\S+) ; EventHub name:"""
  ]}
```