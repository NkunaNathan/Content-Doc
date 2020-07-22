#### Parser Content
```Java
{
Name = s-mssql-database-login
  DataType = "database-login"
  Conditions = [ """EventCode=33205""", """action_id:LGIS""" ]
}

${MicrosoftParserTemplates.s-mssql-database-login}{
  Name = s-mssql-database-login-failed
  DataType = "database-failed-login"
  Conditions = [ """EventCode=33205""", """action_id:LGIF""" ]
  Fields = ${MicrosoftParserTemplates.s-mssql-database-login.Fields} [
    """\Wstatement:({failure_reason}[^.]+)"""
  ]
}

${MicrosoftParserTemplates.s-mssql-database-query}{
  Name = s-mssql-database-query-al
  DataType = "database-query"
  Conditions = [ """EventCode=33205""", """action_id:AL""" ]
}

${MicrosoftParserTemplates.s-mssql-database-query}{
  Name = s-mssql-database-query-dl
  DataType = "database-query"
  Conditions = [ """EventCode=33205""", """action_id:DL""" ]
}

${MicrosoftParserTemplates.s-mssql-database-query}{
  Name = s-mssql-database-query-sl
  DataType = "database-query"
  Conditions = [ """EventCode=33205""", """action_id:SL""" ]
}

{
  Name = xml-microsoft-dns-query
  Vendor = Microsoft
  Product = Microsoft Windows DNSServer
  Lms = Direct
  DataType = "dns-query"
  IsHVF = true
  TimeFormat = "yyyy-MM-dd'T'HH:mm:ss.SSSSSSSSSZ"
  Conditions = [ """<Data Name='QNAME'>""", """<Data Name='QTYPE'>""", """<Data Name='Flags'>""" ]
  Fields = [
    """<TimeCreated SystemTime='({time}\d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\d\.\d{9}Z)""",
    """<Computer>({host}.+?)<\/Computer>""",
    """<Data Name='InterfaceIP'>({dest_ip}[A-Fa-f:\d.]+)""",
    """<Data Name='Source'>({src_ip}[A-Fa-f:\d.]+)""",
    """<Data Name='Port'>({src_port}\d+)""",
    """<Data Name='QNAME'>({query}.+?)<\/Data>""",
    """<Data Name='QTYPE'>({query_type}.+?)<\/Data>""",
    """<Data Name='Flags'>({query_flags}.+?)<\/Data>""",
  ]
}
```