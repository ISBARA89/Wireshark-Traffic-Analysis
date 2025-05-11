# Wireshark Traffic Analysis Project

This project demonstrates basic network traffic monitoring and analysis using Wireshark, a powerful network protocol analyzer that captures and interprets real-time data transmitted during regular web browsing activities.

## Objective

- Learn how to use Wireshark to monitor network packets.
- Understand how DNS, TCP, and HTTPS traffic appear in packet captures.
- Identify the data flow between a local machine and external web servers.

## Tools Used

- **Wireshark**
- **Google Chrome Browser**
- **Windows 11 (any OS with internet access)**

## Websites Visited

- [https://jumia.com.ng](https://jumia.com.ng)
- [https://openai.com](https://openai.com)
- [https://github.com](https://github.com)

## Files Included

- `website_traffic_analysis.pcapng` — The packet capture file.
- `traffic_notes.md` — Observations and analysis of captured traffic.
- `README.md` — Project summary and instructions.

## How to Reproduce

1. Open Wireshark and select your active network interface (e.g., Wi-Fi).
2. Start capturing packets.
3. Open a browser and visit any 2–3 websites.
4. Stop the capture after a few seconds.
5. Apply filters like `dns`, `tcp`, `http`, or `tls` to explore the traffic.
6. Document key observations in a `.md` or `.txt` file.

## What You'll Learn

- How domain name resolution works (DNS)
- How TCP handshakes are structured
- How encrypted traffic (HTTPS/TLS) behaves
- How to filter and analyze different protocol layers

---

**Author:** Adeniyi Moses Oluwaseun  
**License:** MIT
