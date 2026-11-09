# DNS Investigation Using Wireshark

## Project Overview
This project demonstrates practical DNS investigation and packet analysis using Wireshark. The objective was to understand how DNS queries and responses work, identify DNS servers, inspect packet details, and examine different DNS record types.

## Objectives
- Capture and analyze DNS traffic using Wireshark.
- Identify DNS queries and their corresponding responses.
- Examine source and destination IP addresses and UDP port 53.
- Identify the DNS resolver used by the system.
- Investigate common DNS record types.
- Understand DNS response codes and packet details.

## Tools and Environment
- **Operating System:** Windows
- **Packet Analyzer:** Wireshark
- **Command-line Tool:** Windows Command Prompt (`nslookup`, `ipconfig`)

## Practical Work
The investigation included:

1. Flushing the local DNS cache.
2. Generating DNS queries for domains including Google, Microsoft, YouTube, GitHub, and Cloudflare.
3. Capturing DNS traffic in Wireshark.
4. Analyzing query and response packet pairs.
5. Inspecting DNS record types:
   - A
   - AAAA
   - MX
   - NS
   - TXT
   - CNAME
   - PTR
6. Examining transaction IDs, response flags, TTL values, and resolved IP addresses.

## Key Findings
- DNS queries and responses were observed using UDP port 53.
- The local DNS resolver was observed at `192.168.1.1` (IPv4) and `fe80::1` (IPv6).
- The resolver hostname was reported as `gpon.net`.
- Both IPv4 and IPv6 DNS records were identified.
- Mail, name server, text, canonical name, and reverse DNS records were examined.
- A DNS query and its corresponding response were matched using their transaction ID.

## Repository Contents
- `DNS-Investigation-Report.pdf` – Detailed project report and evidence.
- `DNS-Investigation.pcapng` – Wireshark packet capture, if included.

## Learning Outcome
This exercise improved my understanding of DNS resolution, DNS record types, packet-level analysis, and the role of DNS in network communication.

