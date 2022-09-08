Gary King
09/08/2022
Class 08 Reading Notes
Routing
Each VirtualBox VM can use up to eight network adapters, each of which in turn is referred to as a network interface controller (NIC). Four virtual network adapters can be configured in the VirtualBox GUI.
A network of 8 adaptors with Virtual Box can be configured with the VBOXMANAGE modifyvm command.
The different type of network adaptors are  AMD PCnet-PCI II (Am79C970A), AMD PCnet-FAST III (Am79C973), Intel PRO/1000 MT Desktop (82540EM), Intel PRO/1000 T Server (82543GC), Intel PRO/1000 MT Server (82545EM), Paravirtualized Network Adapter (virtio-net).
Jumbo frame support can support packet sizes of 1,500 bytes.
The different network modes are Not Attached, NAT, NAT Network, Bridge Adaptor, Internal Network, Host Only Adaptor and Generic Driver.
Not Attached is like if you were not connected to the net.
NAT mode is enabled for a virtual network adapter by default where a guest OS can access the host network.
NAT Networkis similar to the NAT mode that you use for configuring a router
If NAT Network mode is used for multiple virtual machines, they can communicate with each other via the network. 
Bridge adapter is for connecting the virtual network adapter of a VM to a physical network to which a physical network adapter of the VirtualBox host machine is connected.
Internal Network is when adapters configured to work in the VirtualBox Internal Network mode are connected to an isolated virtual network.
Host Only adapter is used for communicating between a host and guests.
A Generic Driver will allow you to share the generic network interface.
Port Forwarding is a process of intercepting traffic addressed to the appropriate IP address and port in addition to redirecting that traffic to a different IP address and/or port. 



https://www.nakivo.com/blog/virtualbox-network-setting-guide/
