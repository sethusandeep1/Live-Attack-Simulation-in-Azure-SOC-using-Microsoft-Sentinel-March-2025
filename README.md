# Live-Attack-Simulation-in-Azure-SOC-using-Microsoft-Sentinel

## Overview

In this project, I built a **Live Attack Simulation** environment using **Azure** and **Microsoft Sentinel** for a **Security Operations Center (SOC)**. The project is designed to simulate real-world cyber-attacks and demonstrates how SOC teams can monitor, detect, and respond to these attacks in real-time. The simulation leverages **Azure resources**, **Log Analytics Workspaces**, and **Microsoft Sentinel** to centralize log collection and threat detection.

## Steps Taken

### 1. **Setting Up Azure Subscription and Resource Group**

The first step was setting up an **Azure Subscription** and creating a **Resource Group** called `RG-SOC-Lab`. This helps organize the resources involved in the attack simulation process.

![Resource Group Creation](https://drive.google.com/uc?id=10XRWKEzvbekh4_MBD4T2qt7iMt9lf46N)

---

### 2. **Creating Virtual Machine**

I created a **Virtual Machine (VM)** in the `RG-SOC-Lab` resource group. This VM acts as a **honeypot** that gets targeted during the simulated cyber-attacks.

![Virtual Machine Creation](https://drive.google.com/uc?id=1_fsmna-mxFj4p6MUOZYUF9MCJCFeo7yy)

---

### 3. **Configuring Log Analytics Workspace**

Next, a **Log Analytics Workspace** was configured to collect logs from the virtual machine and other Azure resources. The workspace is essential for aggregating all logs that will be analyzed by **Microsoft Sentinel**.

This image shows a GeoIP Lookup query for security events, mapping the IP addresses to geographic locations such as city and country.
![Log Analytics Workspace Setup](https://drive.google.com/uc?id=1swJbr0b--EN4G1ZmUqg7KpCzqHLG9EAU)


This image shows the User Activity logs, tracking actions like logins and account details for monitoring suspicious behavior.
![Log Analytics Workspace Setup](https://drive.google.com/uc?id=1faf1zGkIk_02DSUKkKZ3kFCHb_kRDRjJ)

---

### 4. **Integrating Microsoft Sentinel**

**Microsoft Sentinel** was then integrated with the **Log Analytics Workspace** to provide **advanced threat detection** and **incident management**. Sentinel uses machine learning and analytics to detect malicious activity, making it crucial for security monitoring.

![Sentinel Integration](https://drive.google.com/uc?id=120aAnpaQX47qZjXHaXhz0GobAtkHnceE)


This image displays the query results for SecurityEvent logs, filtered by specific event types. It shows the administrator account logins from the machine CORP-NET-EAST-1, providing a detailed overview of security-related events, including the EventSourceName, Task, and Channel.
![Microsoft Sentinel](https://drive.google.com/uc?id=1sgc9NhWJ4i9vrew5y-F0B3GhtBuJR3yM)


This image shows the integration of Microsoft Sentinel with Log Analytics Workspace, querying SecurityEvent logs for Event ID 4625 (failed login attempts). The results are displayed for monitoring and detecting potential security incidents in real-time.
![Microsoft Sentinel](https://drive.google.com/uc?id=1faf1zGkIk_02DSUKkKZ3kFCHb_kRDRjJ)

---

### 5. **Simulating Attacks and Monitoring with Attack Map**

Simulated cyber-attacks were executed, and an **Attack Map** was built to visualize the sources of these attacks. The map shows the geographical distribution of attacks based on real-time data, helping SOC teams track and respond quickly.

This map displays both city and country names, providing a comprehensive view of the geographical distribution of cyber-attacks for effective tracking and response.
![Attack Map](https://drive.google.com/uc?id=1yZeQhrztU14EQAWGXcJ5fn3FPGWN7C7y)

This map highlights country names, giving a clear overview of the global spread of the simulated cyber-attacks, simplifying threat tracking.
![Attack Map](https://drive.google.com/uc?id=1kEolZzbtCkp2u2oMOce64hzoyzM5fm-s)

This map focuses on city names, offering a more granular view of the attack sources to help pinpoint specific locations for targeted responses.
![Attack Map](https://drive.google.com/uc?id=1GL-qpAYqAFPvfVa71p6OVgDGaJUHQZMX)



## Conclusion

This project demonstrates how **Azure** and **Microsoft Sentinel** can be leveraged to simulate cyber-attacks and efficiently monitor security events. The **Log Analytics Workspace** collects data from different resources, while **Microsoft Sentinel** processes the data for real-time threat detection. The **Attack Map** helps visualize where the attacks are originating from, assisting security teams in making informed decisions.

---

## Future Improvements

- **Enhanced Detection Capabilities**: Expanding detection rules and integrating more data sources for a broader perspective.
- **Automated Threat Response**: Configuring automated actions like blocking IPs or isolating compromised systems.
- **Scalability**: Testing the setup with multiple virtual machines and more complex enterprise environments.
