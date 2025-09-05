## Project: Simulated Phishing & Ransomware Incident Response

This repository contains simulated incident scenarios (phishing and ransomware) analyzed using the **5 W’s** (Who, What, Where, When, Why) and documented with **formal response actions**.

## Scenarios
1. **Phishing Simulation** – Malicious email attempting to harvest credentials.
2. **Ransomware Simulation** – Files encrypted, ransom note demands payment.

Each scenario includes:
- **Incident report (5 W’s + IOCs)**
- **Sample artifacts** (email/ransom note)
- **Response plan** (containment, eradication, recovery, comms)

## Purpose
Practice structured, standards-aligned incident response and showcase documentation skills.

## phishing-simulation/incident_report.md
# Incident Report – Phishing Simulation

## 5 W’s
- **Who:** Targeted employees at ACME Corp.
- **What:** Email spoofing IT; link to fake SSO page to steal credentials.
- **Where:** Corporate email; user workstation browser.
- **When:** Detected 2025-09-04 09:15 PT.
- **Why:** Credential theft for unauthorized access.

## IOCs
- Sender: support@fake-it.helpdesk.com
- Subject: "Password Reset Required Immediately"
- URL: http://malicious-reset.example/login

## Summary
A user reported a suspicious email. Security review confirmed a spoofed domain and credential-harvesting page.

## Impact (Simulated)
No confirmed credential use; 2 users clicked link, 0 submitted credentials.

## Evidence
- `email_sample.eml`
- Proxy logs showing outbound to malicious domain
