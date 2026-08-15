# Packet Tracer - Use Telnet and SSH

## Objective

Establish a remote connection to a router using Telnet and SSH and compare the two remote-access protocols.

## Network Topology

The lab consists of:

- HQ Router
- PC0
- PC1

The HQ router uses the following address:

- IP Address: `64.100.1.1`
- Subnet Mask: `255.255.255.0`

PC0 and PC1 obtain their IP addresses through DHCP.

## Part 1: Verify Connectivity

### 1. Verify IP Address

The PC was checked to confirm that it received an IP address from the DHCP server.

Command used:

ipconfig

### Verify Connectivity to HQ 

ping 64.100.1.1

### Remote Access 
1. Telnet 
telnet 64.100.1.1

The connection was unsuccessful because the router was configured not to allow insecure Telnet access.

2. SSH
ssh -l admin 64.100.1.1 

Password: 
class 

The SSH connection was successful and provided remote access to the HQ router.


## Screenshots 

### IP 
![PING TEST](Screenshots/ip.png)

