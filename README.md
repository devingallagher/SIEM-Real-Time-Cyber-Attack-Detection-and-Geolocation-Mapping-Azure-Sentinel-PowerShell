This project demonstrates the implementation of a Security Information and Event Management (SIEM) system using Microsoft Azure Sentinel to monitor and visualize cyber attack activity in real-time. The project focuses on detecting and analyzing Remote Desktop Protocol (RDP) brute-force attacks, providing actionable insights into potential cybersecurity threats.

Features
Attack Detection: Monitors RDP brute-force attempts by using a custom PowerShell script that extracts key metadata from the Windows Event Viewer.
Geolocation Tracking: Extracted data is processed through a third-party API to retrieve geolocation details, identifying the origin of detected attacks.
Real-Time Visualization: Attack data is displayed on a dynamic world map via Microsoft Sentinel, showcasing frequency and geographic distribution of attacks.
High-Volume Data Insights: Recorded over 12,000 attack attempts originating from 10 distinct locations within the first 24 hours of deployment.
Objective
The goal of this project is to enhance cybersecurity threat detection by leveraging SIEM technology and cloud-based visualization tools. The setup provides a detailed overview of global cyber threats, enabling better analysis of attack patterns and identification of potential vulnerabilities in network defenses.

Additional Sections
Deployment Overview
SIEM Setup on Microsoft Sentinel:

Connected Sentinel to a virtual machine (VM) running Windows Server.
Configured data connectors for Windows Event logs to track RDP activity.
PowerShell Script:

Developed a script to filter and forward relevant Event Viewer logs (e.g., Event ID 4625 for failed login attempts).
Integration with Geolocation API:

Used a geolocation API to map IP addresses to geographic locations for better visualization of attack origins.
Visualization and Alerting:

Created custom Log Analytics queries and workbooks in Azure Sentinel to visualize attack trends on a world map and set up alerting rules.
Key Learnings
Understanding the architecture and functionality of a SIEM solution.
Practical experience in deploying and configuring Microsoft Sentinel for security monitoring.
Insights into RDP brute-force attack patterns and mitigation strategies.
Effective use of scripting and APIs to enrich security data with actionable insights.
Future Enhancements
Expand Threat Detection: Add detection for additional attack vectors such as SSH brute-force, port scans, or malware downloads.
Advanced Analytics: Use machine learning models in Sentinel to predict and classify threats based on historical data.
Automated Responses: Implement Azure Logic Apps to trigger automated responses, such as blocking malicious IPs or sending alerts.
Credit:
Inspiration for this project was drawn from this video tutorial.
