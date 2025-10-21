### How to get the User flag?
This machine doesn’t have a guided mode. There are only two fields: one for the user flag and one for the root flag. Other than the IP address, no information is given, so the idea is probably to start with a port scan. When I scanned the TCP ports using rustscan or nmap, only port 22 (SSH) was open. Since rustscan doesn’t support UDP scans, I used nmap instead, and it showed more open ports on UDP.

```
┌──(kali㉿kali)-[~/Templates]
└─$ nmap -sU --top-ports 100 10.10.11.87
Starting Nmap 7.95 ( https://nmap.org ) at 2025-10-21 02:35 EDT
Nmap scan report for 10.10.11.87
Host is up (0.83s latency).
Not shown: 92 closed udp ports (port-unreach)
PORT      STATE         SERVICE
53/udp    open|filtered domain
68/udp    open|filtered dhcpc
69/udp    open|filtered tftp
500/udp   open          isakmp
4500/udp  open|filtered nat-t-ike
32769/udp open|filtered filenet-rpc
49153/udp open|filtered unknown
49194/udp open|filtered unknown

Nmap done: 1 IP address (1 host up) scanned in 193.41 seconds
```

### How to get the Root flag?
Empty

### Ref
- Target : https://app.hackthebox.com/machines/Expressway
