# Networking

## General

*Q: What is the benefit of a protocol like QUIC?*

*Q: Why would you potentially want to use UDP for a long-distance VPN connection (non commercial)?*

*Q: What protocol is usually used within corporate networks?*

*Q: What are some of the TCP congestion protocols?*

*Q: What is IP fragmentation?*

*Q: Explain how ping works?*

## IP Addressing
*Q? How many usable addresses in a /24?*

A: 254 (including gateway address)

*Q: How many usable addresses in a /31?*

A: Technically 0, but in practice 2


*Q: How many usable addresses in a /30?*
A: 2

*Q: How large is a /16?*

A: 2^16 = 65536

*Q: What is RFC-1918?*  

A:
* Address Allocation for Private Internets
* 10/8, 172.16/12, 192.168/16 prefixes are assigned here

*Q: What is the subnet mask of 10.2.1.2/22?*
A:

* 255.255.252.0
* See [IPv4 subnetting cheatsheet](https://packetlife.net/media/library/15/IPv4_Subnetting.pdf)

## OSI Model

*Q:What is the OSI model?*

A:

1. Physical
2. Data
3. Network
4. Transport
5. Session
6. Presentation
7. Application

*Q: What is your favourite protocol in the OSI layer?*

### L1 Protocols

*Q: Explain the L1 model*?

*Q: What are some L1 protocols

*Q: How do you troubleshoot a layer 1 issue with an ethernet jack?*

*Q: How do you troubleshoot a flapping link between 2 routers?*

### L2 Protocols

*Q: Describe the Ethernet Protocol?*

*Q: What is ARP?*

*Q: What is the purpose of the broadcast address in a network?*

### L3 Protocols

#### IPv4

*Q: Describe an IPv4 packet*

*Q: What is the purpose of the ECN field?*

*Q: What are some of the options that can be set in an IPv4 field?*

*Q: What are examples of IP protocols?

A:

* https://en.wikipedia.org/wiki/List_of_IP_protocol_numbers

*Q: Describe IP-in-IP*

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

*Q: Name some L7 protocols?*

A:

* DNS
* HTTP/ HTTPS/ HTTP2
* QUIC
* NTP
* SNMP
* SSH

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

*Q: What the 6 BGP session states?*

A:

* Idle
* Connect
* Active
* OpenSent
* OpenConfirm
* Established

*Q: What port/ protocol does BGP run on?*

A: TCP/179

*Q: Explain the difference between eBGP and iBGP?*

A:

* eBGP is used for communication between different autonomous systems
*  [Reference](https://ipwithease.com/ebgp-vs-ibgp/)

*Q: What is the smallest prefix size you can publically announce?*

A: Reliably /24

*Q: What is a BGP community?*

A:

*Q: What is the administrative distance BGP uses for iBGP and eBGP?*

A:

* iBGP 200
* eBGP 20

*Q: What is the difference between a hard reset and soft reset?*
A: 

*Q: What are the different BGP message types?*

A: 

*Q: What are the BGP path attributes?*

A:

*Q: What is an AS?*

*Q: What is a route reflector?*

A:

*Q: What is the BGP path selection criteria?*

*Q: What is the purpose of route dampening?*

### OSPF

*Q: What is a OSPF?*

*Q: What are the steps to create router adjacency?*

*Q: What is a LSA?*
*Q: What is a LSU?*

*Q: What is a LSR?*

*Q: What is an OSPF backbone area?*

*Q: What are the different neighbour states?*

*Q: What are the different OSPF network types?*

*Q: What is the default link cost?*

*Q: Explain stubby areas and non-so-stubby-area?*

*Q: What are the three types of authentication supported by OSPF?*

## Good Reads

* [How do TCP Sockets work](https://eklitzke.org/how-tcp-sockets-work)
* [The inner workings of bind and listen on Linux](https://ops.tips/blog/how-linux-tcp-introspection/)
* [How TCP backlog works in Linux](http://veithen.io/2014/01/01/how-tcp-backlog-works-in-linux.html)
* [SYN Packet handling in the wild](https://blog.cloudflare.com/syn-packet-handling-in-the-wild/)

## References

* http://networkerinterview.net/entries/bgp/border-gateway-protocol-ccnp
