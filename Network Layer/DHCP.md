# Dynamic Host Configuration Protocol

Used for automatically assigning IP addresses to hosts in a network. It is also called a _plug and play Protocol_


__How it works__

_DHCP discover_: client sends a DHCP discover message to identify a DHCP server to interact with. Destination address of this packet is 255.255.255.255

_DHCP server offer_: DHCP server responds to the client with an offer message(DHCP offer message). This message is also broadcasted to all the hosts using the IP 255.255.255.255.  This message contains the proposed Ip address, subnet mask and the IP lease time.

_DHCP request_: client chooses from one of the offer messages and echoes back the Configuration details. It sends back a DHCP request message.

_DHCP ACK_: The server responds to a DHCP request message with q DHCP ACK, confirming the request parameters.
