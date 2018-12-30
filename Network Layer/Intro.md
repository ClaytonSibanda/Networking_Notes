__Routing vs Forwarding__

Routing - involves all network's routers to determine path to be taken from source to destination(makes use  routing algorithms)
Forwarding - involves transfer of a packet from an incoming link to an appropriate output link within a single router.

Routing Analogy- travelling from Cape Town to Joburg. We can think of routing as the process of planning the journey before starting the journey.
Forwarding Analogy - we can think of Forwarding as a car taking an interchange to take another road.

Every router has a Forwarding table used to choose the best path.
Routers use a field in the packets to determine the output link
Routing algorithm determine numbers inserted into the Forwarding table
Routers are network layer switches

Network layer can also offer connectionless and connection oriented services

Network layer provides either a host-to-host connectionless service or a host-to-host connection oriented services

__Virtual Circuit networks__

refers to networks that provide only a connection oriented service at the network layer

__Datagram networks__

refers to networks that provide a connectionless service at the network layer.
Internet is a datagram network.
- this involves the use of addresses carried by packets to forward packets through different paths from source to destination.

    __longest prefix matching__

    Is done in datagram networks e.g the Internet.
    Used to forward packets to the correct outgoing links

    Prefix Match                     Link Interface

11001000 00010111 00010    ->         0

11001000 00010111 00011000 ->         1

11001000 00010111 00011   ->          2

otherwise                 ->            3

With this style of forwarding table, the router matches a prefix using the packet's destination address. The longest prefix is used to choose which link is to be chosen. If two matches are found then the longest match is taken.
