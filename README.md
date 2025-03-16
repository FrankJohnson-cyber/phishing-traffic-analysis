# Email Phishing Traffic Analysis with Wireshark

This project simulates a phishing email attack, capturing and analyzing network traffic with Wireshark to identify indicators of compromise (IOCs) and document response steps for a SOC playbook.

## Overview
- **Objective:** Detect and analyze a phishing email with a malicious link.
- **Tools:** Wireshark, VirtualBox, Kali Linux, Windows VM.
- **Key Findings:** Spoofed SMTP sender, unencrypted email traffic, HTTP credential harvesting.

## Files
- `phishing-email.pcap`: Sample packet capture (simulated).
- `phishing-analysis.md`: Analysis report with screenshots and playbook snippet.

## Usage
Open `phishing-email.pcap` in Wireshark, filter with `smtp` or `http`, and follow TCP streams to explore the attack.

Built by Frank Johnson, CompTIA CSAP | CySA+ | Security+ certified.
