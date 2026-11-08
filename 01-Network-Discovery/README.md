# Network Discovery

## Project Overview
Network Discovery is the process of identifying devices connected to a network and collecting basic information about them.

This project demonstrates practical network discovery using Nmap in Kali Linux.

## Objectives
- Identify the network range.
- Discover live hosts.
- Identify MAC addresses (where available).
- Detect operating systems (where possible).

## Tool Used
- Nmap

## Methodology
Nmap was used to scan the authorized lab network, identify active hosts, detect available services, and gather operating system information.

## Results

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

### Key Findings
- Successfully identified five active hosts.
- Identified available MAC addresses.
- Detected the target machine's estimated operating system.
- Saved actual Nmap scan outputs in this repository.

## Conclusion
This project demonstrates fundamental network discovery and host identification using Nmap.

## Disclaimer
All activities are performed for educational purposes in an authorized lab environment.
