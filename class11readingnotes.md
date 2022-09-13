Gary King
09/13/2022
Class 11 Reading Notes
Network Address Translation (NAT)
https://www.geeksforgeeks.org/network-address-translation-nat/

To access the Internet, one public IP address is needed, but we can use a private IP address in our private network. The idea of NAT is to allow multiple devices to access the Internet through a single public address. To achieve this, the translation of a private IP address to a public IP address is required.
It will also do the translation of port numbers i.e. mask the port number of the host with another port number, in the packet that will be routed to the destination. It then makes the corresponding entries of IP address and port number in the NAT table. NAT generally operates on a router or firewall. 
The border router is configured for NAT i.e the router which has one interface in the local (inside) network and one interface in the global (outside) network. When a packet traverses outside the local (inside) network, NAT converts that local (private) IP address to a global (public) IP address. 
 In a network, two hosts A and B are connected. Now, both of them request for the same destination, on the same port number, say 1000, on the host side, at the same time.
Inside local address – An IP address that is assigned to a host on the Inside (local) network. The address is probably not an IP address assigned by the service provider i.e., these are private IP addresses. This is the inside host seen from the inside network. 
 
Inside global address – IP address that represents one or more inside local IP addresses to the outside world. This is the inside host as seen from the outside network. 
 
Outside local address – This is the actual IP address of the destination host in the local network after translation. 
 
Outside global address – This is the outside host as seen from the outside network. It is the IP address of the outside destination host before translation. 
