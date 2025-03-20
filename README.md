# Live-Attack-Simulation-in-Azure-SOC-using-Microsoft-Sentinel-March-2025


# Live-Attack-Simulation-in-Azure-SOC-using-Microsoft-Sentinel

## Overview

In this project, I built a **Live Attack Simulation** environment using **Azure** and **Microsoft Sentinel** for a **Security Operations Center (SOC)**. The goal of this project is to simulate real-world cyber-attacks and demonstrate how security operations teams can detect, monitor, and respond to these attacks in real time. The project leverages **Azure resources**, **Log Analytics Workspaces**, and **Microsoft Sentinel** for collecting, analyzing, and visualizing logs to improve threat detection and incident management.

## Steps Taken

### 1. Setting Up an Azure Subscription

The first step was setting up an **Azure subscription** followed by creating a **Resource Group** to organize all the resources. A **Virtual Machine (VM)** was deployed and exposed to the internet, which acts as a **honeypot** to attract and simulate attack attempts.

![Resource Group Creation](https://drive.google.com/file/d/10XRWKEzvbekh4_MBD4T2qt7iMt9lf46N/view?usp=drive_link)

---

### 2. Configuring Log Analytics Workspace

A **Log Analytics Workspace** was created in Azure to collect logs from the virtual machine and other Azure resources. This workspace is essential for centralizing log data, which is required for monitoring and performing security analysis.

![Log Analytics Workspace Setup](path-to-your-uploaded-image3)

---

### 3. Integrating Microsoft Sentinel

Next, **Microsoft Sentinel** was integrated into the environment to provide real-time threat detection capabilities. Sentinel uses advanced analytics and machine learning to automatically detect threats and provide insights into the collected logs from the Log Analytics Workspace.

![Sentinel Integration](path-to-your-uploaded-image4)

---

### 4. Attack Simulation and Querying

Custom **KQL (Kusto Query Language)** queries were written to detect suspicious activities such as **failed login attempts** and other indicators of compromise (IOCs). These queries were then configured to trigger alerts when certain conditions were met, providing security teams with the necessary data to investigate potential threats.

![Custom Detection Rules](path-to-your-uploaded-image7)

---

### 5. Building the Attack Map

An **Attack Map** was created to visualize the geographic source of the simulated attacks. This feature provides valuable insights into attack patterns and allows security teams to monitor attacks from specific regions in real-time.

![Attack Map Visualization](path-to-your-uploaded-image5)

---

### 6. Incident Management

Once an attack is detected, it is logged into the **Incident Management Dashboard**. This dashboard provides an overview of the incident's details, including its severity, the affected systems, and actions to mitigate the impact. It is a central point for security teams to prioritize and respond to incidents.

![Incident Management](path-to-your-uploaded-image6)

---

## Technologies Used

- **Azure**: A cloud platform that provides the infrastructure for hosting virtual machines, networks, and security monitoring tools.
- **Microsoft Sentinel**: A SIEM (Security Information and Event Management) solution used for threat detection, investigation, and response.
- **Log Analytics Workspace**: A service in Azure that collects, organizes, and analyzes logs from various Azure resources.
- **KQL (Kusto Query Language)**: The language used to write custom queries for analyzing logs in Sentinel and Log Analytics.

---

## Screenshots of the Project

Here are key screenshots showing the steps and features implemented in the project:

### 1. Resource Group Creation

A **Resource Group** was created to organize all resources, such as virtual machines and security monitoring tools.

![Resource Group Creation](path-to-your-uploaded-image1)

---

### 2. Virtual Machine Creation

A **Virtual Machine (VM)** was deployed to act as a honeypot, simulating a vulnerable target for attack attempts.

![Virtual Machine Creation](path-to-your-uploaded-image2)

---

### 3. Log Analytics Workspace Setup

The **Log Analytics Workspace** collects and organizes logs from all Azure resources, enabling detailed security analysis.

![Log Analytics Workspace Setup](path-to-your-uploaded-image3)

---

### 4. Sentinel Integration

**Microsoft Sentinel** was configured to integrate with the **Log Analytics Workspace**, enabling automated threat detection and analysis.

![Sentinel Integration](path-to-your-uploaded-image4)

---

### 5. Attack Map Visualization

The **Attack Map** provides a real-time visualization of attack sources on a global scale, helping security teams track the geographic distribution of attacks.

![Attack Map Visualization](path-to-your-uploaded-image5)

---

### 6. Incident Management

The **Incident Management Dashboard** allows security teams to manage and prioritize security incidents detected in the environment.

![Incident Management](path-to-your-uploaded-image6)

---

## Conclusion

The **Live-Attack-Simulation-in-Azure-SOC-using-Microsoft-Sentinel** project demonstrates how Azure and Sentinel can be leveraged to create an effective security operations center. The integration of threat detection, log collection, and incident management provides a comprehensive solution for monitoring and responding to cyber-attacks. The project also highlights the power of **KQL queries** and **visualization tools** such as **attack maps** to help security teams quickly identify and respond to emerging threats.

---

## Future Improvements

- **Enhanced Detection**: Adding additional detection rules and integrating other Azure services for deeper insights into network activity.
- **Automation**: Implementing automated responses to common threats, such as blocking IPs or isolating compromised virtual machines.
- **Scalability**: Expanding the solution to cover multiple virtual machines and larger network setups to simulate a more complex enterprise environment.

---

### License

This project is licensed under the MIT License. See the LICENSE file for more details.

---

### How to Use

1. **Fork this repository** to clone the project to your own GitHub account.
2. **Set up an Azure subscription** and create the required resources (Resource Groups, Virtual Machines, Log Analytics Workspaces, etc.).
3. **Integrate Microsoft Sentinel** and use the **KQL queries** to begin detecting, monitoring, and responding to simulated cyber-attacks.

---

Make sure to replace the **image paths** with the correct file locations in your GitHub repository. You can add this markdown content to your repository's **README.md** file to present the project.

Let me know if you need any further changes or additions to this!
