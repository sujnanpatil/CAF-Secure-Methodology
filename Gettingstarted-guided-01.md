# Getting Started with Your Microsoft Azure Infrastructure and Application Security Workshop

### Overall Estimated Duration : 60 Minutes

## Overview 

Organizations require robust tools to ensure secure administration and efficient management of network resources in the cloud. Azure offers a suite of services that enable comprehensive monitoring, visualization, and secure access to resources. This lab demonstrates how to utilize Azure Monitor Network Insights for real-time health monitoring, visualize network relationships using Azure Network Watcher, and securely connect to virtual machines through Azure Bastion. Additionally, it guides the configuration of NSG Flow Logs and diagnostic settings to capture and analyze network traffic for enhanced security and compliance.  

By completing this lab, you will gain practical experience in improving network security, troubleshooting connectivity issues, and monitoring traffic patterns to maintain a resilient and secure Azure environment.

## Objective  

**Secure Administration and Management**: Gain practical expertise in securing and managing Azure network resources by leveraging key Azure features and tools. Learn to monitor network health using Azure Monitor Network Insights, visualize the network topology with Azure Network Watcher, and establish secure access to virtual machines through Azure Bastion. Additionally, configure NSG Flow Logs and diagnostic settings to capture traffic data for comprehensive monitoring and analysis. This hands-on lab equips you with the skills needed to enhance the security, visibility, and efficiency of your Azure networking environment.

## Prerequisites

Participants should have: 

- **Understanding of Azure Networking Concepts**: Familiarity with virtual networks, subnets, and network security groups (NSGs) is essential for configuring and analyzing network topology and security.  

- **Knowledge of Azure Monitoring Tools**: Prior experience with tools like Azure Network Watcher and analyzing logs is necessary to set up monitoring environments and interpret NSG flow logs effectively.  

- **Secure Access Practices**: Understanding secure remote access methods, including Azure Bastion, to enable secure management of virtual machines and network resources.  

- **Troubleshooting Skills**: Basic troubleshooting knowledge to diagnose and resolve network health issues.

## Architecture

The architecture for this lab focuses on securing administration and managing Azure environments effectively. It integrates multiple Azure services to ensure comprehensive monitoring, secure access, and traffic analysis. The flow begins with monitoring network health and visualizing topology, then enforces secure access using a Bastion Host, and finally prepares a robust monitoring setup with Network Watcher and NSG Flow logs. This architecture ensures end-to-end visibility and secure management of the network environment.

## Architecture Diagram 

![](./images/Lab001.png) 

## Explanation of Components 

The architecture for this lab involves the following key components: 

- **Network Health:** Azure Monitor provides tools to track and visualize the performance and health of your Azure resources. It collects metrics, logs, and diagnostics to identify bottlenecks, latency, or downtime issues. With custom dashboards and alerts, you can proactively address potential network problems, ensuring seamless operations.  

- **Network Topology:** Azure Network Watcher's topology feature offers a graphical representation of your network resources, such as virtual networks, subnets, and connected devices. This visualization helps you understand your network structure and analyze connectivity issues, providing insights into the dependencies between resources.  

- **Secure Access via Bastion Host:** Azure Bastion is a secure and fully managed service that allows remote access to your virtual machines directly from the Azure portal without exposing RDP or SSH ports over the internet. This eliminates security risks associated with public IP exposure, ensuring safe administration of your VMs.  

- **Prepare the Monitoring Environment and NSG Flow:** NSG Diagnostic Logs offer comprehensive insights into the configuration, rules evaluation, and overall health of Network Security Groups, enabling the identification of misconfigurations and unauthorized access attempts. Additionally, NSG Flow Logs capture detailed traffic data, such as source and destination IPs, ports, and protocols, facilitating network traffic analysis, threat detection, and the investigation of security incidents to ensure secure and efficient network operations.  

## Getting Started with the Lab Environment

## Accessing Your Lab Environment

Once you're ready to begin, your virtual machine and lab guide will be available directly within your web browser.

![](./images/vm00100.png)

## Virtual Machine & Lab Guide

The virtual machine provides access to the Azure Portal and Microsoft security portals.  
The lab guide remains visible throughout the lab exercises.

## Exploring Your Lab Resources

Navigate to the **Environment** tab to review lab resources and credentials.

![](./images/env01.png)

## Utilizing the Split Window Feature

Use the **Split Window** button in the top-right corner to open the lab guide in a separate window for easier navigation.

![](./images/splitwin01.png)

## Managing Your Virtual Machine

Start, stop, or restart your virtual machine as needed from the **Resources** tab.

![](./images/RT1.png)

## Lab Guide Zoom In / Zoom Out

Adjust the zoom level using the **A↕ : 100%** icon located next to the timer.

![](./images/zoominout1.png)

## Let's Get Started with Azure Portal

1. On the virtual machine, click the **Azure Portal** icon:

    ![](./images/vm101.png)

1. On the **Sign in to Microsoft Azure** page, enter:

   - **Email/Username:** <inject key="AzureAdUserEmail" enableCopy="true"/>

       ![](./images/sign1.png)

1. Enter the password:

   - **Password:** <inject key="AzureAdUserPassword" enableCopy="true"/>

      ![](./images/tpwrd.png)

1. Select **No** when prompted to stay signed in.

   ![](./images/sign001.png)

## Support Contact

CloudLabs support is available 24/7 to assist learners and instructors.

- **Email:** cloudlabs-support@spektrasystems.com  
- **Live Chat:** https://cloudlabs.ai/labs-support  

Now, click on **Next** from the lower right corner to move on to the next page. 

![](./images/next.png)

### Happy Learning!!