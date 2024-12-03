# MTProto Proxy Auto Installer
A very small script to install MTProtoProxy On Centos or Ubuntu

## Why this installer?
* Generate random secret
* Scripts for all proxy servers
* Automatically configure firewall
* Create a service to run it on background and start up
* Choose between Official Proxy, Python Proxy and Erlang Proxy
* Easy to setup
* Revoke and add secrets after install
* Supports Centos 7/8 or Ubuntu 18 or later and Debian 10 or later
* Automatically configure NTP
* API Support [[Reference](https://github.com/o-k-l-l/MTProtoProxyInstaller/wiki/API-For-Python-Script)]
## Official Or Python Proxy?
Use python if:
1. Your server's CPU has one core or you want to run proxy on one core.
2. Your server is low-end.
3. You are serving a small group of people. (Like family or small company)
4. You want to limit user connections.
5. You also have another application or service running on your server. (Openvpn, shadowsocks, nginx or ...)

Otherwise, use official proxy.
#### Performance?
Python proxy says it can serve about 4000 concurrent connections with 1 CPU core (~2.5 GHz) and 1024MB RAM.

Official proxy can serve about 10000 to 16000 connections per core.
```bash
curl -o MTProtoProxyOfficialInstall.sh -L https://github.com/o-k-l-l-a/MTProtoProxyInstaller/raw/refs/heads/master/MTProtoProxyOfficialInstall.sh && bash MTProtoProxyOfficialInstall.sh
```

