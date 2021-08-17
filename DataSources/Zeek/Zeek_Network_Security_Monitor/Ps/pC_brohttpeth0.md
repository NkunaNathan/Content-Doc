#### Parser Content
```Java
{
Name = bro-httpeth0
  Vendor = Zeek
  Product = Zeek Network Security Monitor
  Lms = Direct
  DataType = "web-activity"
  TimeFormat = "epoch_sec"
  Conditions = [ "/http_eth0.log" ]
  Fields = [
    """exabeam_host=({host}[\w.\-]{1,2000})""",
    """({time}\d{10})\.\d{6}\t({conn_id}[^\t]{1,2000})\t(?:-|(({src_ip}(\d{1,3}\.){3}\d{1,3}|([A-Fa-f0-9%.]{0,2000}:[A-Fa-f0-9%.:]{1,2000}(th0)?))|[^\t]{1,2000}))\t(?:-|(({src_port}\d{1,100}?)|[^\t]{1,2000}))\t(?:-|(({dest_ip}(\d{1,3}\.){3}\d{1,3}|([A-Fa-f0-9%.]{0,2000}:[A-Fa-f0-9%.:]{1,2000}(th0)?))|[^\t]{1,2000}))\t(?:-|(({dest_port}\d{1,100}?)|[^\t]{1,2000}))\t(?:-|([^\t]{1,2000}))\t(?:-|({method}[^\t]{1,2000}))\t(?:-|([^\t]{1,2000}))\t([^\t]{1,2000})\t(?:-|({referrer}[^\t]{1,2000}))\t(?:-|([^\t]{1,2000}))\t(?:-|({user_agent}[^\t]{1,2000}))\t(?:-|([^\t]{1,2000}))\t(?:-|([^\t]{1,2000}))\t(?:-|({result_code}[^\t]{1,2000}))\t(?:-|({status_msg}[^\t]{1,2000}))\t(?:-|([^\t]{1,2000}))\t(?:-|([^\t]{1,2000}))\t(?:-|(\(empty\))|({tags}[^\t]{1,2000}))\t(?:-|({user}[^\t]{1,2000}))\t(?:-|([^\t]{1,2000}))\t(?:-|({proxied}[^\t]{1,2000}))\t(?:-|([^\t]{1,2000}))\t(?:-|({orig_filenames}[^\t]{1,2000}))\t(?:-|([^\t]{1,2000}))\t(?:-|([^\t]{1,2000}))\t(?:-|([^\t]{1,2000}))\t(?:-|({mime}[^\t]{1,2000}?))\s{0,100}$""",
    """({time}\d{10})\.\d{6}\t({conn_id}[^\t]{1,2000})\t(?:-|(({src_ip}(\d{1,3}\.){3}\d{1,3}|([A-Fa-f0-9%.]{0,2000}:[A-Fa-f0-9%.:]{1,2000}(th0)?))|[^\t]{1,2000}))\t(?:-|(({src_port}\d{1,100}?)|[^\t]{1,2000}))\t(?:-|(({dest_ip}(\d{1,3}\.){3}\d{1,3}|([A-Fa-f0-9%.]{0,2000}:[A-Fa-f0-9%.:]{1,2000}(th0)?))|[^\t]{1,2000}))\t(?:-|(({dest_port}\d{1,100}?)|[^\t]{1,2000}))\t(?:-|([^\t]{1,2000}))\t(?:-|({method}[^\t]{1,2000}))\t(?:-|([^\t]{1,2000}))\t([^\t]{1,2000})\t(?:-|({referrer}[^\t]{1,2000}))\t(?:-|({user_agent}[^\t]{1,2000}))\t(?:-|([^\t]{1,2000}))\t(?:-|([^\t]{1,2000}))\t(?:-|({result_code}[^\t]{1,2000}))\t(?:-|({status_msg}[^\t]{1,2000}))\t(?:-|([^\t]{1,2000}))\t(?:-|([^\t]{1,2000}))\t(?:-|({orig_filenames}[^\t]{1,2000}))\t(?:-|(\(empty\))|({tags}[^\t]{1,2000}))\t(?:-|({user}[^\t]{1,2000}))\t(?:-|([^\t]{1,2000}))\t(?:-|({proxied}[^\t]{1,2000}))\t(?:-|([^\t]{1,2000}))\t(?:-|([^\t]{1,2000}))\t(?:-|([^\t]{1,2000}))\t(?:-|({mime}[^\t]{1,2000}?))\s{0,100}$""",
    """\d{10}\.\d{6}\t([^\t]{1,2000}\t){7}(?:-|(?!(\d{1,3}\.){3}\d{1,3})({web_domain}.+?))\s{0,100}\t([^\t]{1,2000}\t){16}(?:-|({mime}[^\t]{1,2000}))\t""",
    """\d{10}\.\d{6}\t([^\t]{1,2000}\t){7}[^\t]{0,2000}?({top_domain}[^\t.]{1,2000}(?:\.(?:com|net|info|edu|org|gov|co|jp|ru|de|ir|it|in|fr|info|pl|nl|es|gr|cz|eu|tv|me|jp|ca|cn|uk|my|cc|id|us|nz|biz|club|io|gg|fi|au|st|tw|asia|sg|ie|li|za))+)""",
    """\d{10}\.\d{6}\t([^\t]{1,2000}\t){8}(?:-|({uri_path}[^\t\?]{1,2000})(\?({uri_query}[^\t]{1,2000}))?)""",
    """\d{10}\.\d{6}\t([^\t]{1,2000}\t){11}[^\t]{0,2000}?({browser}Chrome|Safari|Opera|(?:F|f)irefox|MSIE|Trident)""",
    """\d{10}\.\d{6}\t([^\t]{1,2000}\t){11}[^\t]{0,2000}?({os}iOS|Android|BlackBerry|Windows Phone|BeOS|(?:X|x)11|(?:W|w)indows|(?:L|l)inux|(?:M|m)acintosh|(?:D|d)arwin)""",
    """({protocol}http)"""
  ]
}
```