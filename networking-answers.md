## General
* What is the benefit of a protocol like QUIC
* Why would you potentially want to use UDP for a long-distance VPN connection (non commercial)
* What protocol is usually used within corporate networks
* What are some of the TCP congestion protocols
* What is IP fragmentation
* Explain how ping works

## IP Addressing
* How many usable addresses in a /24
** 254 (including gateway address)
* How many usable addresses in a /31
** Technically 0, but in practice 2
* How many usable addresses in a /30
** 2
* How large is a /16
** 2^16 = 65536
* What is RFC-1918 
** Address Allocation for Private Internets
** 10/8, 172.16/12, 192.168/16 prefixes are assigned here
* What is the subnet mask of 10.2.1.2/22
** 255.255.252.0
** See [IPv4 subnetting cheatsheet](https://packetlife.net/media/library/15/IPv4_Subnetting.pdf)

## OSI Model
* What is the OSI model
** Physical
** Data
** Network
** Transport
** Session
** Presentation
** Application

### L1 Protocols
1. Explain the L1 model
2. What are some L1 protocols
3. How do you troubleshoot a layer 1 issue with an ethernet jack
4. How do you troubleshoot a flapping link between 2 routers

### L2 Protocols
1. Describe the Ethernet Protocol
2. What is ARP
3. What is the purpose of the broadcast address in a network

### L3 Protocols
#### IPv4
1. Describe an IPv4 packet
2. What is the purpose of the ECN field
3. What are some of the options that can be set in an IPv4 field
4. What are examples of IP protocols
  * https://en.wikipedia.org/wiki/List_of_IP_protocol_numbers
5. Describe IP-in-IP 

#### IPv6
1. Describe an IPv6 packet
2. What are some benefits of IPv6

#### ICMP
1. Describe how traceroute works
2. Describe how ping works
3. Describe how tcptraceroute works

### L4 Protocols
#### TCP
1. What are the 6 TCP flags

### L7 Protocols
* Name some L7 protocols
** DNS
** HTTP/ HTTPS/ HTTP2
** QUIC
** NTP
** SNMP
** SSH
** DHCP

## Loadbalancing
* What's the difference between a L2, L4, L7 load-balancer

* What are the various load-balancing methods?
** Round Robin
** Weighted Round Robin
** Least Connections
** Weighted least connections
** Fixed Weighting
** Hash (L7)
** SRC IP Hash
** Response time
** [Power of Two Random Choices](https://www.haproxy.com/blog/power-of-two-load-balancing/)

## Routing Protocols
### BGP
* What the 6 BGP session states
** Idle
** Connect
** Active
** OpenSent
** OpenConfirm
** Established
* What port/ protocol does BGP run on
** TCP/179
* Explain the difference between eBGP and iBGP
** eBGP is used for communication between different autonomous systems
** [Reference](https://ipwithease.com/ebgp-vs-ibgp/)
* What is the smallest prefix size you can publically announce
** Reliably /24
* What is a BGP community?
* What is the administrative distance BGP uses for iBGP and eBGP
** iBGP 200
** eBGP 20
* What is the difference between a hard reset and soft reset
* What are the different BGP message types
* What are the BGP path attributes
* What is an AS
* What is a route reflector
* What is the BGP path selection criteria
* What is the purpose of route dampening

### OSPF
1. What is a OSPF
2. What are the steps to create router adjacency
3. What is a LSA
4. What is a LSU
5. What is a LSR
6. What is an OSPF backbone area
7. What are the different neighbour states
8. What are the different OSPF network types
9. What is the default link cost
10. Explain stubby areas and non-so-stubby-area
11. What are the three types of authentication supported by OSPF

## References
* http://networkerinterview.net/entries/bgp/border-gateway-protocol-ccnp
