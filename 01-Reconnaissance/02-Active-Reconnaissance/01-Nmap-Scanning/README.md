# Nmap Scanning [ Active Reconnaissance ]

## Project Overview

Nmap (Network Mapper) is an open-source network scanning tool used to discover hosts, identify open ports, detect running services, determine software versions, and gather information about target systems.

This project demonstrates practical network scanning and enumeration techniques using Nmap in an authorized VMware virtual lab environment.

## Project Objectives

- Discover active hosts within a network.
- Identify open, closed, and filtered ports.
- Perform TCP and UDP scanning.
- Detect running services and their versions.
- Identify probable operating systems.
- Perform full TCP port scanning.
- Understand different Nmap scanning techniques.

## Lab Environment

| Component | Details |
|---|---|
| Operating System | Kali Linux |
| Scanning Tool | Nmap |
| Nmap Version | 7.99 |
| Virtualization | VMware |
| Target IP | 192.168.96.137 |
| Network | 192.168.96.0/24 |

## Tools Used

- Nmap
- Kali Linux
- VMware Workstation

## Scanning Methodology

### 1. Host Discovery

**Flag:** `-sn`

**Command:**
```bash
nmap -sn 192.168.96.0/24 -oN 01-host-discovery.txt
```

**Purpose:** Discover active hosts on the network without performing port scanning.

**Observation:** Identified 5 active hosts within the scanned network.

**Evidence:**
- [Scan Output](Outputs/01-host-discovery.txt)
- [Screenshot](Screenshots/01-host-discovery.png)

### 2. TCP SYN Scan

**Flag:** `-sS`

**Command:**
```bash
sudo nmap -sS 192.168.96.137 -oN 02-tcp-syn-scan.txt
```

**Purpose:** Perform a TCP SYN scan to identify port states without completing the normal TCP handshake for open ports.

**Evidence:**
- [Scan Output](Outputs/02-tcp-syn-scan.txt)
- [Screenshot](Screenshots/02-tcp-syn-scan.png)

### 3. TCP Connect Scan

**Flag:** `-sT`

**Command:**
```bash
sudo nmap -sT 192.168.96.137 -oN 03-tcp-connect-scan.txt
```

**Purpose:** Identify TCP port states by establishing full TCP connections.

**Evidence:**
- [Scan Output](Outputs/03-tcp-connect-scan.txt)
- [Screenshot](Screenshots/03-tcp-connect-scan.png)

### 4. Service and Version Detection

**Flag:** `-sV`

**Command:**
```bash
sudo nmap -sV 192.168.96.137 -oN 04-service-version-detection.txt
```

**Purpose:** Identify running services and detect their software versions.

**Evidence:**
- [Scan Output](Outputs/04-service-version-detection.txt)
- [Screenshot](Screenshots/04-service-version-detection.png)

### 5. UDP Scan

**Flag:** `-sU`

**Command:**
```bash
sudo nmap -sU 192.168.96.137 -oN 05-udp-scan.txt
```

**Purpose:** Identify UDP port states and discover services communicating over UDP.

**Evidence:**
- [Scan Output](Outputs/05-udp-scan.txt)
- [Screenshot](Screenshots/05-udp-scan.png)

### 6. Specific Port Scan

**Flag:** `-p`

**Command:**
```bash
sudo nmap -p 21,22,23,80,443 192.168.96.137 -oN 06-specific-port-scan.txt
```

**Purpose:** Scan five selected TCP ports associated with commonly used network services.

| Port | Service |
|---|---|
| 21 | FTP |
| 22 | SSH |
| 23 | Telnet |
| 80 | HTTP |
| 443 | HTTPS |

**Evidence:**
- [Scan Output](Outputs/06-specific-port-scan.txt)
- [Screenshot](Screenshots/06-specific-port-scan.png)

### 7. Full Port Scan

**Flag:** `-p-`

**Command:**
```bash
sudo nmap -p- 192.168.96.137 -oN 07-full-port-scan.txt
```

**Purpose:** Scan all 65,535 TCP ports to identify exposed services running on standard and non-standard ports.

**Evidence:**
- [Scan Output](Outputs/07-full-port-scan.txt)
- [Screenshot](Screenshots/07-full-port-scan.png)

### 8. Operating System Detection

**Flag:** `-O`

**Command:**
```bash
sudo nmap -O 192.168.96.137 -oN 08-os-detection.txt
```

**Purpose:** Identify the probable operating system running on the target using OS fingerprinting.

**Evidence:**
- [Scan Output](Outputs/08-os-detection.txt)
- [Screenshot](Screenshots/08-os-detection.png)

### 9. Aggressive Scan

**Flag:** `-A`

**Command:**
```bash
sudo nmap -A 192.168.96.137 -oN 09-aggressive-scan.txt
```

**Purpose:** Gather detailed target information through:
- OS detection
- Service and version detection
- Default NSE script scanning
- Traceroute

**Evidence:**
- [Scan Output](Outputs/09-aggressive-scan.txt)
- [Screenshot 1](Screenshots/09-aggressive-scan-01.png)
- [Screenshot 2](Screenshots/09-aggressive-scan-02.png)
- [Screenshot 3](Screenshots/09-aggressive-scan-03.png)

### 10. Comprehensive Nmap Scan

**Command:**
```bash
sudo nmap -sS -sV -O -A -p- 192.168.96.137 -oN 10-comprehensive-scan.txt
```

**Purpose:** Combine multiple Nmap scanning and detection techniques into a comprehensive assessment of the authorized lab target.

**Techniques included:**
- TCP SYN scanning
- Service and version detection
- Operating system detection
- Aggressive detection
- Full TCP port scanning

**Evidence:**
- [Scan Output](Outputs/10-comprehensive-scan.txt)
- [Screenshot 1](Screenshots/10-comprehensive-scan-01.png)
- [Screenshot 2](Screenshots/10-comprehensive-scan-02.png)
- [Screenshot 3](Screenshots/10-comprehensive-scan-03.png)

## Key Learnings

Through this practical exercise, I gained experience in:

- Host discovery and network enumeration.
- Understanding TCP SYN and TCP Connect scanning.
- Identifying TCP and UDP port states.
- Detecting services and software versions.
- Performing operating system fingerprinting.
- Scanning specific ports and the complete TCP port range.
- Combining multiple Nmap techniques for detailed network assessment.

## Conclusion

This project provided hands-on experience with Nmap scanning and enumeration techniques in a virtual lab environment. It strengthened my understanding of network reconnaissance, exposed services, port states, and target information gathering.

## Disclaimer

All scanning activities documented in this project were performed against an authorized virtual lab environment for educational and practical learning purposes. Scanning systems without proper authorization is not encouraged.
