# Passive Reconnaissance

## 1. Overview

Passive Reconnaissance is the process of collecting information about a target using publicly available sources without directly interacting with the target's systems.

It helps security professionals understand a target's digital footprint before conducting a security assessment.

## 2. Objective

To perform passive information gathering and identify publicly available domain registration details using WHOIS.

## 3. Target

`certifiedhacker.com`

## 4. Tool Used

- WHOIS

## 5. Command Executed

```bash
whois certifiedhacker.com
```

## 6. Key Findings

- **Domain Name:** certifiedhacker.com
- **Registrar:** Network Solutions, LLC
- **Creation Date:** 30 July 2002
- **Expiry Date:** 30 July 2027
- **Name Servers:** NS1.BLUEHOST.COM, NS2.BLUEHOST.COM
- **DNSSEC Status:** Unsigned
- **Privacy Protection:** Perfect Privacy, LLC
- **Domain Status:** clientTransferProhibited

## 7. Analysis of Findings

- Identified the domain registrar and registration history.
- Discovered the name servers used for DNS management.
- Identified the domain's registration expiry date.
- Observed that registrant information is protected by a privacy service.
- Found that DNSSEC is unsigned.

## 8. Result

Successfully performed passive reconnaissance and collected publicly available domain registration information using WHOIS.

## 9. Evidence

Refer to `whois-output.txt` for the original command output.

## 10. Disclaimer

This exercise was performed for educational purposes using publicly available domain registration information. No intrusive testing or unauthorized access was attempted.
