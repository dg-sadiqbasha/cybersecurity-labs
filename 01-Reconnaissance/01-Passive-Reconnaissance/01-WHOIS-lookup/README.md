# WHOIS Lookup – Passive Reconnaissance

## Project Overview

WHOIS is a protocol used to retrieve publicly available domain registration information, such as registrar details, registration dates, domain status, and name servers.

This exercise demonstrates passive information gathering using the WHOIS tool.

## Objective

To collect and analyze publicly available domain registration information.

## Target

`certifiedhacker.com`

## Tool Used

- **Tool:** WHOIS
- **Environment:** Kali Linux

## Command Used

```bash
whois certifiedhacker.com
```

## Findings

The WHOIS lookup returned the following information:

| Information | Observed Result |
|---|---|
| Domain Name | certifiedhacker.com |
| Registrar | Network Solutions, LLC |
| Creation Date | 30 July 2002 |
| Expiry Date | 30 July 2027 |
| Name Server 1 | ns1.bluehost.com |
| Name Server 2 | ns2.bluehost.com |
| DNSSEC | Unsigned |
| Domain Status | clientTransferProhibited |
| Registrant | PERFECT PRIVACY, LLC |

## Analysis

- The domain was originally registered in 2002.
- Network Solutions, LLC is listed as the registrar.
- The domain uses Bluehost name servers.
- DNSSEC is reported as unsigned.
- Registrant information is protected through a privacy registration service.
- The `clientTransferProhibited` status indicates a restriction on transferring the domain.

## Result

Successfully retrieved and analyzed publicly available domain registration information using WHOIS.

This exercise demonstrates how WHOIS supports passive reconnaissance by providing useful domain-related information without directly probing the target's systems.

## Evidence

- `whois-output.txt` – Contains the captured WHOIS command output.

## Disclaimer

This exercise was conducted for educational purposes using publicly available domain registration information. No intrusive testing or exploitation was performed.
