# Microsoft 365 Defender Suite

## Overview

Microsoft 365 Defender is an integrated security suite designed to offer comprehensive protection across various Microsoft 365 services. It brings together multiple security solutions to provide advanced threat protection, detection, and response capabilities.


### Key features of Microsoft Sentinel

- Microsoft Defender for Endpoint: Defender for Endpoint is a unified endpoint platform for preventative protection, post-breach detection, automated investigation, and response.
- Microsoft Defender for Office 365: Defender for Office 365 safeguards your organization against malicious threats posed by email messages, links (URLs) and collaboration tools.
- Microsoft Defender for Identity: Microsoft Defender for Identity is a cloud-based security solution that leverages your on-premises Active Directory signals to identify, detect, and investigate advanced threats, compromised identities, and malicious insider actions directed at your organization.
- Microsoft Defender for Cloud Apps: Microsoft Defender for Cloud Apps is a comprehensive cross-SaaS solution bringing deep visibility, strong data controls, and enhanced threat protection to your cloud apps.
- Microsoft Defender Vulnerability Management: Microsoft Defender Vulnerability Management delivers continuous asset visibility, intelligent risk-based assessments, and built-in remediation tools to help your security and IT teams prioritize and address critical vulnerabilities and misconfigurations across your organization.
- Microsoft Entra ID Protection: Microsoft Entra ID Protection helps organizations detect, investigate, and remediate identity-based risks. These identity-based risks can be further fed into tools like Conditional Access to make access decisions or fed back to a security information and event management (SIEM) tool for further investigation and correlation.
- Microsoft Data Loss Prevention: In Microsoft Purview, you implement data loss prevention by defining and applying DLP policies. With a DLP policy, you can identify, monitor, and automatically protect sensitive items
- App Governance: App governance in Defender for Cloud Apps is a set of security and policy management capabilities designed for OAuth-enabled apps registered on Microsoft Entra ID, Google, and Salesforce.

## Sandbox Scenario
Contoso is a global organization with a complex IT infrastructure that includes a combination of on-premises data centers and cloud-based resources. They are looking to enhance their security posture by deploying Azure Sentinel, Microsoft's cloud-native security information and event management (SIEM) and security orchestration automation and response (SOAR) solution. Additionally, Contoso aims to onboard its cloud resources and servers to Azure Sentinel to gain better visibility and proactive threat detection and response capabilities.

By implementing a robust log analytics and threat detection program, Contoso aims to proactively identify and mitigate threats, reduce the risk of security breaches, and maintain a strong security posture in an ever-evolving threat landscape. This approach will enable Contoso to stay ahead of potential threats and protect its digital assets effectively.

## About the Sandbox

Using this environment, You'll be able to explore complete features and offerings offered by Microsoft Sentinel. Please find the detailed overview of the sandbox environment below.

### Pre-provisioned resources

#### **Virtual Machines**: 

- 2 *Windows Server 2019 Datacenter* Virtual machines, virtual machine-related resources like Virtual networks, Network security groups, managed disks, Network interface cards, and IP addresses are deployed as part of the automation.

  You are recommended to use the same virtual machine throughout the lab for the best experience through out the lab.

#### **License and subscription**: 

- You'll have access to a pre-configured Microsoft user account with an active Azure subscription, a tenant, and a Microsoft 365 E5 license assigned to the user. 
   
  User account has assigned as Owner at subscription and Global administrator at the tenant level. You need to use the same user account throughout the lab to get the most out of the lab. 

#### **Azure Credits**: 

- You have been given a quota of **$83 USD** which includes the running cost of Pre-deployed resources, license cost, and other resources deployed while running through the lab.

  You will receive **cost alerts** to your registered email address at **50%/75%/90%/95%/100%** of the allotted Azure Credit is spent.

  You can visit the Azure Subscription page to check the current Azure credit spend and Analysis on **Cost analysis** tab under the Cost Management option.

  ![Picture 1](../media/o1.jpg)

#### **Duration and Deletion of sandbox**:  

- The sandbox environment will be active for **30 days/730** hours from the time of registration. 
- The allowed uptime of the virtual machine is **40 hours**.
- The virtual machines will automatically **shut down** if not in use or if virtual machines are left idle. This feature is enabled in virtual machines to minimize the Azure spend.
- when 100% of Azure credits are spent, the sandbox environment will get automatically deleted without any prior notification. To retain the environment for a longer period and to get the most out of the environment, please follow the best practices mentioned below.

#### **Best practices**: 

- **Resources usage**: Please stop the virtual machines and other resources when not in use in order to minimize the Azure spend.

- **Azure Cost Analysis**: Maintain a practice of checking the Cost Analysis report of the assigned Azure subscription oftenly in check the Azure spend so that enviornment for a longer duration of time.

- **Alert notifications**: Make sure to check your registered email's inbox for any alert-related mails. Alerts give you can head start to keep your Azure spending in control and to plan out the remaining credits in the best way possible.

## Using this Sandbox

In this sandbox environment, You'll have access to a predeployed environment with an active Azure subscription, a tenant, and a Microsoft 365 E5 license assigned to the user. 

Using this environment, You'll be able to explore complete features and offerings offered by Microsoft 365 Defender Suite.

The lab scenarios are given as reference material to assist you in getting started with the exploration. You are encouraged to explore Microsoft 365 Defender Suite further based on your interests and preferences.


## Lab Guide Contents:
You will have access to a lab guide which is a reference material to assist you in getting started with the exploration. You are encouraged to explore Microsoft Defender further based on your interests and preferences.

- Lab 01 - Explore Microsoft Defender Portal 
- Lab 02 - Configure Email authentication
- Lab 03 - Configure Protection Policies (Anti-Spam, Anti-malware and Anti-phishing) 
- Lab 04 - Configure Priority accounts.  
- Lab 05 - Configure block/allow lists. 
- Lab 06 - Launch phishing simulation campaigns. 
- Lab 07 - Create Incidents 
- Lab 08 - Detect & Investigate threats
- Lab 09 - Discover Apps 
- Lab 10 - Configure App Access Policies 
- Lab 11 - Setup Alerts & App Governance 
- Lab 12 - Investigate Alerts and activities
- Lab 13 - Deploy Domain Controller 
- Lab 14 - Setup Defender for Identity Sensors 
- Lab 15 - Download and schedule defender for identity reports.

### Azure services and related products

- Microsoft Defender for Office 365
- Microsoft Defender for Cloud Apps
- Microsoft Defender for Identity
