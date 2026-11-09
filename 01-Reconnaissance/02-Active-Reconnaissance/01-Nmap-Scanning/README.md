# Nmap Scanning [ Active Reconnaissance ]

## Project Overview

Nmap (Network Mapper) is a network scanning tool used for Active Reconnaissance, to discover hosts, identify open ports, detect services and versions, and gather information about target systems.

This project demonstrates practical network scanning and enumeration techniques using Nmap in an authorized VMware lab environment.

## Objectives

- Discover active hosts on a network.
- Identify open, closed, and filtered ports.
- Perform TCP and UDP port scanning.
- Detect running services and their versions.
- Identify target operating systems.
- Understand different Nmap scanning techniques.

## Lab Environment

| Component | Details |
|---|---|
| Operating System | Kali Linux |
| Scanning Tool | Nmap |
| Nmap Version | 7.99 |
| Environment | VMware Virtual Lab |
| Target | Authorized lab machine |

## Nmap Scanning Techniques

| Flag | Description |
|---|---|
| `-sn` | Host discovery without port scanning |
| `-sS` | TCP SYN scan |
| `-sT` | TCP Connect scan |
| `-sU` | UDP scan |
| `-sV` | Service and version detection |
| `-O` | Operating system detection |
| `-A` | Aggressive detection |
| `-p-` | Scan all TCP ports |
| `-p` | Scan specified ports |
| `-Pn` | Skip host discovery |

## Project Methodology

1. Identify the authorized lab target.
2. Perform host discovery.
3. Conduct TCP and UDP port scanning.
4. Scan selected ports and all TCP ports.
5. Detect services and their versions.
6. Perform operating system detection.
7. Use aggressive detection to gather additional information.
8. Analyze and document the results.

## Expected Outcomes

- Understand different Nmap scanning techniques.
- Identify exposed network services.
- Understand port states and service detection.
- Gain practical experience in network reconnaissance.

## Disclaimer

All scanning activities in this project are performed only against an authorized virtual lab environment for educational purposes. Scanning systems without permission is not encouraged.
