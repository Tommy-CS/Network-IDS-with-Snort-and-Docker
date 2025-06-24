# That's Snort of a Lot of Rules: Network IDS with Snort & Docker
I built this lab as part of CodePath’s CYB102 cybersecurity course to gain hands-on experience with Snort, a signature-based Network Intrusion Detection System (NIDS). The goal was to simulate attacks using pytbull-ng and write custom Snort rules to detect and alert on malicious traffic in real time. After completing this project, I learned how Snort rules are written, tested, and deployed, and how packet analysis is used to secure networked systems.

## Tools & Technologies Used
- Ubuntu 22.04 LTS VM (hosted via Azure or local VirtualBox)
- Snort 3
- Docker (pytbull-ng attack simulation)
- Vim (for Snort config editing)
- Firefox (for HTTPS traffic testing)

## What This Lab Does
- Installs Snort in an Ubuntu VM and configures it to monitor network traffic.
- Uses Docker to simulate attack traffic using the pytbull-ng framework.
- Writes a custom Snort rule to detect HTTPS traffic to google.com.
- Tests Snort alerts by pinging and accessing websites to trigger detections.
- Modifies snort.lua to properly include local rules and enable built-in rule detection.

## Screenshots
### Generating attacks with pytbull-ng:
<img src="https://github.com/user-attachments/assets/19f559f4-7676-4a23-afa3-345e69fdce27" width="600"/>

###  Snort Detection Mode Triggered by ICMP Ping:
<img src="https://github.com/user-attachments/assets/0e98b4fc-4ecf-45b9-9d16-eea6089fc92c" width="600"/>

### Snort Rule Triggered! Blocking HTTPS Traffic to Google:
<img src="https://github.com/user-attachments/assets/8b4c56bc-5f44-421c-b3f4-298622008f84" width="600"/>


## Lessons Learned
Throughout this lab, I developed a deeper understanding of how IDS like Snort operate in real-time environments. I became comfortable writing and testing custom Snort rules, modifying its configuration files, and interpreting alerts triggered by simulated attacks. Setting up pytbull-ng helped me visualize what malicious traffic looks like and how an IDS detects it. Additionally, I improved my command-line proficiency, especially with tools like Vim and Docker, and gained practical experience managing network configurations and monitoring traffic on a virtual machine.
