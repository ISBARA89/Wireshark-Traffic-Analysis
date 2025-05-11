# Wireshark Traffic Analysis Notes 
_Captured during visits to jumia.com.ng, openai.com, and github.com_

## Capture Overview
- **Date:** [Insert Date of Capture]
- **Interface Used:** Wi-Fi
- **Tools:** Wireshark v[version], Chrome Browser
- **Websites Visited:** 
  - https://jumia.com.ng 
  - https://openai.com 
  - https://github.com 

---

## DNS Queries
- Multiple DNS queries observed:
  - `jumia.com.ng` resolved to [IP address seen]
  - `openai.com` resolved to [IP address seen]
  - `github.com` resolved to [IP address seen]
- DNS server response received from `8.8.8.8` (Google DNS) 
- Query Type: A and AAAA

---

## TCP Traffic
- Normal TCP 3-way handshakes captured:
  - SYN → SYN-ACK → ACK 
- TCP sessions established between local IP and servers for the three websites.
- Typical ports used: 443 (HTTPS), 80 (HTTP)

---

## HTTP/HTTPS Requests
- **jumia.com.ng**:
  - Encrypted HTTPS traffic (port 443)
  - Observed SNI (Server Name Indication) as `jumia.com.ng`

- **openai.com** and **github.com**:
  - Also over HTTPS (port 443)
  - TLS handshake packets observed

---

## ICMP (Optional, if ping used)
- No ICMP traffic observed during session (ping not initiated)

---

## Observations & Learning
- HTTPS encrypts most web content, but we can still see metadata like domain names, IPs, and handshake processes.
- DNS lookups occur before TCP connections — confirms the order of operations.
- TLS Handshakes reveal certificate information and supported cipher suites.

---

## File Info
- Capture File: `website_traffic_analysis.pcapng` 
- Notes Author: Adeniyi Oluwaseun | ISBARA89