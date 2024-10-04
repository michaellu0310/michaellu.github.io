# Introduction
Welcome to my Portfolio

Hello and welcome! I am Michael! I’m a recent graduate from Rutgers University’s Computer Science program, where my lifelong passion for technology only grew & grew. It started me on a path that resulted in the CompTIA Security+ & ISC2 Certified in Cybersecurity certifications.

In this portfolio, you'll find an overview of projects focused on blue team roles & responsibilities that showcase my skills and expertise. Each project is documented to illustrate my methods, tools, and results. I hope you find my work both engaging and insightful!

[You can find all of my projects in their entirety on github](https://github.com/michaellu0310?tab=repositories)

Thank you for visiting!

# EDR Home Lab: Attack and Defense

## Overview

This project simulates real-world cybersecurity scenarios within a controlled lab environment, providing hands-on experience with SOC (Security Operations Center) operations. The lab setup includes an attacker machine running Linux Ubuntu and a victim machine running Windows 11, with Microsoft Defender disabled. The focus of the project is on endpoint detection and response (EDR), using Sliver for command-and-control operations and LimaCharlie as the EDR solution. Sysmon logs are imported to monitor and analyze system activities.

**Key Skills**: EDR, Incident Response, Sysmon, LimaCharlie, Sliver (Command and Control), Ubuntu, Linux, Windows 11, CLI, Log Analysis and Correlation, SIEM, Virtualization and VM Management

## Visuals

![Sliver-C2](https://github.com/user-attachments/assets/8a48095c-e7fb-401c-b75a-fa29f66640e4)
![Attack Privileges](https://github.com/user-attachments/assets/bfdea9d5-591c-4d09-b0e7-98f013ec8124)
![LimaCharlie-Detections](https://github.com/user-attachments/assets/d4cb0ce6-c667-4a07-b7a7-79fea6f73b1f)

### Challenges & Solutions

**Challenge**: Difficulty establishing a connection between the Sliver C2 server on the Ubuntu Linux machine and the Windows 11 machine using Port 80 (HTTP).

**Solution**: After researching and troubleshooting, I realized the issue was due to not having the necessary administrative privileges. By using the `sudo su` command to elevate my permissions on the Ubuntu machine, I was able to successfully establish the connection between the Sliver C2 server and the Windows 11 machine.

### Documentation

This project was executed using a structured approach based on [Eric Capuano's SOC Analyst guide](https://blog.ecapuano.com/p/so-you-want-to-be-a-soc-analyst-intro). While I followed the provided instructions, I also applied my technical skills to resolve unique challenges, such as establishing the Sliver C2 connection on Ubuntu Linux. The experience strengthened my ability to implement cybersecurity solutions in a controlled environment. For a detailed walkthrough of the setup, along with the adjustments I made, visit the [full project documentation on GitHub](https://github.com/michaellu0310/EDR-Attack-n-Defense).


# MasterCard Cybersecurity Virtual Experience

## Overview
This project is from [MasterCard Cybersecurity Virtual Experience](https://www.theforage.com/simulations/mastercard/cybersecurity-t8ye) focused on identifying phishing emails and creating educational content around them. I successfully analyzed suspicious emails to identify potential phishing attempts and then crafted a realistic phishing email scenario. To further reinforce the learning, I developed a PowerPoint presentation aimed at teaching employees how to recognize phishing emails and protect themselves from such threats. This experience has sharpened my skills in phishing detection, social engineering, and cybersecurity awareness training.

**Key Skills**: Phishing Detection, Social Engineering Techniques, Email Analysis, Threat Simulation, Cybersecurity Awareness Training, Presentation Skills

## Visuals
![Phishing-Detection](https://github.com/user-attachments/assets/baa14f01-2a88-4bdf-9abb-5ab01ef26ea1)
![Threat-Simulation](https://github.com/user-attachments/assets/d4bc6748-f8bb-4d4c-9093-18b9579cbfe8)
![Presentation](https://github.com/user-attachments/assets/ab772250-28bc-434a-b2a8-cde668694d41)

### Challenges & Solutions
Challenge #1: To able to contextualize the importance of the phishing email attempt for the specific employee without sounding suspicious.\
Solution #1: The phishing email was made to be sound more generic and bland which would push urgency to fix a problem that doesn't exist.


Challenge #2: Make the presentation not boring.\
Solution #2: Present data that would show who may be a victim to these phishing attempts so they are more inclined to follow along.


### Documentation
The project is following [MasterCard Cybersecurity Virtual Experience](https://www.theforage.com/simulations/mastercard/cybersecurity-t8ye). This experience breaks down the order in which a phishing campaign is done. Each learner's experience is different from another, I can only imagine how different  my phishing email and presentation may look from another. When these minds are working together in a team, we could have something incredible. [This experience documentation can be found on GitHub](https://github.com/michaellu0310/mastercard-forage-simulation).


# Intrusion Detection and Threat Analysis Lab

## Overview
This lab was made from scratch to simulate a real-world network attack focusing on detecting, logging, and analyzing threats in a controlled environment. The lab will involve creating two virtual machines: one running Kali Linux (acting as the attacker) and the other running Ubuntu (serving as the victim and network analyzer). The Kali Linux machine will utilize a backdoor Metasploit method to attempt exploit, while the Ubuntu machine will employ Snort as an IDS/IPS and logging solution, and Wireshark as a network analyzer.

Key Skills: IDS/IPS, Network Traffic Analysis, Snort, Metasploit, Wireshark, Kali Linux, Ubuntu, CLI, Virtualization and VM Network Configuration, Attack Simulation

## Visuals
![11-1](https://github.com/user-attachments/assets/64dc2f2f-9944-49ab-a4ef-6d915b3b7cd3)
![11-2](https://github.com/user-attachments/assets/1d99d651-3cd3-455d-a760-a40658f4fb37)
![27](https://github.com/user-attachments/assets/3f5b71ca-ea34-48e2-b29d-5e876e9400f3)
![28](https://github.com/user-attachments/assets/95477b90-74e6-4486-9958-512eea00289e)

### Challenges & Solutions

**Challenge #1:** Kali Linux did not have the proper tools to download anything on terminal such as installing metasploit.\
**Solution #1:** Kali Linux needed to install the debian package to get started for this project.

**Challenge #2:** When running ```sudo snort -T -i enp0s3 -c /etc/snort/snort.conf``` it said ```ERROR: /etc/snort/snort.conf(280) Unknown rule type: et. Fatal Error. Quitting..```\
**Solution #2:** Going back into snort.conf using vim and removing the extra typo lines when trying to exit vim.

**Challenge #3:** VMs utilizing same IP so I cannot ping to test snort.\
**Solution #3:** In VirtualBox, set each VM network setting to be Host-Only Ethernet Adapter.

**Challenge #4:** With the new IP Addresses both VMs refuses to talk to each other.\
**Solution #4:** In VirtualBox, create and set NAT Network for both machines.

**Challenge #5:** Finding var folder for snort logs.\
**Solution #5:** Press CTRL+H in file explorer to show hidden folders.

### Documentation
Metasploit is one of the most used penetrating testing framework with a lot of ways to exploit networks. Snort and Wireshark are free powerful tools to use for network security, pairing it with Metasploit makes it a great project combination. More for this project can be found on the [full documentation on GitHub](https://github.com/michaellu0310/Intrusion-Detection-and-Threat-Analysis-Lab).

# C-Bot

## Overview
Currently developing a logging bot for a social media community of 300+ members, utilizing Python, Tesseract/EasyOCR, AWS, and GitHub in collaboration with a team.

Key Skills: Python, Pytesseract/EasyOCR, AWS, Discord Bot, Logging, Spreadsheet

### Documentation
This project is in high demand across thousands of similar communities. The GitHub page for this project is currently unavailable.
