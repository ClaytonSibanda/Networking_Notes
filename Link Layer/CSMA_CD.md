# Career Sense Multiple Access
Link layer protocol used in ethernet.
Link layer is implemented on the network interface card(NIC)


- __Carrier Sensing__ - refers to listening before transmitting(wait for the other person to finish talking before you start to talk)
    - So a node listens to the channel(carrier) before transmitting
    - If there is transmission the node waits until there is no transmission for a certain amount of time and then begins transmitting

- __Collision Detection__ - if someone else begins talking, stop talking. I a node is transmission and then another is also transmitting, it stops and wait for a random time before transmitting again to avoid collision. Problem comes up when two nodes start transmission at the same time, then we have a collision.



# Taking Turns Protocol
- This eliminates collisions as only one node can transmit at a timer
- makes use of a special frame called a token. The node with the token is the one that can transmit
- Node only holds the tokeen if it has frames to transmit
- the protocol is designed in such a way that node1 always passes the token to node2 and nodeN always passes it to node 1.
- problesm with token passing is when one node fails then the whole channel fails

- taking turns can also be implemented using a master node that determiens which node shoould transmit
