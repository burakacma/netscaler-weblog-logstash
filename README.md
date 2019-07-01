# netscaler-weblog-logstash
Netscaler weblog logstash configurasyon

## Grok Pattern 

```bash
logFormat =>  W3C %{%Y-%m-%dT%H:%M:%S.000Z}t %a %A %p %m %v %U %q %s %j %J %M %H %+{user-agent}i %+{referer}i

Grok Pattern => %{NOTSPACE:request_date} %{IPV4:client_ip} %{IPV4:server_ip} %{INT:server_port} %{WORD:request_type} %{URIHOST:hostname} %{URIPATH:request_path} %{NOTSPACE:query_string} %{INT:status_code} %{INT:request_size} %{INT:response_size} %{INT:request_time} %{NOTSPACE:protocol} %{NOTSPACE:user_agent} %{NOTSPACE:header_referer}
```

## Argument Table
[Citrix Netscaller Offical Argumant Table](https://docs.citrix.com/en-us/netscaler/media/argument-table.pdf)

