## Concept
Port Address Translation (PAT), is an extension to network address translation (NAT) that permits multiple devices on a local area network (LAN) to be mapped to a single public IP address. The goal of PAT is to conserve IP addresses. Most home networks use PAT. (Credits: [TechTarget](https://www.techtarget.com/searchnetworking/definition/Port-Address-Translation-PAT#:~:text=Port%20Address%20Translation%20(PAT)%2C,Most%20home%20networks%20use%20PAT.))

## Bullet points:
- The WebServer's router public IP address is 198.51.100.2
- The WebServer has an HTTP server running on port 80 (which is accessible by clients on their browsers)
- The WebServer's router is forwarding traffic coming to its port 80 to the WebServer on port 80 using PAT.

![PAT project on Cisco Packet Tracer](pat.png)
![WebServer's HTTP Web page](web-server-http-server.png)
