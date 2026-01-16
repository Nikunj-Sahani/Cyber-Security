<h1 align="center">📧 DNS in Detail 📧</h1>

---
## DNS - Domain Name System
DNS converts website names into IP addresses so computers can find each other.

- [X] When we search **Google.com - Convert to IP - Show Google.com in Browser.**

- [ ] 👉 DNS is a naming system of the internet.
- [ ] 👉 Humans remember names like google.com
- [ ] 👉 Computers understand numbers like 142.250.190.14

### Why DNS is Needed

 - Computers use IP addresses, not names
 - DNS removes the need to remember numeric IPs
 - Enables fast and scalable internet communication

### How DNS Works (Step-by-Step)

 - 1️⃣ User enters a website name (e.g., www.example.com)
 - 2️⃣ Browser checks local cache
 - 3️⃣ If not found, request goes to Recursive DNS Resolver
 - 4️⃣ Resolver asks:
   
    > - Root DNS Server
    > - TLD Server (.com, .org)
    > - Authoritative DNS Server

- 5️⃣ IP address is returned to the browser
- 6️⃣ Browser connects to the web server using that IP

### Types of DNS Servers

| Server Type          | Role                            |
| -------------------- | ------------------------------- |
| Recursive Resolver   | Finds IP on behalf of user      |
| Root Server          | Directs to TLD server           |
| TLD Server           | Directs to authoritative server |
| Authoritative Server | Stores actual DNS records       |

### Common DNS records include:

   > - **A Record –** Maps a domain to an IPv4 address

   > - **AAAA Record –** Maps a domain to an IPv6 address

   > - **CNAME –** Alias of one domain to another

   > - **MX Record –** Specifies mail servers for the domain

   > - **NS Record –** Indicates authoritative name servers

   > - **TXT Record –** Stores text data (often used for verification and security)

### DNS Ports & Protocol

UDP 53 → Normal queries (fast)

TCP 53 → Large responses, zone transfers
