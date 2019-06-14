# shadownet-compose
A docker-compose file to create a VPN and socks5 proxy stack

Requirements
------------
- [Docker-compose](https://docs.docker.com/compose/install/) 
- Domain name and [dns provider account](https://github.com/Neilpang/acme.sh/wiki/dnsapi) (GoDaddy for example)

Quick Start
-----------
1) Replace environment variables with your values:
    - GD_Key=`GODADDY_KEY`
    - GD_Secret=`GODADDY_SECRET`
    - PROXY_SECRET=`user1:P@ssw0rd1,user2:P@ssw0rd2`
    - OC_SECRET=`user1:P@ssw0rd1,user2:P@ssw0rd2`
2) Change domain name from `example.com` to your value in all entries.

Start deply:
```
$ docker-compose up -d
```
