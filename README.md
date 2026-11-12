# 🌐 Networking Fundamentals

![Networking](https://img.shields.io/badge/Subject-Networking-blue)
![Level](https://img.shields.io/badge/Level-Beginner%20to%20Intermediate-green)
![Focus](https://img.shields.io/badge/Focus-Cybersecurity-red)

## 📌 About This Repository

Welcome to my Networking Fundamentals repository.

This repository contains structured notes, practical commands, networking concepts, protocols, and hands-on examples designed to build a strong foundation in computer networking and cybersecurity.

The purpose of this repository is to understand how computer networks communicate, how data travels between devices, and how network infrastructure works.

---

# 📚 Table of Contents

1. Introduction to Networking
2. Types of Networks
3. Network Topologies
4. Network Devices
5. OSI Model
6. TCP/IP Model
7. IP Addressing
8. IPv4 and IPv6
9. Public and Private IP Addresses
10. Subnetting
11. MAC Address
12. TCP and UDP
13. Common Network Protocols
14. Common Port Numbers
15. DNS
16. DHCP
17. ARP
18. HTTP and HTTPS
19. Routing and Switching
20. Firewalls
21. VPN
22. Network Security
23. Common Networking Commands
24. Practical Networking Examples
25. Important Interview Questions

---

# 1. Introduction to Networking

Computer networking is the process of connecting two or more computers or devices to share information, resources, and services.

A network allows devices to communicate with each other through wired or wireless connections.

### Why Do We Need Networking?

- Sharing files and documents.
- Sharing printers and other hardware.
- Accessing the internet.
- Communicating through email and messaging.
- Sharing applications and databases.
- Managing systems remotely.
- Supporting cybersecurity operations.

### Real-World Example

When you open Google in your browser, your computer communicates with Google's servers through a network using different protocols.

---

# 2. Types of Networks

### LAN – Local Area Network

A LAN connects devices within a limited geographical area, such as a home, office, school, or laboratory.

Example: Computers connected through a home Wi-Fi router.

### WAN – Wide Area Network

A WAN connects networks across large geographical areas.

Example: The Internet.

### MAN – Metropolitan Area Network

A MAN connects multiple networks across a city or metropolitan area.

### PAN – Personal Area Network

A PAN connects personal devices over a short distance.

Example: A smartphone connected to Bluetooth headphones.

### WLAN – Wireless Local Area Network

A WLAN is a local network that uses wireless communication, usually Wi-Fi.

---

# 3. Network Topologies

Network topology describes how devices are connected within a network.

### Bus Topology
All devices share a single communication cable.

### Star Topology
All devices connect to a central switch or hub.

### Ring Topology
Devices connect in a circular arrangement.

### Mesh Topology
Devices have multiple connections to other devices, providing alternative communication paths.

### Tree Topology
Multiple star networks are connected in a hierarchical structure.

---

# 4. Network Devices

### Router
A router connects different networks and forwards packets between them using IP addresses.

### Switch
A switch connects devices within a LAN and forwards Ethernet frames using MAC addresses.

### Hub
A hub broadcasts incoming data to all connected ports.

### Modem
A modem converts signals to establish communication over an internet service provider's connection.

### Access Point
An access point allows wireless devices to connect to a wired network.

### Firewall
A firewall monitors and filters network traffic according to security rules.

---

# 5. OSI Model

The Open Systems Interconnection (OSI) model is a conceptual framework that explains how network communication works through seven layers.

| Layer | Name | Function |
|---|---|---|
| 7 | Application | Network services for applications |
| 6 | Presentation | Data formatting and encryption |
| 5 | Session | Manages communication sessions |
| 4 | Transport | End-to-end data delivery |
| 3 | Network | Logical addressing and routing |
| 2 | Data Link | MAC addressing and frames |
| 1 | Physical | Transmission of raw bits |

### Explanation of Each Layer

**Layer 7 – Application**

Provides network services to applications.

Examples: HTTP, FTP, DNS, SMTP.

**Layer 6 – Presentation**

Handles data formatting, encoding, compression, and encryption.

**Layer 5 – Session**

Establishes, manages, and terminates communication sessions.

**Layer 4 – Transport**

Provides communication between devices using TCP and UDP.

**Layer 3 – Network**

Handles logical addressing and routing using IP addresses.

**Layer 2 – Data Link**

Handles Ethernet frames and MAC addresses.

**Layer 1 – Physical**

Transmits raw binary data through cables, radio signals, and other physical media.

### OSI Layer Memory Trick

From Layer 7 to Layer 1:

All People Seem To Need Data Processing.

---

# 6. TCP/IP Model

The TCP/IP model explains how devices communicate over modern networks.

It commonly consists of four layers.

| TCP/IP Layer | Main Function | Examples |
|---|---|---|
| Application | Application-level communication | HTTP, DNS, FTP |
| Transport | End-to-end communication | TCP, UDP |
| Internet | IP addressing and routing | IPv4, IPv6, ICMP |
| Network Access | Local network transmission | Ethernet, Wi-Fi |

### OSI vs TCP/IP

The OSI model has seven layers, while the commonly used TCP/IP model has four layers.

The OSI model is mainly used as a conceptual reference, while TCP/IP describes the practical Internet protocol architecture.

---

# 7. IP Addressing

An IP address is a logical address assigned to a network interface to identify it within an IP network.

Example:

`192.168.1.10`

An IPv4 address contains 32 bits and is represented using four decimal octets.

Example:

`192.168.1.10`

Each octet can have a value from 0 to 255.

### IPv4 Address Classes

| Class | First Octet Range | Traditional Default Mask |
|---|---|---|
| A | 1–126 | 255.0.0.0 |
| B | 128–191 | 255.255.0.0 |
| C | 192–223 | 255.255.255.0 |
| D | 224–239 | Multicast |
| E | 240–255 | Experimental |

Note: Classful addressing is historical. Modern networks use CIDR.

### IP Address Components

An IP address contains:

- Network portion.
- Host portion.

The subnet mask determines which bits identify the network and which identify the host.

---

# 8. IPv4 and IPv6

### IPv4

- Uses 32-bit addresses.
- Written in dotted-decimal format.
- Example: `192.168.1.1`
- Provides approximately 4.3 billion possible addresses.

### IPv6

- Uses 128-bit addresses.
- Written in hexadecimal format.
- Example: `2001:db8::1`
- Provides a vastly larger address space.

### Main Differences

| Feature | IPv4 | IPv6 |
|---|---|---|
| Address Size | 32 bits | 128 bits |
| Format | Decimal | Hexadecimal |
| Address Space | Smaller | Extremely large |
| Broadcast | Supported | Not supported |
| Example | 192.168.1.1 | 2001:db8::1 |

---

# 9. Public and Private IP Addresses

### Public IP

A public IP address is globally routable on the Internet.

It is generally assigned to an internet-facing network interface by an ISP or another address provider.

### Private IP

Private IP addresses are used inside local networks and are not directly routable across the public Internet.

Private IPv4 ranges:

| Range | CIDR |
|---|---|
| 10.0.0.0 – 10.255.255.255 | 10.0.0.0/8 |
| 172.16.0.0 – 172.31.255.255 | 172.16.0.0/12 |
| 192.168.0.0 – 192.168.255.255 | 192.168.0.0/16 |

---

# 10. Subnetting

Subnetting is the process of dividing a larger IP network into smaller logical networks.

### Why Is Subnetting Important?

- Efficient IP address management.
- Better network organization.
- Reduced broadcast domains.
- Improved network security and segmentation.
- Efficient use of IP addresses.

### Subnet Mask

A subnet mask identifies the network portion and host portion of an IPv4 address.

Example:

IP Address: `192.168.1.10`

Subnet Mask: `255.255.255.0`

CIDR: `/24`

### Important CIDR Values

| CIDR | Subnet Mask | Total Addresses |
|---|---|---|
| /8 | 255.0.0.0 | 16,777,216 |
| /16 | 255.255.0.0 | 65,536 |
| /24 | 255.255.255.0 | 256 |
| /25 | 255.255.255.128 | 128 |
| /26 | 255.255.255.192 | 64 |
| /27 | 255.255.255.224 | 32 |
| /28 | 255.255.255.240 | 16 |
| /29 | 255.255.255.248 | 8 |
| /30 | 255.255.255.252 | 4 |

For conventional IPv4 subnets, usable host addresses are generally total addresses minus two (network and broadcast addresses). Special cases exist.

### Subnetting Example

Network: `192.168.1.0/24`

Divide into four equal subnets.

New prefix: `/26`

| Subnet | Network Address | Usable Host Range | Broadcast |
|---|---|---|---|
| 1 | 192.168.1.0 | .1 – .62 | .63 |
| 2 | 192.168.1.64 | .65 – .126 | .127 |
| 3 | 192.168.1.128 | .129 – .190 | .191 |
| 4 | 192.168.1.192 | .193 – .254 | .255 |

Each subnet contains 64 total addresses and 62 traditionally usable host addresses.

---

# 11. MAC Address

MAC stands for Media Access Control.

A MAC address is a link-layer address used to identify a network interface on a local network.

Example:

`00:1A:2B:3C:4D:5E`

### Important Points

- Common Ethernet MAC addresses are 48 bits.
- MAC addresses are used at the Data Link layer.
- Switches use MAC addresses to forward Ethernet frames.
- IP addresses are used for logical addressing and routing.

---

# 12. TCP and UDP

TCP and UDP are transport-layer protocols.

### TCP – Transmission Control Protocol

TCP provides reliable, connection-oriented communication.

Features:

- Connection establishment.
- Reliable data delivery.
- Acknowledgments.
- Retransmission of lost data.
- Ordered delivery.

Example: HTTPS, SSH, and FTP control connections commonly use TCP.

### UDP – User Datagram Protocol

UDP provides connectionless communication with lower protocol overhead.

Features:

- No connection establishment.
- No built-in delivery guarantee.
- No built-in retransmission.
- No guarantee of packet ordering.

Example: DNS queries, VoIP, and many real-time applications use UDP.

### TCP vs UDP

| Feature | TCP | UDP |
|---|---|---|
| Connection | Connection-oriented | Connectionless |
| Reliability | Built-in | Not guaranteed |
| Ordering | Yes | Not guaranteed |
| Overhead | Higher | Lower |
| Common Uses | HTTPS, SSH | DNS, VoIP |

---

# 13. Common Network Protocols

| Protocol | Purpose |
|---|---|
| HTTP | Web communication |
| HTTPS | Encrypted web communication |
| FTP | File transfer |
| SFTP | Secure file transfer over SSH |
| SSH | Secure remote administration |
| Telnet | Remote terminal communication |
| DNS | Domain name resolution |
| DHCP | Automatic IP configuration |
| SMTP | Sending email |
| POP3 | Receiving email |
| IMAP | Accessing and synchronizing email |
| SMB | Network file and printer sharing |
| RDP | Remote Desktop access |
| SNMP | Network device monitoring |
| ICMP | Network diagnostics and error reporting |
| NTP | Time synchronization |
| LDAP | Directory services |
| Kerberos | Network authentication |
| TLS | Cryptographic security for communication |

---

# 14. Common Port Numbers

A port identifies a service or application endpoint associated with a transport protocol.

| Port | Protocol | Service |
|---|---|---|
| 20 | TCP | FTP Data |
| 21 | TCP | FTP Control |
| 22 | TCP | SSH |
| 23 | TCP | Telnet |
| 25 | TCP | SMTP |
| 53 | TCP/UDP | DNS |
| 67/68 | UDP | DHCP |
| 69 | UDP | TFTP |
| 80 | TCP | HTTP |
| 88 | TCP/UDP | Kerberos |
| 110 | TCP | POP3 |
| 123 | UDP | NTP |
| 135 | TCP | MS RPC |
| 139 | TCP | NetBIOS |
| 143 | TCP | IMAP |
| 161/162 | UDP | SNMP |
| 389 | TCP/UDP | LDAP |
| 443 | TCP | HTTPS |
| 445 | TCP | SMB |
| 465 | TCP | SMTPS |
| 587 | TCP | SMTP Submission |
| 636 | TCP | LDAPS |
| 993 | TCP | IMAPS |
| 995 | TCP | POP3S |
| 1433 | TCP | Microsoft SQL Server |
| 3306 | TCP | MySQL |
| 3389 | TCP/UDP | RDP |
| 5432 | TCP | PostgreSQL |
| 5900 | TCP | VNC |
| 8080 | TCP | Alternative HTTP |

Note: A service can be configured to use a non-standard port.

---

# 15. DNS – Domain Name System

DNS translates domain names into IP addresses.

Example:

`google.com` → IP address

Without DNS, users would need to remember IP addresses instead of domain names.

### Common DNS Record Types

| Record | Purpose |
|---|---|
| A | Maps a name to an IPv4 address |
| AAAA | Maps a name to an IPv6 address |
| CNAME | Alias for another domain name |
| MX | Mail server information |
| NS | Authoritative name server |
| TXT | Text information and verification |
| PTR | Reverse DNS lookup |

### Practical DNS Command

```bash
nslookup google.com
```

Another useful command:

```bash
dig google.com
```

---

# 16. DHCP – Dynamic Host Configuration Protocol

DHCP automatically assigns network configuration to devices.

It can provide:

- IP address.
- Subnet mask.
- Default gateway.
- DNS server addresses.
- Lease information.

### DORA Process

DHCP commonly uses four steps:

1. Discover – Client searches for a DHCP server.
2. Offer – Server offers an IP configuration.
3. Request – Client requests the offered configuration.
4. Acknowledge – Server confirms the lease.

---

# 17. ARP – Address Resolution Protocol

ARP resolves an IPv4 address to a MAC address on a local network.

Example:

A computer wants to communicate with another device on its local network.

It knows the destination IP address but needs the corresponding MAC address.

ARP helps discover that MAC address.

### Practical Command

```cmd
arp -a
```

This displays the local ARP cache.

---

# 18. HTTP and HTTPS

### HTTP

Hypertext Transfer Protocol is used for communication between web clients and web servers.

Default port: 80/TCP.

### HTTPS

HTTPS uses HTTP over TLS to provide encrypted communication and server authentication.

Default port: 443/TCP.

### HTTP Methods

| Method | Purpose |
|---|---|
| GET | Retrieve a resource |
| POST | Submit data |
| PUT | Create or replace a resource |
| PATCH | Partially update a resource |
| DELETE | Delete a resource |
| HEAD | Retrieve response headers |
| OPTIONS | Discover supported methods |

---

# 19. Routing and Switching

### Routing

Routing is the process of forwarding packets between different IP networks.

Routers use routing tables to determine the next hop or outgoing interface.

### Switching

Switching forwards Ethernet frames within a local network.

Switches commonly learn MAC addresses and store them in a MAC address table.

### Routing vs Switching

| Routing | Switching |
|---|---|
| Uses IP addressing | Uses MAC addressing |
| Connects different networks | Connects devices within a LAN |
| Mainly Layer 3 | Mainly Layer 2 |

---

# 20. Firewalls

A firewall is a security system that monitors and controls incoming and outgoing network traffic according to configured rules.

### Types of Firewalls

- Packet-filtering firewall.
- Stateful firewall.
- Proxy firewall.
- Next-Generation Firewall (NGFW).
- Web Application Firewall (WAF).

### Firewall Functions

- Block unauthorized traffic.
- Allow approved network connections.
- Filter traffic by IP and port.
- Monitor network activity.
- Enforce security policies.

---

# 21. VPN – Virtual Private Network

A VPN creates an encrypted tunnel between a device and a VPN endpoint or network.

### Benefits

- Protects traffic over untrusted networks.
- Enables secure remote access.
- Connects geographically separated networks.
- Helps protect data confidentiality.

### Common VPN Technologies

- OpenVPN.
- WireGuard.
- IPsec.
- IKEv2.

---

# 22. Network Security

Network security involves protecting network infrastructure, devices, applications, and data against unauthorized access and attacks.

### Common Network Threats

**1. DoS – Denial of Service**

Attempts to make a service unavailable by overwhelming or disrupting it.

**2. DDoS – Distributed Denial of Service**

A denial-of-service attack launched from multiple systems.

**3. MITM – Man-in-the-Middle**

An attacker positions themselves between communicating parties to intercept or potentially modify traffic.

**4. ARP Spoofing**

An attacker sends forged ARP messages to manipulate IP-to-MAC address mappings.

**5. DNS Spoofing**

An attacker manipulates DNS responses to redirect users to unintended destinations.

**6. Packet Sniffing**

Capturing and analyzing network traffic.

**7. Port Scanning**

Identifying open, closed, or filtered network ports.

### Basic Security Practices

- Use strong authentication.
- Keep operating systems updated.
- Use firewalls.
- Encrypt sensitive communication.
- Disable unnecessary services.
- Monitor network traffic.
- Apply network segmentation.
- Use secure protocols such as SSH and HTTPS.

---

# 23. Common Networking Commands

These commands are useful for network troubleshooting and security assessments.

### Windows Commands

**1. ipconfig**

Displays IP configuration.

```cmd
ipconfig
```

**2. ipconfig /all**

Displays detailed network configuration.

```cmd
ipconfig /all
```

**3. ping**

Tests connectivity to another host.

```cmd
ping 8.8.8.8
```

**4. tracert**

Displays the route taken by packets.

```cmd
tracert google.com
```

**5. nslookup**

Queries DNS information.

```cmd
nslookup google.com
```

**6. netstat**

Displays network connections and listening ports.

```cmd
netstat -ano
```

**7. arp**

Displays the ARP cache.

```cmd
arp -a
```

**8. route**

Displays the IP routing table.

```cmd
route print
```

### Linux Commands

**1. ip addr**

Displays network interfaces and IP addresses.

```bash
ip addr
```

**2. ip route**

Displays the routing table.

```bash
ip route
```

**3. ping**

Tests network connectivity.

```bash
ping -c 4 8.8.8.8
```

**4. traceroute**

Traces the network path.

```bash
traceroute google.com
```

**5. ss**

Displays socket information.

```bash
ss -tulnp
```

**6. dig**

Performs DNS queries.

```bash
dig google.com
```

**7. ip neigh**

Displays the neighbor cache.

```bash
ip neigh
```

**8. nmap**

Scans hosts and services on authorized networks.

```bash
nmap -sV 192.168.1.1
```

---

# 24. Practical Networking Examples

### Example 1: Check Your IP Address

Windows:

```cmd
ipconfig
```

Linux:

```bash
ip addr
```

### Example 2: Test Internet Connectivity

```cmd
ping 8.8.8.8
```

### Example 3: Check DNS Resolution

```cmd
nslookup google.com
```

### Example 4: View Active Connections

Windows:

```cmd
netstat -ano
```

Linux:

```bash
ss -tunap
```

### Example 5: Identify Open Ports

Only scan systems for which you have authorization.

```bash
nmap -sV 192.168.1.1
```

---

# 25. Important Interview Questions

**Q1. What is computer networking?**

Computer networking is the connection of two or more devices to communicate and share resources.

**Q2. What is the OSI model?**

The OSI model is a seven-layer conceptual framework used to understand network communication.

**Q3. How many layers are in the OSI model?**

Seven layers.

**Q4. What is the difference between TCP and UDP?**

TCP provides reliable, connection-oriented communication, while UDP provides connectionless communication without built-in delivery guarantees.

**Q5. What is an IP address?**

An IP address is a logical address used to identify a network interface within an IP network.

**Q6. What is a MAC address?**

A MAC address is a link-layer address used to identify a network interface on a local network.

**Q7. What is DNS?**

DNS translates domain names into IP addresses.

**Q8. What is DHCP?**

DHCP automatically provides IP configuration to network clients.

**Q9. What is subnetting?**

Subnetting divides a larger IP network into smaller logical networks.

**Q10. What is a default gateway?**

A default gateway is the router or network device used to forward traffic to destinations outside the local network.

**Q11. What is a firewall?**

A firewall monitors and filters network traffic according to security rules.

**Q12. What is the difference between a router and a switch?**

A router forwards packets between networks, while a switch forwards frames within a local network.

**Q13. What is a port number?**

A port number identifies a service or application endpoint associated with a transport protocol.

**Q14. What is HTTPS?**

HTTPS is HTTP protected by TLS encryption and authentication.

**Q15. What is ARP?**

ARP resolves IPv4 addresses into MAC addresses on a local network.

---

# 🎯 Learning Objectives

After studying these topics, I aim to understand:

- Fundamental networking concepts.
- OSI and TCP/IP models.
- IPv4 and IPv6 addressing.
- Subnetting and CIDR.
- TCP and UDP communication.
- Common network protocols and ports.
- DNS, DHCP, and ARP.
- Network troubleshooting.
- Basic network security.
- Practical Windows and Linux networking commands.

---

# 🛠️ Tools Used for Learning

- Wireshark – Network protocol analysis.
- Nmap – Network discovery and port scanning.
- Packet Tracer – Network simulation.
- Kali Linux – Cybersecurity learning environment.
- Windows CMD – Network troubleshooting.
- PowerShell – Windows network administration.

---

# 📖 Learning Resources

- [Cisco Networking Academy](https://www.netacad.com/)
- [CompTIA Network+](https://www.comptia.org/certifications/network)
- [Cloudflare Learning Center](https://www.cloudflare.com/learning/)
- [Microsoft Learn](https://learn.microsoft.com/)
- [Wireshark Documentation](https://www.wireshark.org/docs/)
- [Nmap Documentation](https://nmap.org/book/man.html)

---

# ⚠️ Disclaimer

This repository is intended for educational purposes and authorized cybersecurity training only.

All practical testing and network scanning should be performed on systems and networks for which proper authorization has been obtained.

---

## 👨‍💻 Author

**Muhammad Ahsan**

Cybersecurity Student | Networking Enthusiast | Aspiring Security Professional

This repository represents my learning journey in Computer Networking and Cybersecurity.

⭐ If you find these notes useful, feel free to star this repository.
