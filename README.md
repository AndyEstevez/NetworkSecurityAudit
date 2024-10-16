# Network Security Audit
- Use Nmap to discover open ports on TCP or UDP for your private/public IP address
- Learn what those ports are for in your network
- Use Nessus for vulnerability scanning on your IP address
- Solve and fix vulnerabilities in your network

### Download
- Nmap: https://nmap.org/download.html
- Nessus: https://www.tenable.com/downloads/nessus
  - When installing Nessus, select Nessus Essentials and register to get activation code

## Using NMAP
1. Used Zenmap program to do a quick scan on my private IP to view my non-closed TCP ports
   - Msrpc on port 135, which is a protocol for being a interface between programs to request a service.
   - Netbios-ssn on port 139, which is a protocol for File & Printer Sharing.
   - Microsoft-ds on port 445, which is for sharing resources like files/printers on SMB. *This will become important later*
   - MySQL on port 3306, which is used to connect to databases.

<img src="images/01-NMAP_on_privateIPv4.png" height='auto' width='auto'/>

2. Now, this is for my public IP non-closed TCP ports
   - SSH on port 22, this is for creating secured network connection through encryption between devices.
   - Domain on port 53, this is the DNS server, which translates names to IP addresses. Ex: www.google.com -> 142.250.176.206
   - The remaining services are for Http/Https/http-proxy/https-alt, which relates to a client communicating and receive info from server.
 Filtered means that a firewall, filter, or other network obstacle is blocking the port so that Nmap cannot tell whether it is open or closed.
<img src="images/01-NMAP_on_publicIPv4.png" height='auto' width='auto'/>

3. The open state for a port means its looking for connections on that port. The filtered state for a port means a firewall is blocking the port.
4. Therefore, my computer is looking for connections to connect to databases, file or print sharing, communicating with servers, and translating domain names to IP addresses. Also, my SSH is filtered by my firewall which is being done by Windows Firewall.


## Using Nessus

## Vulnerability Researched & Fixed
  
