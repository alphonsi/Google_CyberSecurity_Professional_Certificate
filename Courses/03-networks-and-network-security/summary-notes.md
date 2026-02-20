# Networks and Network Security - Summary Notes (Google Cybersecurity Professional Certificate)

## Module 1: Introduction to Networks

### What is a Network?
A network is a collection of interconnected devices (computers, servers, routers, switches) that communicate with each other to share resources and information. Networks are essential for modern organizations to function efficiently.

### Types of Networks
- **LAN (Local Area Network)**: Covers a small geographic area (e.g., office, school)
- **WAN (Wide Area Network)**: Covers a large geographic area (e.g., multiple offices, cities)
- **MAN (Metropolitan Area Network)**: Covers a city or metropolitan area
- **PAN (Personal Area Network)**: Covers a small area around an individual (e.g., smartphone, laptop)

### Network Topologies
- **Star**: All devices connect to a central hub or switch
- **Mesh**: Each device connects directly to every other device
- **Bus**: All devices connect to a single central cable
- **Ring**: Devices connect in a circular loop

### Network Addressing and Routing
- **IP Addressing**: Assigns a unique identifier to each device on a network
- **IPv4**: 32-bit address (e.g., 192.168.1.1)
- **IPv6**: 128-bit address (e.g., 2001:0db8:85a3:0000:0000:8a2e:0370:7334)
- **Routing**: Process of forwarding packets from source to destination

## Module 2: Network Fundamentals

### OSI Model
The Open Systems Interconnection (OSI) model is a conceptual framework that standardizes communication functions into 7 layers:

1. **Physical Layer**: Deals with physical transmission of data
2. **Data Link Layer**: Handles data framing and error detection
3. **Network Layer**: Handles packet routing and addressing
4. **Transport Layer**: Provides reliable data transfer (TCP) or unreliable (UDP)
5. **Session Layer**: Manages communication sessions
6. **Presentation Layer**: Handles data formatting and encryption
7. **Application Layer**: Provides network services to applications

### TCP/IP Model
A practical implementation of network communication with 4 layers:

1. **Link Layer**: Physical and data link functions
2. **Internet Layer**: IP addressing and routing
3. **Transport Layer**: TCP and UDP protocols
4. **Application Layer**: Application protocols (HTTP, FTP, DNS, etc.)

## Module 3: Network Protocols

### TCP and UDP
- **TCP (Transmission Control Protocol)**: Reliable, connection-oriented protocol
- **UDP (User Datagram Protocol)**: Unreliable, connectionless protocol

### IP Addressing
- **IPv4**: 32-bit addresses (4.3 billion possible addresses)
- **IPv6**: 128-bit addresses (3.4 × 10³⁸ possible addresses)
- **Subnetting**: Dividing a network into smaller subnetworks
- **CIDR (Classless Inter-Domain Routing)**: Variable-length subnet masking

### DNS and DHCP
- **DNS (Domain Name System)**: Translates domain names to IP addresses
- **DHCP (Dynamic Host Configuration Protocol)**: Automatically assigns IP addresses to devices

### HTTP/HTTPS
- **HTTP (Hypertext Transfer Protocol)**: Unencrypted web communication
- **HTTPS (Hypertext Transfer Protocol Secure)**: Encrypted web communication using SSL/TLS

## Module 4: Network Devices

### Routers and Switches
- **Router**: Forwards packets between networks
- **Switch**: Forwards packets within a network

### Firewalls and IDS/IPS
- **Firewall**: Filters network traffic based on security rules
- **IDS (Intrusion Detection System)**: Detects security incidents
- **IPS (Intrusion Prevention System)**: Detects and prevents security incidents

### Load Balancers and Proxies
- **Load Balancer**: Distributes network traffic across multiple servers
- **Proxy Server**: Acts as an intermediary between clients and servers

## Module 5: Network Security Controls

### Access Control Lists (ACLs)
- Filter network traffic based on source/destination IP, port, or protocol
- Can be implemented on routers, switches, or firewalls

### Virtual Private Networks (VPNs)
- Create secure connections over public networks
- Encrypts data to protect it from eavesdropping
- Types: Site-to-site, remote access

### Network Segmentation
- Divides a network into smaller segments to limit the impact of security incidents
- Examples: VLANs (Virtual Local Area Networks), DMZs (Demilitarized Zones)

### IDS/IPS
- **Network-based IDS/IPS**: Monitors network traffic
- **Host-based IDS/IPS**: Monitors individual systems

## Module 6: Network Monitoring and Analysis

### Network Monitoring Tools
- **Wireshark**: Packet sniffing and analysis
- **Nmap**: Network mapping and port scanning
- **SolarWinds**: Network performance monitoring
- **Zabbix**: Open-source network monitoring

### Packet Sniffing and Analysis
- Capturing and analyzing network packets
- Identifying network issues and security incidents
- Wireshark filters and analysis techniques

### Network Performance Monitoring
- Monitoring bandwidth usage
- Tracking network latency
- Identifying bottlenecks
- Capacity planning

## Module 7: Wireless Network Security

### Wireless Network Fundamentals
- **Wi-Fi Standards**: 802.11a/b/g/n/ac/ax
- **Wireless Channels**: Frequency bands used for communication
- **Signal Strength**: Measured in dBm (decibel-milliwatts)

### Wi-Fi Security Protocols
- **WEP**: Weak security protocol (easily cracked)
- **WPA**: Improved security protocol
- **WPA2**: Current standard with strong security
- **WPA3**: Newer protocol with enhanced security

### Wireless Network Threats
- **Rogue Access Points**: Unauthorized access points
- **Evil Twin Attacks**: Fake access points masquerading as legitimate ones
- **Wireless Eavesdropping**: Intercepting wireless communications
- **MAC Spoofing**: Impersonating another device's MAC address

## Module 8: Network Hardening and Optimization

### Network Hardening Techniques
- **Disabling Unnecessary Services**: Reducing attack surface
- **Implementing ACLs**: Controlling network traffic
- **Enabling Encryption**: Protecting data in transit
- **Updating Firmware**: Patching vulnerabilities

### Network Performance Optimization
- **Load Balancing**: Distributing traffic across servers
- **Caching**: Storing frequently accessed data
- **Compression**: Reducing data size for faster transfer
- **Quality of Service (QoS)**: Prioritizing network traffic

### Network Security Policies and Procedures
- **Acceptable Use Policy (AUP)**: Defines proper network usage
- **Password Policy**: Requirements for strong passwords
- **Incident Response Policy**: Procedures for handling security incidents
- **Change Management Policy**: Process for making network changes

## Key Takeaways

1. **Network fundamentals are essential for cybersecurity**: Understanding how networks work is crucial for securing them
2. **Network security is multi-layered**: Implementing multiple security controls provides better protection
3. **Network monitoring is important**: Regularly monitoring networks helps detect security incidents early
4. **Wireless networks require special security measures**: Wireless networks are more vulnerable to attacks
5. **Network hardening reduces attack surface**: Disabling unnecessary services and implementing security controls reduces vulnerabilities

## Best Practices Summary

- Implement a defense-in-depth security strategy
- Use strong authentication and access controls
- Regularly update and patch network devices
- Monitor networks for security incidents
- Train employees on network security best practices
- Develop and test incident response plans
- Conduct regular network security assessments

These summary notes are specifically aligned with the **Networks and Network Security** course in the Google Cybersecurity Professional Certificate program, focusing on the skills and knowledge needed for entry-level Security Analyst roles.