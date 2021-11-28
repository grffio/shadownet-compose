# shadownet-compose
A docker-compose file to create a VPN and socks5 proxy stack

Requirements
------------
- [Docker-compose](https://docs.docker.com/compose/install/) 
- Domain name: `example.com`

Quick Start
-----------
Caddy is used to issue certificates to ocserv, can be used as a reverse proxy for other services.
1) Replace secret environment variables with your values, for example:
    - PROXY_SECRET=`user1:P@ssw0rd1,user2:P@ssw0rd2`
    - OC_SECRET=`user1:P@ssw0rd1,user2:P@ssw0rd2`
2) Change domain name from `example.com` to your value in all entries.
3) Create /opt/caddy/Caddyfile: `example.com {}`

Start deply:
```
$ docker-compose up -d
```
