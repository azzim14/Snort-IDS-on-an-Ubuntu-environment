# Snort-IDS-on-an-Ubuntu-environment

## Objective

The objective of this project was to deploy and configure Snort Intrusion Detection System (IDS) on an Ubuntu environment to gain hands-on experience with network traffic monitoring and intrusion detection.
Specifically, the project aimed to:
Install and configure Snort on Ubuntu Linux
Understand how Snort analyzes network packets using rules and signatures
Detect and log suspicious or policy-violating network activity
Test alert generation and review Snort logs for analysis
Build foundational skills in IDS concepts, network security monitoring, and log interpretation
This project was completed as part of my cybersecurity learning and home lab practice to strengthen practical defensive security skills.

### Skills Learned

- Network Security Monitoring (NSM)
- Writing and tuning Snort IDS rules
- Understanding packet structure and protocol behaviors
- Hands-on blue team detection workflow
- Attack simulation and traffic analysis
- Using Linux for defensive security

### Tools Used

- Ubuntu Machine
- Network analysis tools (such as Wireshark) for capturing and examining network traffic.


## Steps
Installed & Configured Snort on Ubuntu

I successfully installed Snort from the official repositories and performed the base configuration, including:
Verifying network interfaces
Updating Snort rules and directories
Creating a custom snort.conf file
Setting up Snort to run in packet-logging mode

 2. Wrote Custom Snort Rules

To better understand how detection logic works, I manually wrote several custom rules to detect:
ICMP Echo Requests (ping)
HTTP GET requests
SSH connection attempts
This helped me understand rule syntax, metadata, and how Snort matches patterns during packet inspection.

3. Attack Simulation Using Kali Linux

To validate the setup, I used a Kali Linux machine as an attacker and ran:
ICMP ping sweeps
Curl-based HTTP GET requests
SSH connection attempts
Nmap scans for reconnaissance

As soon as the traffic hit the Ubuntu machine, Snort immediately triggered alerts, displaying realtime event logs directly in the terminal. Seeing my custom rules fire during the tests was rewarding.

4. What This Project Strengthened

Network Security Monitoring (NSM)
Writing and tuning Snort IDS rules
Understanding packet structure and protocol behaviors
Hands-on blue team detection workflow
Attack simulation and traffic analysis
Using Linux for defensive security

This project was a great way to combine offensive simulation with defensive monitoring. I’m continuing to build more detection rules and automate alerts as I expand my SOC cybersecurity lab.

If anyone is building a similar home lab or wants the full step-by-step guide, feel free to reach out!


<img src="https://i.postimg.cc/y6XwqdG9/Whats-App-Image-2025-12-11-at-7-57-34-PM.jpg" height="80%" width="80%" alt="Snort"/>
<img src="https://i.postimg.cc/5ND5n5mj/Whats-App-Image-2025-12-11-at-7-57-36-PM.jpg" height="80%" width="80%" alt="ICMP ping sweep from another tab"/>
<img src="https://i.postimg.cc/tC626C01/Whats-App-Image-2025-12-11-at-7-57-38-PM.jpg" height="80%" width="80%" alt="ICMP ping detection alert"/>
<img src="https://i.postimg.cc/QCGWZDfc/Whats-App-Image-2025-12-11-at-7-57-38-PM-(1).jpg" height="80%" width="80%" alt="Nmap scans for reconnaissance from Kali linux machine"/>

