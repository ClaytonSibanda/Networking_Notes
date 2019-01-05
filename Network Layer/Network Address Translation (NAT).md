used for home networks where many ip addresses are needed for different devices.

A NAT router is connected to many hosts and is used to access those hosts from the broader internet.

From the outside the NAT router is as if was a single device with a single IP address. The NAT router hides the details of the home network from the rest of the world. A DHCP server in the NAT router is used to assign addresses to the devices in the home network.

A NAT translation table contains ports and IP addresses. It is used to determine how packets are forwarded to different hosts in the home network.

_example_

If a host with ip 10.0.0.1:3345 sends request to 196.3.45.1:20. The NAT router will generate an unused port and save it with 10.0.0.1 in the table. It will then replace the source IP(with its IP i.e 138.76.29.7) and the source port(with the new port not in the NAT table i.e 5001) in the packets before forwarding them to the global internet. When the response returns the NAT uses the destination ip address and the port to index the table to obtain the actual IP address and the actual port number.

_contains source address and source ports only_

|NAT translation table|
|----------------------|
| WAN side  | LAN side  |      
| 138.76.29.7, 5001  |10.0.0.1, 3345   |  
