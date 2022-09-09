Gary King
09/09/2022
Class 9 Reading Notes
CIDR Block Notation 
https://medium.com/@ethicalentrepreneur/cidr-block-notation-explained-in-2-minutes-1010ec0dbc15

CIDR notation is a way of representing a CIDR block which is a range of IP Addresses.
When a network is created the aim is to have enough IP addresses for you to use without making the CDR block too large or wasteful.
An IPv4 (version 4 of IP) address is usually represented as four 8-bit decimal numbers or octets separated by dots, for example 127.0.0.1 (localhost on most systems). An 8-bit number when represented in the decimal system as opposed to binary has a range of 0–255.
If we wanted a smaller range (say half of the example just given) we would write 10.0.0.0/17, which would give us a range of 32,768 (or 2¹⁵) IP addresses.
As you can see, the larger the mask, the smaller the range. So 10.0.0.0/24 will give us a range of 10.0.0.0–10.0.0.255, which is just 256 (or 2⁸) IP addresses.

What Is Network Segmentation
https://www.comptia.org/blog/security-awareness-training-network-segmentation

Network segmentation is when different parts of a computer network, or network zones, are separated by devices like bridges, switches and routers.
The following are a few key benefits of network segmentation:
Limiting access privileges to those who truly need it.
Protecting the network from widespread cyberattacks.
Boosting network performance by reducing the number of users in specific zones.

If network segmentation is set up then when the hackers try find a way in thats when they will find an obstacle. It's like turning a corner within a hedge maze to find a dead end: the threat hacker will have to work their way backward and attempt to find other access points to the systems and data they are attempting to compromise.
Here are some examples of the types of network zones you may want to establish:
Users: Users are a network in and of themselves. Make sure you have correct access control on your users in your active directory. Who needs the least privilege on your network? Privilege levels should be based on the user’s role in switching administration. How many admins have full access rights? Make sure you have less than a handful. Access control lists are typically already a part of your active directory server. The idea here is you are extending that practice to more components of your network.
Screened Subnet: This includes the subnetworks that expose externally facing systems – where the handshakes take place on your network. For example, it may include public-facing websites or other resources accessible via the internet. You want to separate things that the public can access from your local area network (LAN) and internal data that needs to be protected.
Guest Network: Guest Wi-Fi should be separate from the corporate Wi-Fi. This may seem like a no brainer, but I find a lot of smaller businesses never bother to set it up. Even residential routers include this feature – you can easily set up a guest Wi-Fi in your home!
IT Workstations: This is the dev network zone for IT. It’s where your IT staff does non-administrative work, and it should be segmented for testing. I would also recommend giving IT a dedicated internet circuit for testing. This can be a best effort, cheaper connection. Don’t let anyone else in the company have network access to it aside from IT.
Servers by Department: Do department servers need to talk to one another? Create a public drive and a private drive, and then segment access on the private drives to those within each team or department. This can limit the crawl of malware.
VoIP/Communications: Placing communications systems on their own network zone boosts performance and enhances quality. But in terms of network security, as communications move toward more APIs unique to your most used software as a service (SaaS) platforms, this network will become a more common attack surface.
Traditional Physical Security: Cameras, ID card scanners, etc., should be in their own network zone. This is not to be taken lightly, as the risk of a physical breach can be more harmful than a digital one. There are a number of real-world examples of this, including in 2017, the closed-circuit camera network in Washington, D.C., was hacked, leaving police cameras unable to function for three days.
Industrial Control Systems: HVAC, for example, like the non-segmented network compromised in the Target breach, should have two-factor authentication and be segmented.
Customer Databases: Due to compliance requirements, customer databases need to be secured more intently than, for instance, your print server. PCI-DSS, HIPAA, HiTRUST, FINRA, GDPR and other pieces of data legislation will determine the level of segmentation and cybersecurity that would be best practice in terms of implementation.
While safety and security are critical benefits unto themselves, the following are also excellent advantages when it comes to network segmentation:
Damage control and limitation in case of an incident via the smaller attack surface
Improved access control for external and internal network security
Reducing the attack plane and scope of compliance requirements related auditing
Improved performance with less congestion on network traffic
Better analytics around network monitoring, network access and network devices
Endpoint device protection, especially important as IoT devices become more common
