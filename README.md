# temp

sing-box config:
```
{"inbounds":[{"auto_route":true,"domain_strategy":"","endpoint_independent_nat":true,"inet4_address":"172.19.0.1/28","interface_name":"nekoray-tun","mtu":9000,"sniff":true,"sniff_override_destination":false,"stack":"gvisor","strict_route":true,"tag":"tun-in","type":"tun","inet4_route_exclude_address":["10.0.0.0/8","172.16.0.0/12","192.168.0.0/16","fc00::/7","fe80::/10","fd00::/8"]}],"log":{"level":"warn"},"outbounds":[{"domain_strategy":"","server":"172.16.10.84","server_port":8686,"tag":"proxy","type":"socks"},{"tag":"direct","type":"direct"},{"tag":"bypass","type":"direct"},{"tag":"block","type":"block"},{"tag":"dns-out","type":"dns"}],"route":{"final":"proxy","rules":[{"ip_cidr":["10.0.0.0/8","172.16.0.0/12","192.168.0.0/16"],"outbound":"bypass"}]}}
```
