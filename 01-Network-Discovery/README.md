# Network Discovery

## 🟡 PROJECT OVERVIEW
Network Discovery is the process of identifying devices connected to a network and collecting basic information about them.

This project demonstrates practical network discovery using Nmap in Kali Linux.

## 🟡 OBJECTIVES

- Identify the network range.
- Discover live hosts.
- Identify MAC addresses (where available).
- Detect operating systems (where possible).

## 🟡 TOOLS USED
- Nmap

## 🟡 METHODOLOGY

Nmap was used in an authorized virtual lab environment to:

- Scan the local network and identify active hosts.
- Identify MAC addresses where available.
- Perform operating system detection on the selected target.
- Identify open TCP ports and their associated service names.



## 🟡 COMMANDS EXECUTED

### For Network Discovery

```bash
nmap -sn -oN 01-network-discovery.txt 192.168.96.0/24
```

### For Operating System Detection

```bash
sudo nmap -O -oN 02-os-detection.txt 192.168.96.137
```




## 🟡 SCAN RESULTS

### Network Discovery
- Network Range: 192.168.96.0/24
- Total IP addresses scanned: 256
- Live hosts discovered: 5
- MAC addresses identified: 4

### Target Identification
- Target IP: 192.168.96.137
- MAC Address: 00:0C:29:FA:DD:2A
- MAC Vendor: VMware

### Operating System Detection
- Detected OS: Linux 2.6.x
- Device Type: General Purpose
- Network Distance: 1 hop

## 🟡 KEY FINDINGS

- Successfully identified five active hosts.
- Identified available MAC addresses.
- Detected the target machine's estimated operating system.
- Saved actual Nmap scan outputs in this repository.


## 🟡 CONCLUSION
This project demonstrates fundamental network discovery and host identification using Nmap.

## 🟡 DISCLAIMER
All activities are performed for educational purposes in an authorized lab environment.
