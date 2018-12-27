# ICMP

## Internt Control Message Protocol

- mostly used for error reporting in the network layer
- ICMP messages are carried inside IP datagrams
- ICMP messages have a type and a code

How Ping works

Ping sends an ICMP(type8 code0(echo request)) message to the specified host
The host on seeing the request sends back another ICMP(type 0 code 0(echo reply)) message as a response
