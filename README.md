# MicrosoftSentinel (SIEM)
## Descirption
Discover the power of Microsoft Sentinel with this step-by-step guide showcasing my work. I successfully set up Microsoft Sentinel as a Security Information and Event Management (SIEM) system and connected it to a live virtual machine that acted as a honeypot. Real-time attacks, including RDP Brute Force, were observed from various parts of the world. A custom PowerShell script was utilized to identify the attacker's geolocation information and I was able to visualize it on the Azure Sentinel map through detailed screenshots
# Languages and Utilities Used
• PowerShell
# Environments Used 
• Microsoft Sentinel
# Project walk-through
1. Setting up a VM in Azure:![image](https://github.com/ShaneAlves/Microsoft-Sentinel-SIEM-Homelab/assets/111554296/d13fd193-cab7-45c2-8425-df3068a967a4)


2. Created firewall rules to accept all ngress and degress traffic:![68747470733a2f2f692e696d6775722e636f6d2f715369416858412e706e67](https://github.com/ShaneAlves/Microsoft-Sentinel-SIEM-Homelab/assets/111554296/dac34f1a-4ce4-4440-89f5-e29a9eca1358)

3. Created a Log Analytics workspace:
 # ![image](https://github.com/ShaneAlves/Microsoft-Sentinel-SIEM-Homelab/assets/111554296/ddbb774a-b656-465a-b526-2b8f8e228f8b)

4. Connected Log Analytics to VM (No Picture)

5. Setting up Sentinel, connecting VM Previously Created:![68747470733a2f2f692e696d6775722e636f6d2f686447694562492e706e67](https://github.com/ShaneAlves/Microsoft-Sentinel-SIEM-Homelab/assets/111554296/b8474b1d-bb4e-4c49-a060-30a94377f083)

6. Connecting to VM through Remote Desktop:![image](https://github.com/ShaneAlves/Microsoft-Sentinel-SIEM-Homelab/assets/111554296/dd3707d2-9c65-422e-b4e3-d8e3135eeddb)

7. Pinging VM to validate traffic flow:![image](https://github.com/ShaneAlves/Microsoft-Sentinel-SIEM-Homelab/assets/111554296/6c5247d3-a1d3-4a47-b7ca-8fb71d470f9a)

8. Executing a Powershell Strip (Propagates all Event-logs-Security Logs and failed login events and creates a new logfile):![image](https://github.com/ShaneAlves/Microsoft-Sentinel-SIEM-Homelab/assets/111554296/9621a329-e7a3-4e8b-b80e-667192927c09)

9. Log Created after running Powershell strip:![image](https://github.com/ShaneAlves/Microsoft-Sentinel-SIEM-Homelab/assets/111554296/4e234e24-e60f-4084-81d0-218a12f70e42)

10. Creating Custom logfile to train log analytics what to look for in the logfile:![image](https://github.com/ShaneAlves/Microsoft-Sentinel-SIEM-Homelab/assets/111554296/0a0124e7-8c24-43e2-addf-af7494dbc932)

11. Ensuring successful delivery of logs: ![image](https://github.com/ShaneAlves/Microsoft-Sentinel-SIEM-Homelab/assets/111554296/2e014d77-1472-4857-8e45-2626f8f7f78d)

12. Setting up World MAP:![image](https://github.com/ShaneAlves/Microsoft-Sentinel-SIEM-Homelab/assets/111554296/09fc7a03-2bb5-40bd-8fb0-b1c24e0bc88b)

13. Reviewing Powershell strip again, Identified brute force attempts:![image](https://github.com/ShaneAlves/Microsoft-Sentinel-SIEM-Homelab/assets/111554296/7973781e-955b-48f3-84a8-fdead5db5444)
![image](https://github.com/ShaneAlves/Microsoft-Sentinel-SIEM-Homelab/assets/111554296/7bc95a73-1ae7-4785-9dda-6e53fdf17d84)
