
# ELASTIC SIEM LAB

## Objective

The Elastic SIEM lab project is meant to establish a controlled environment for simulating and detecting cyber attacks. The primary focus was to ingest and analyze logs within a Security Information and Event Management (SIEM) system, generating test telemetry to mimic real-world attack scenarios. This hands-on experience was designed to deepen my understanding of network security, attack patterns, and defensive strategies.

### Skills Learned

- Setup and configuration of an elastic stack SIEM
- Developing a custom dashboard for security events
- Demonstrate profieciency in deploying a Kali Linux VM
- Advanced understanding of SIEM concepts and practical application.
- Proficiency in analyzing and interpreting network logs.
- Ability to generate and recognize attack signatures and patterns.
- Enhanced knowledge of network protocols and security vulnerabilities.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used

- Security Information and Event Management (SIEM) system for log ingestion and analysis.
- Network analysis tool for capturing and examining network traffic.
- Telemetry generation tool to create realistic network traffic and attack scenarios.
- Kali Linux
- Elastic Cloud 

## Steps

1. Set up an Elastic account at https://cloud.elastic.co.
2. Download & Install the Kali VM https://www.kali.org/get-kali/#kali-virtual-machines. <br> <img src="https://github.com/user-attachments/assets/c6aa5654-8672-4388-a757-7fa0260a0612" width="400" height="300"/>
3. Run the KaliVM on the virtualization platform (VirtualBox in this case). <br> <img src="https://github.com/user-attachments/assets/c97fedb0-ad1c-43d5-bfbc-5e0c5faa5adb" width="400" height="300"/>
4. Setup the Elastic Agent by adding an integration and selecting the "Elastic Defend" option. <br> <img src="https://github.com/user-attachments/assets/fd2f7314-b31c-4b21-95e9-b1ea2292410d" width="400" height="300"/>

5. Copy the "Linux Tar" command to your clipboard and paste the command into the Kali terminal. Make sure to use the sudo command to install the program. <br> <img src="https://github.com/user-attachments/assets/8cbda3ef-1e80-4302-968c-ce0134c9d472" width="400" height="300"/>



6. Run a few Nmap scans on the terminal using the commands; "nmap -sS", "nmap -sT", "nmap -p-". This will generate security events such as the detection of open ports. <br> <img src="https://github.com/user-attachments/assets/7947ce60-1559-4cd4-9155-b93b558346d2" width="400" height="300"/>


7. Return to the Elastic SIEM and make sure that logs are correctly displayed and showing up by navigating to the "logs" tab. <br> <img src="https://github.com/user-attachments/assets/ea2225eb-56ce-4856-bb43-f7aec07c71bf" width="400" height="300"/>

8. Create a Dashboard to visualize security events. <br> <img src="https://github.com/user-attachments/assets/3a022ed6-daf5-46bb-8101-7c6ccd87a2d0" width="400" height="300"/>



9. Create a custom query in the "Security" section in elastic lab using the following query: <br> <img src="https://github.com/user-attachments/assets/036890e4-129f-494c-9d12-b8b7575843c3" width="700" height="100"/>

10. The above query should monitor your logs for any Nmap scan events and trigger an alert.

## Conclusion
In this lab, I demonstrated the process of setting up an Elastic account and integrating it with a Kali virtual machine to monitor security events. By installing and running Kali VM on VirtualBox, I set the foundation for simulating real-world scenarios where security monitoring is critical. I configured the Elastic Agent with the "Elastic Defend" integration to ensure that system activity could be tracked and logged.

Through executing Nmap scans, I generated network traffic and security events, which were then captured by Elastic’s SIEM (Security Information and Event Management). This allowed me to visualize the collected data using dashboards and custom queries, providing insights into network activity. The custom query is useful in identifying potential threats like Nmap scans.

Overall, I created a comprehensive monitoring setup using Elastic's SIEM, leveraging visualizations and custom queries to enhance visibility into security events. This setup is valuable for detecting potential vulnerabilities and responding to security incidents effectively.


