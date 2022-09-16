Gary King 
09/16/2022
Class 14 Reading Notes
Network scanning with NMAP
https://www.varonis.com/blog/port-scanning-techniques
A port scanner is a computer program that checks network ports for one of three possible statuses – open, closed, or filtered.
Port scanners are good in diagnosing network and connectivity issues. Attackers use port scanners to detect possible access points for infiltration and to identify what kinds of devices you are running on the network.
A port scanner sends a network request to connect to a specific TCP or UDP port on a computer and records the response.
A computer has an Internet Protocol (IP) address, which is how the network knows which computer to send packets to. If you send a packet to the IP address, the computer knows what port to route the packet to based on the application or packet contents. Each service running on the computer needs to “listen” on a designated port.
A port scanner sends a TCP or UDP network packet and asks the port about their current status. The three types of responses are below:
1 Open, Accepted: The computer responds and asks if there is anything it can do for you.
2 Closed, Not Listening: The computer responds that “This port is currently in use and unavailable at this time.”
3 Filtered, Dropped, Blocked: The computer doesn’t even bother to respond.

Port scans generally occur early in the cyber kill chain, during reconnaissance and intrusion. Attackers use port scans to detect targets with open and unused ports that they can repurpose for infiltration, command and control, and data exfiltration or discover what applications run on that computer to exploit a vulnerability in that application.
PING Scanner is sending PING requests ,Ping scans aren’t technically port scanning techniques, as the best you can get back is that there is a computer on the other end, but it’s related and usually the first task before you do a port scan. 
A popular port scanning technique is the TCP half-open port scan, sometimes referred to as an SYN scan. It’s a fast and sneaky scan that tries to find potential open ports on the target computer.
Any SYN-ACK responses are possibly open ports. An RST(reset) response means the port is closed, but there is a live computer here. No responses indicate SYN is filtered on the network. An ICMP (or ping) no response also counts as a filtered response.
TCP half-open scans are the default scan in NMAP.
A TCP connectis basically the same as the TCP Half-Open scan, but instead of leaving the target hanging, the port scanner completes the TCP connection.

UDP scans work best when you send a specific payload to the target. For example, if you want to know if a DNS server is up, you would send a DNS request. For other UDP ports, the packet is sent empty. An ICMP unreachable response means the port is closed or filtered. If there is a service running, you might get a UDP response, which means the port is open. No response could mean that the port is open or filtered.
