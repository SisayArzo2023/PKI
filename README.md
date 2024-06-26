# Public Key Infrastructure (PKI)
This project is aimed at developing a basic PKI monitoring and analysis tool <br>
## Introduction:
Wikipedia provided a comprehensive definition of PKI as "a set of roles, policies, hardware, software and procedures needed to create, manage, distribute, use, store and revoke digital certificates and manage public-key encryption." In the typical application, we can say PKI is a method used by web browsers to determine if a website is genuine and belongs to the correct business or organization.
## Components of PKI
1. Digital certificate: an electronic document that is used to bind identities with the keys. The document may contain the digital identity a public key owner which could be an individual, organization, a hardware device, etc, and the corresponding public key.  
2. Certificate authority:
3. Public and private key:
4. Digital signature:
5. Certificate revocation:
6. Certificate policies and practices:
7. Key Management:
8. Trust Models:
9. Standards and protocols:
10. Applications:

## PKI Procedural Model
![Architectural-model-of-a-PKI](https://github.com/SisayArzo2023/PKI/assets/122646258/a2952529-db0b-4551-bf0a-9318d126fab4)

## Monitoring PKI agents 
Monitoring a Public Key Infrastructure (PKI) in a Microsoft Windows environment using agents involves leveraging various tools and utilities to collect data and metrics from PKI components. Here's how we can implement monitoring using agents specifically tailored for Microsoft Windows:

### Windows Performance Monitor (PerfMon):
Utilize PerfMon to monitor system performance metrics relevant to PKI components, such as CPU usage, memory utilization, disk I/O, and network traffic. Create custom performance counters to monitor specific aspects of PKI, such as Certificate Services performance counters for monitoring certificate issuance rates, pending certificate requests, and database performance.

### Event Viewer:
Use Event Viewer to monitor and analyze Windows event logs generated by PKI components, including Certificate Services, Active Directory Certificate Services (AD CS), and related services. Set up event log subscriptions to centralize event log collection and analysis across multiple Windows servers hosting PKI components.

### PowerShell Scripting:
Develop PowerShell scripts to automate monitoring tasks and collect data from PKI components using built-in cmdlets or WMI (Windows Management Instrumentation).
Use PowerShell remoting to execute scripts on remote PKI servers and gather information about certificate issuance, revocation, and key management.

### System Center Operations Manager (SCOM):
Deploy SCOM agents on Windows servers hosting PKI components to enable centralized monitoring and management. Configure SCOM management packs for PKI to monitor performance, availability, and security events related to certificate services, AD CS, and other PKI-related services.

### Third-party Monitoring Solutions:
Explore third-party monitoring solutions compatible with Windows environments, such as SolarWinds Server & Application Monitor, ManageEngine OpManager, or PRTG Network Monitor.
Install monitoring agents or probes on Windows servers to collect data and metrics specific to PKI components, including certificate issuance, revocation, and key usage.

### Certificate Services Monitoring Tools:
Use built-in tools and utilities provided by Microsoft Windows for monitoring Certificate Services and AD CS. Monitor Certificate Services health using the Certification Authority Management Console (certsrv.msc) to view certificate status, pending requests, and CA configuration.

### Task Scheduler:
Schedule recurring tasks or PowerShell scripts to automate PKI monitoring activities, such as checking certificate expiration dates, verifying CRL (Certificate Revocation List) publication, or monitoring certificate revocation events.

### Security Information and Event Management (SIEM) Integration:
Integrate Windows event log data from PKI components with SIEM solutions, such as Splunk, ArcSight, or Elastic SIEM, for centralized log management, correlation, and analysis.
Configure event log forwarding or agent-based log collection to stream Windows event logs to the SIEM platform for real-time monitoring and alerting.

By leveraging these tools and utilities within the Microsoft Windows ecosystem, we can effectively monitor and manage the PKI infrastructure, ensuring the security, reliability, and compliance of certificate services and key management processes.

### The architecture of the monitoring tool
i. Database
ii. Collection agents 

### A Little About C# 
#### Type Safe
The C# code is type safe can only access memory locations that it has permission to execute. This feature significantly enhances program security.
