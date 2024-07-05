Network Configuration Task
You are tasked with configuring the network for DAYA AMINATION as per the following topology and addressing table.

Addressing Table
Device	Interface	IP Address	Subnet Mask	Default Gateway
Admin Block	Fa0/0	172.16.12.1	255.255.255.0	N/A
Fa0/1	172.16.13.1	255.255.255.248	N/A
Se0/0/0	10.1.1.1	255.255.255.252	N/A
Patients Block	Fa0/0	172.16.14.1	255.255.255.0	N/A
Fa0/1	172.17.15.1	255.255.255.248	N/A
Se0/0/0	10.1.1.2	255.255.255.252	N/A
Switch1	VLAN1	192.168.10.2	255.255.255.0	192.168.10.1
Switch2	VLAN1	192.168.10.3	255.255.255.0	192.168.10.1
Switch3	VLAN1	192.168.10.4	255.255.255.0	192.168.10.1
Switch4	VLAN1	172.16.2.4	255.255.255.0	172.16.21
Switch5	VLAN1	172.16.2.5	255.255.255.0	172.16.2.1
PC1	NIC	192.168.10.6	255.255.255.0	192.168.10.1
PC2	NIC	192.168.10.7	255.255.255.0	192.168.10.1
PC3	NIC	192.168.10.8	255.255.255.0	192.168.10.1
PC4	NIC	192.168.11.2	255.255.255.0	192.168.11.1
PC5	NIC	192.168.11.3	255.255.255.0	192.168.11.1
PC6	NIC	192.168.11.4	255.255.255.0	192.168.11.1
Your tasks are to:

Configure basic router and switch configurations as per the addressing table.
Configure OSPF to route packet network.
Configure basic router and switch security:
Set minimum password length to 6 characters.
Encrypt plaintext passwords.
Configure AAA local authentication in Administration Block:
Create local users with a secret password and privilege level 15 for admin.
Enable AAA services.
Implement AAA services using the local database as the first option.
Configure a site-to-site IPsec VPN between Administration Block and Patients Block.
Configure ACL 101 to allow traffic from the Administration Block Fa0/0 network to access Patients Block Fa0/1 LAN.
Configure the crypto ISAKMP policy 10 phase I properties.
Configure firewall and ISP settings on Administration Block Router:
Configure Zone-Based Policy Firewall:
Create a zone name.
Create an ACL number 110 that defines internal traffic, which permits all IP protocols from the 172.16.12.1/24 source network to any destination.
Create a policy map that inspects all matched traffic.
Create a zone pair name.
Configure ASA basic security and firewall settings:
Create a user and configure AAA to use the local database for remote authentication.
Configure the ASA as a DHCP server by assigning IP addresses to inside DHCP clients from 192.168.10.5 to 192.168.10.100.
Enable DHCP to listen for DHCP client requests.
Configure static routing and NAT.
Provide the complete set of commands required to achieve these configurations.
