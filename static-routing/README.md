
## Concept
Static routing is a form of routing that occurs when a router uses a manually-configured routing entry, rather than information from dynamic routing traffic. (Credits: [Wikipedia](https://en.wikipedia.org/wiki/Static_routing))

## Bullet points:
- Router from 172.16.0.0 has a static route configured to communicate with the client from 192.168.0.0 (the next hop is the router from 192.168.0.0)
- Router from 192.168.0.0 has a static route configured to communicate with the client from 172.16.0.0 (the next hop is the router from 172.16.0.0)

These bullet points make it possible for one client ping the other.
![Image showing the project on the Cisco Packet Tracer software](static-routing.png)
