# The Internet Protocol (IP): Forwarding and Addressing in the Internet

forwarding happens inside the router using forwarding tables that are determined by the routing algorithms


__Addressing__

Currently the Internet uses the classless interdomain routing(CIDR) for addressing
Classful addressing led to underutilization of ip addresses hence was dropped.

An IP4 address is a 32 bit number written dot notation i.e a.b.c.d/x each number being 8 bits

_x_ is called the network prefix. It represents the number of bits used to identify the network. The rest 32-x bits are used to distinguish among devices in the network.

__IP addresses__

A router connects a host to the Internet. This router is called a default gateway.
The connection between a router and a host is called an Interface. A router can have multiple interfaces.

An interface therefore has an ip address. Ip address does not belong to the router/host but the interface.

__SUBNETTING__

a subnent is a routerless network. It consists of multiple hosts connected to the same default gateway(router).

_example of subnet addresses_

 223.1.1.0/24
 /24 is the subnet mask, meaning that 24 bits of the 32 bits belong to the subnet

 __Broadcast Address__

 it is 255.255.255.255
 It is used to send a message to all the hosts on the same subnet
