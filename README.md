### How to get the User flag?
This machine doesn’t have a guided mode. There are only two fields: one for the user flag and one for the root flag. Other than the IP address, no information is given, so the idea is probably to start with a port scan. When I scanned the TCP ports using rustscan or nmap, only port 22 (SSH) was open. Since rustscan doesn’t support UDP scans, I used nmap instead, and it showed more open ports on UDP.

### How to get the Root flag?
Empty

### Ref
- Target : https://app.hackthebox.com/machines/Expressway
