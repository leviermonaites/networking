## VLANS
In this project I show the communication between hosts connected to the same switch but on different VLANs through a router.

Bullet points:
- The blue box you will find on the right represents VLAN 10. <br>
- The green box you will find on the left represents VLAN 20.
- VLAN 10's interface was configured with the following IP and IP submask on the switch: 192.168.0.1 255.255.240.0
- VLAN 20's interface was configured with the following IP and IP submask on the switch: 172.16.0.1 255.255.240.0
- There is a link between the interface GigabitEthernet 0/1 on the switch and the interface Gigabit Ethernet 0/0/1 on the router.
- On the router we have two sub interfaces on Gigabit Ethernet 0/0/1. 0/0/0.1 for VLAN 10, 0/0/0.2 for VLAN 20. (I've used trunking here)
- The address of the router's sub interface Gigabit Ethernet 0/0/0.1 is 192.168.0.1
- The address of the router's sub interface Gigabit Ethernet 0/0/0.2 is 172.16.0.1

If you try to ping 172.16.0.4 (the IP address of a host on VLAN 20) using the prompt command of some host from VLAN 10 (inside the blue box on the left) you will see that the flow of the packet is the following:
- Packet goes from the host to the switch.
- Switch forwards it to the router.
- Router forwards it back to the switch.
- Switch forwards it to the host from VLAN 20.
- Host responds to Switch
- Switch forwards the response to the router.
- Router forwards it back to the Switch.
- Switch forwards it to the initial host.
