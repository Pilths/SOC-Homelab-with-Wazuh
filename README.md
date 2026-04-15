# Security Monitoring Homelab with Wazuh

## Objectives
This project demonstrates a small security monitoring homelab built with Wazuh in a virtualized environment. The lab focuses on collecting endpoint telemetry from a Windows machine, validating security event visibility, and applying basic alert tuning to improve monitoring clarity.

## Tools Used
- Wazuh
- Docker
- Oracle VirtualBox
- Ubuntu Server
- Windows 10

## Lab Environment
- **Host Machine:** Windows 11
- **Virtualization Platform:** Oracle VirtualBox
- **Wazuh Server Host:** Ubuntu virtual machine
- **Monitored Endpoint:** Windows 10 virtual machine with Wazuh agent installed

## Architecture Diagram
![Wazuh Homelab Architecture](diagrams/wazuh-homelab-architecture.png)

## Architecture Overview
The homelab is hosted on a Windows 11 machine running Oracle VirtualBox. Inside the virtualized environment, an Ubuntu virtual machine hosts the Wazuh stack through Docker, including the Wazuh Manager, Indexer, and Dashboard. A separate Windows 10 virtual machine acts as the monitored endpoint and runs the Wazuh agent, which forwards security-related events to the Wazuh server for monitoring and analysis.

## Test Scenarios
- User Account Creation Detection
- Failed Logon Detection


## Key Outcomes

The project successfully deployed Wazuh in a virtualized homelab environment using Docker on an Ubuntu virtual machine. A Windows 10 endpoint was connected as a Wazuh agent, allowing the lab to collect and review endpoint-generated security events through the Wazuh dashboard.

Through simple validation scenarios such as user account creation and failed logon activity, the project confirmed that Wazuh was able to provide visibility into selected Windows security events. This helped demonstrate a practical understanding of endpoint monitoring, alert observation, and the role of SIEM in a small lab environment.
