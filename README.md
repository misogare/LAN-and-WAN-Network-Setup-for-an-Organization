LAN and WAN Network Setup for an Organization
This project describes the LAN and WAN network setup for an organization, including the network address, subnet mask, and usage for each subnet. The network devices, interfaces, IP addresses, subnet masks, and default gateway are also provided.

Network Addressing Scheme
| Network | Address |	Subnet Mask |	Used for |
| ------------- | ------------- | ------------- |
| 192.168.50.0/24 | 255.255.255.0 | VLAN 50 (Business) |
| 192.168.60.0/24 | 255.255.255.0 | VLAN 60 (HR) |
| 192.168.99.0/24 | 255.255.255.0 | VLAN 99 (Management) |
| 10.0.0.0/30 | 255.255.255.252 | WAN (Melbourne to Perth) |
| 209.195.205.0/29 | 255.255.255.248 | Internet (Lo1) |
Network Devices
|Device|Interface|IP Address|Subnet Mask|Default Gateway|
|Melbourne|S0/0/1|10.0.0.1|255.255.255.252|N/A|
|G0/1.50|192.168.50.1|255.255.255.0|N/A|
|G0/1.60|192.168.60.1|255.255.255.0|N/A|
|G0/1.99|192.168.99.1|255.255.255.0|N/A|
|Perth|S0/0/0|10.0.0.2|255.255.255.252|N/A|
|Lo1|209.195.205.1|255.255.255.248|N/A|
|S1|VLAN 99|192.168.99.11|255.255.255.0|192.168.99.1|
|S2|VLAN 99|192.168.99.12|255.255.255.0|192.168.99.1|
|PC-A|NIC|192.168.50.2|255.255.255.0|192.168.50.1|
|PC-B|NIC|192.168.50.3|255.255.255.0|192.168.50.1|
|PC-C|NIC|192.168.60.2|255.255.255.0|192.168.60.1|
|PC-D|NIC|192.168.50.4|255.255.255.0|192.168.50.1|
|PC-E|NIC|192.168.60.3|255.255.255.0|192.168.60.1|
How to Use
This project provides a simple example of a LAN and WAN network for an organization using the IP addressing scheme outlined in the table. To use this project, simply follow the instructions below:

Set up the devices according to the IP addressing scheme outlined in the table above.
Connect the devices together as shown in the diagram.
Configure the devices with the appropriate IP addresses and default gateways.
Test connectivity between the devices to ensure that the network is functioning correctly.
