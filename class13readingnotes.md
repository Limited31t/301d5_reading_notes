Gary King
09/15/2022
Class 13 reading notes
Traffic Mirroring
https://accedian.com/blog/capture-network-traffic-span-vs-tap/

Port Mirroring is also known as SPAN  or roving analysis and is a method of monitoring network traffic.
This traffic is forwarded as a copy of each incoming and/or outgoing packet from one (or several) port(s) (or VLAN) of a switch to another port where the analysis device is connected.
The administrator can include either all packets in the port mirroring or only the transmitted /received packets. In case both transmitted and received packets are included, a packet going from a first monitored port to another monitored port will be copied twice to the destination port.
Port mirroring is the most commonly used solution for capturing traffic because it is inexpensive, flexible in terms of how much traffic can be captured at once, and remotely configurable.
Port mirroring can have drawbacks like consuming your CPU, there is a risk of not receiving packets, traffic congestion.
One solution to long term monitoring could be a passive TAP or an ethernet repeater.
Some advantages to mirroring are low cost to perform, and can be configured remotely.
Some drawbacks are if it is not fully utilized it may have dropped packets,filters out physical errors,an impact on the switches CPU.
The network TAP has at least three ports: an A port, a B port, and a monitor port. To place a tap between points A and B, the network cable between point A and point B is replaced with a pair of cables, one going to the TAP’s A port, the other one going to the TAP’s B port. The TAP passes all traffic between the two network points, so they are still connected to each other. The TAP also copies the traffic to its monitor port, thus enabling an analysis device to listen.
