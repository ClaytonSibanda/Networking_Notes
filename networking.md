# Traceroute 
__Routers__

Hop - physical distance between two nodes

__traceroute__
All traceroute impl depend on ICMP packets

_timetolive_ - number of hops a packet is permitted to travel before a router discards it

Traceroute will send probe packet with a small TTL(time to live) and then listen to an ICMP (time exceeded) response from the gateway
We start with a ttl of one and increase by one until we get an ICMP "port unreachable" reply which means we got to the host

- it measures transit delay
- it displays the route/path of packets accross an IP
 network

**Meaning of traceroute results**

Each hop is represented by a different line.
Each line has 5 columns

- first column is the number of the hop
- traceroute sends 3 packets and measure the time taken for each
*** means that the server at the node does not accept ICMP packets
