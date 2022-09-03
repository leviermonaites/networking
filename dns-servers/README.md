Bullet points:
- DHCP server handing out IPs for network 192.168.0.0 /24
- 192.168.0.1 is excluded from the DHCP Server's pool as it is the router.
- 192.168.0.2 is excluded from the DHCP Server's pool as it is the DNS Server.
- 192.168.0.4 was the IP handed out to the WebServer
- ermonaites.com is configured as a domain in the DNS Server and its IP address is 192.168.0.4
- www.ermonaites.com is an CNAME record pointing to ermonaites.com
