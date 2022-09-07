Gary King
09/05/2022
Class o7 Reading Notes
Web Server Deployment
NGINX is for open source software web serving, reverse proxy, caching, load balancing, media and streaming.
NGINX can also be used to as a email proxy for email systems (IMAP, POP3 & SMTP).

When NGINX was designed it was design to be the fastest web server around and that is still a goal of NGINX.
NGINX now supports all the components of the modern web, including WebSocket, HTTP/2, gRPC, and streaming of multiple video formats (HDS, HLS, RTMP)

NGINX is most commonly used as a reverse proxy and load balancer to manage incoming traffic and distribute it to slower upstream servers – anything from legacy database servers to microservices.
A lot of times NGINX will be put between clients and a second web server to serve as an SSL/TLS terminator or web accelerator.
As an intermediary NGINX can handle task that could slow down a web server such as negotiating SSL/TLS or compressing and caching content.
