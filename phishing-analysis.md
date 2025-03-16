# Phishing Analysis Report

## Steps
1. Captured SMTP traffic (`tcp.port == 25`) showing email from `spoofed@example.com`.
2. Identified malicious URL (`http://fake-phish.com`) in the email body via TCP stream.
3. Tracked HTTP GET request to `192.168.1.100`, revealing a phishing form.

## IOCs
- IP: `192.168.1.100`
- Domain: `fake-phish.com`
- URL: `http://fake-phish.com/login`

## Playbook Snippet
- Filter: `smtp contains "fake-phish"`
- Action: Block IP, alert SOC team.
