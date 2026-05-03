# SOC Homelab with Wazuh

## Overview

This repository documents the development of a SOC-style security monitoring homelab built using Wazuh, Docker, VirtualBox, and additional security tools.

The project was created to gain hands-on experience in endpoint monitoring, centralized logging, intrusion detection, alert analysis, and security lab documentation.

The homelab was developed in two main versions:

- **V1:** Base Wazuh deployment with Windows endpoint monitoring
- **V2:** Expanded monitoring environment with Suricata IDS, DVWA, and additional attack/testing scenarios

## Project Versions

| Version | Focus | Status |
|---|---|---|
| [V1 - Wazuh Endpoint Monitoring](v1/) | Wazuh deployment, Windows endpoint agent, basic alert review | Completed |
| [V2 - IDS and Web Attack Monitoring](v2/) | Suricata IDS, DVWA, network monitoring, attack simulation | Completed, documentation in progress |

## Architecture Overview

<p align="center">
  <img src="v2/images/v2-architecture.png"
       alt="SOC Homelab V2 Architecture"
       width="700">
</p>

> Detailed architecture diagrams and explanations are available in each version folder.

## Tools and Technologies:
- Wazuh
- Docker
- Oracle VirtualBox
- Ubuntu Server
- Windows 10 endpoint
- Suricata IDS
- DVWA
- Kali Linux

## Detection Scenarios

The lab includes several controlled security testing scenarios, including:

- Nmap scan detection
- Nikto web scan detection
- Suricata alert forwarding into Wazuh
- SSH failed-login and brute-force detection
- Windows endpoint monitoring through the Wazuh agent

## Repository Structure

```text
v1/    Documentation for the initial Wazuh endpoint monitoring setup
v2/    Documentation for the expanded IDS and web attack monitoring setup
