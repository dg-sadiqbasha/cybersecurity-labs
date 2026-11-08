# theHarvester – Passive Information Gathering

## Project Overview

theHarvester is an information-gathering tool used to collect publicly available information about a target domain from multiple search engines and data sources.

This exercise demonstrates passive reconnaissance using theHarvester.

## Objective

To identify publicly available information associated with a domain, including hostnames, IP addresses, URLs, and other domain-related details.

## Target

`certifiedhacker.com`

## Tool Used

- **Tool:** theHarvester
- **Version:** 4.11.1
- **Environment:** Kali Linux

## Command Used

```bash
theHarvester -d certifiedhacker.com -b all
```

## Findings

The tool reported the following results:

| Information | Results |
|---|---:|
| Hosts found | 88 |
| IP addresses found | 8 |
| Interesting URLs | 3 |
| ASNs found | 1 |
| Email addresses | 0 |
| People found | 0 |
| LinkedIn users | 0 |

### Examples of Discovered Hostnames

- `mail.certifiedhacker.com`
- `blog.certifiedhacker.com`
- `cpanel.certifiedhacker.com`
- `ftp.certifiedhacker.com`
- `webmail.certifiedhacker.com`
- `soc.certifiedhacker.com`

### Examples of Reported IP Addresses

- `162.241.216.11`
- `183.82.41.50`
- `202.75.54.102`
- `64.90.163.30`
- `69.89.31.193`

*These are examples from the tool output; their ownership and current reachability were not independently verified.*

## Analysis

TheHarvester collected domain-related information from multiple public sources.

It reported 88 hosts and 8 IP addresses, along with 3 interesting URLs and 1 ASN.

Several integrated sources could not complete their searches because API keys or valid authentication credentials were unavailable. Therefore, the results represent the information retrieved during this particular run and may not be exhaustive.

## Result

This exercise demonstrated how theHarvester can help gather publicly available domain-related information and support the passive reconnaissance phase of a security assessment.

## Evidence

- `theHarvester-output.txt` – Command output containing the collected results.

## Disclaimer

This exercise was conducted for educational purposes using publicly available information. No exploitation or intrusive testing was performed. Always obtain proper authorization before conducting security testing.
