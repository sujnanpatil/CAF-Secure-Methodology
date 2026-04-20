# Getting Started with Your Microsoft Azure Infrastructure and Application Security Workshop

### Overall Estimated Duration : 2 hours 30 Minutes

## Overview 

This lab focuses on improving the security and performance of web applications using Azure's network and application protection services. You'll explore **Azure Firewall**, which provides scalable, stateful protection for Azure Virtual Network resources, and **Azure Application Gateway** with **Web Application Firewall (WAF)**, which protects against common web vulnerabilities like SQL injection and XSS attacks.

In this exercise, you’ll deploy and configure Azure Firewall, Application Gateway with WAF, and Azure Front Door to secure a sample application. Key tasks include setting up WAF for protection, creating custom rules to block IPs, simulating attacks, and applying rate limiting with Azure Front Door to optimize and secure the application.

## Objective  

**Secure Application:** Learn to configure **Web Application Firewall (WAF)** to protect your web application and ensure its security. Gain hands-on experience in accessing your application using **Azure Application Gateway**. Learn how to create **custom rules in Application Gateway WAF** to block specific IP addresses and protect against potential threats. Simulate attacks to test your application’s security measures and implement **rate limiting** using **Azure Front Door** to control traffic and prevent overloading. This lab will help you understand and apply best practices to secure and optimize web applications hosted on Azure.

## Prerequisites

Participants should have:

- **Basic Knowledge of Microsoft Azure:** Familiarity with the Azure portal and working with virtual networks, web applications, and cloud security.
- **Understanding of Web Application Security:** Basic understanding of web application vulnerabilities and security practices like WAF and rate limiting.
- **Familiarity with Azure Networking Services:** Knowledge of services like Azure Front Door and Application Gateway.
- **Basic Experience with Azure Firewall:** Understanding of how to configure and manage network security in Azure.

## Architecture

The architecture begins with configuring Azure Application Gateway to serve as the front-end for the web application, followed by adding the Virtual Machine to the backend pool of the Application Gateway. The Application Gateway is also configured with a Firewall Policy, which secures the application by applying security rules. After setting up the Application Gateway, users can access the application through this secure entry point.

Next, Application Gateway WAF Custom Rules are created to block specific IPs, such as the Lab VM’s public IP, ensuring that only authorized traffic can access the application. Once security is in place, an Attack Simulation is performed, testing the application for vulnerabilities like Cross-Site Scripting (XSS), where malicious scripts are injected into the application to assess its resilience.

Finally, to ensure performance and security, Azure Front Door is deployed with rate limiting enabled to regulate traffic and ensure that the application can handle high loads while maintaining security across multiple regions. This configuration ensures that traffic is directed to the nearest application instance and can automatically failover in case of regional unavailability.

## Architecture Diagram 

![](./images/Lab002.png) 

## Explanation of Components 

The architecture for this lab involves the following key components: 


- **Azure Application Gateway**: Acts as the entry point for the web application, routing traffic to the backend. It integrates with Web Application Firewall (WAF) to inspect incoming traffic and prevent malicious attacks, such as SQL injection and XSS, ensuring a secure application environment.

- **Web Application Firewall (WAF)**: Integrated with both Azure Application Gateway and Azure Front Door, the WAF helps protect the web application from threats and vulnerabilities by filtering and blocking malicious traffic based on custom security policies. It ensures the application remains secure from a range of attacks.

- **Azure Front Door**: A global load balancer and traffic manager that ensures high availability and low latency for the application by routing traffic to the nearest region. It provides an additional layer of security through its own WAF and rate limiting features, preventing abuse by controlling the number of requests a client can make within a specified time frame.

- **Azure Virtual Machines (VMs)**: Hosts the backend services of the application, providing the necessary compute resources for processing requests and serving the application content. These VMs are protected by the Application Gateway and WAF to ensure that only secure traffic reaches the backend.

- **Rate Limiting (via Azure Front Door)**: This feature controls the number of requests that a client can make within a specific time period, protecting the application from Denial of Service (DoS) attacks. Rate limiting ensures the application remains responsive and maintains a smooth user experience, even under heavy traffic conditions.

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