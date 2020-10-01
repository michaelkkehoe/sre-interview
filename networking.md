## General
* What is the benefit of a protocol like QUIC
* Why would you potentially want to use UDP for a long-distance VPN connection (non commercial)
* What protocol is usually used within corporate networks
* What are some of the TCP congestion protocols
* What is IP fragmentation
* Explain how ping works
* What is TCP Fast Open and what are the reasons to use it and not to use it. 


## IP Addressing
* How many usable addresses in a /24
* How large is a /16
* What is RFC-1918 
* What is the subnet mask of 10.2.1.2/22

## OSI Model
1. What is the OSI model
  * Physical
  * Data
  * Network
  * Transport
  * Session
  * Presentation
  * Application

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
1. Name some L7 protocols
  * DNS
  * HTTP/ HTTPS/ HTTP2
  * QUIC
  * NTP
  * SNMP
  * SSH
  * DHCP

## Loadbalancing
1. What's the difference between a L2, L4, L7 load-balancer
2. What are the various load-balancing methods?

## Routing Protocols
### BGP
1. What the 6 BGP session states
2. What port/ protocol does BGP run on
3. Explain the difference between eBGP and iBGP
4. What is the smallest prefix size you can publically announce
5. What is a BGP community?
6. What is the administrative distance BGP uses for iBGP and eBGP
7. What is the difference between a hard reset and soft reset
8. What are the different BGP message types
9. What are the BGP path attributes
10. What is an AS
11. What is a route reflector
12. What is the BGP path selection criteria
13. What is the purpose of route dampening

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

## Good Reads
* [How do TCP Sockets work](https://eklitzke.org/how-tcp-sockets-work)
* [The inner workings of bind and listen on Linux](https://ops.tips/blog/how-linux-tcp-introspection/)
* [How TCP backlog works in Linux](http://veithen.io/2014/01/01/how-tcp-backlog-works-in-linux.html)

## Question References
* http://networkerinterview.net/entries/bgp/border-gateway-protocol-ccnp
