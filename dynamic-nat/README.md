Bullet points:
- This project is very much like the [Static NAT Project](../static-nat/static-nat.pkt), the only change here is that the network on the bottom-left is using dynamic NAT now for its multiple hosts.
- There is a NAT Pool on Router0 with addresses ranging from 192.0.2.3 to 192.0.2.8
- There is an Access List on Router 0 attached to the NAT pool permitting traffic from 192.168.0.x (this way NAT will be applied to all of the hosts on the LAN)
