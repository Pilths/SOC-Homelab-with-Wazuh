## Lab Environment

- **Host Machine:** Windows 11
- **Virtualization Platform:** Oracle VirtualBox
- **Wazuh Server Host:** Ubuntu virtual machine
- **Monitored Endpoint:** Windows 10 virtual machine with Wazuh agent installed
- **Deployment Method:** Docker-based Wazuh installation

## Deployment Summary

The lab was built by deploying Wazuh on an Ubuntu virtual machine using Docker. The Ubuntu VM acts as the main server host for the Wazuh components, including the Manager, Indexer, and Dashboard. A separate Windows 10 virtual machine was prepared as the monitored endpoint and connected to the Wazuh server using the Wazuh agent.

After the containers were started successfully, the Wazuh dashboard was accessed through the browser to confirm that the services were running. The Windows 10 endpoint was then enrolled to the Wazuh server so that endpoint-generated events could be collected and reviewed through the dashboard.

## Agent Enrollment

The Wazuh agent was installed on the Windows 10 virtual machine and configured to connect to the Wazuh server running on the Ubuntu virtual machine. After installation, the agent service was started and its connection status was verified through the Wazuh dashboard.

## Validation Performed

Basic validation was performed to confirm that the deployment was working correctly. This included verifying that:
- the Wazuh dashboard was accessible
- the Windows endpoint appeared as an active agent
- endpoint-generated security events could be viewed from the dashboard

At this stage, the project focused on confirming successful deployment and basic visibility of monitored endpoint activity.

## Challenges Encountered

During deployment, several practical issues were encountered in the homelab environment. These included service startup delays, dashboard readiness after container launch, and networking considerations between the virtual machines. Additional care was also required to ensure that the Windows endpoint could communicate correctly with the Wazuh server.

Overall, these issues helped improve understanding of container startup behavior, VM networking, and agent connectivity in a small monitoring lab.

## Reference
The Wazuh deployment in this project was based on the Wazuh Docker documentation.
