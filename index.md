# Introduction
Welcome to my Portfolio

Hello and welcome! I'm Michael, a cybersecurity enthusiast with a solid background in computer science. Initially, I aimed to be a Software Engineer, but my passion shifted towards threat hunting and incident response, guiding me towards a career as a SOC Analyst. I am particularly drawn to Cloud Security (and perhaps Cloud Security Engineer) because the Cloud is a central part of modern IT infrastructure, and securing it is crucial for protecting sensitive data. Additionally, my ability to work around the clock aligns perfectly with the demands of a SOC Analyst role, where vigilance and adaptability are key.

In this portfolio, you'll discover a range of projects that showcase my skills and expertise. Each project is carefully documented to illustrate my methods, tools, and results. I hope you find my work both engaging and insightful.

Feel free to explore the detailed documentation and reach out if you have any opportunities!

[You can find all of my projects here as well](https://github.com/michaellu0310?tab=repositories)

Thank you for visiting!

# SOC Analyst Home Lab Project

## Overview

This project simulates real-world cybersecurity scenarios within a controlled lab environment, providing hands-on experience with SOC (Security Operations Center) operations. The lab setup includes an attacker machine running Linux Ubuntu and a victim machine running Windows 11, with Microsoft Defender disabled. The focus of the project is on endpoint detection and response (EDR), using Sliver for command-and-control operations and LimaCharlie as the EDR solution. Sysmon logs are imported to monitor and analyze system activities.

**Key Skills**: EDR, Incident Response, Sysmon, LimaCharlie, Sliver (Command and Control), Ubuntu, Linux, Windows 11, CLI, Log Analysis and Correlation, SIEM, Virtualization and VM Management

## Visuals

![Sliver-C2](https://github.com/user-attachments/assets/8a48095c-e7fb-401c-b75a-fa29f66640e4)
![Attack Privileges](https://github.com/user-attachments/assets/bfdea9d5-591c-4d09-b0e7-98f013ec8124)
![LimaCharlie-Detections](https://github.com/user-attachments/assets/d4cb0ce6-c667-4a07-b7a7-79fea6f73b1f)

### My Role

In this project, I was responsible for designing, configuring, and executing both offensive and defensive cybersecurity operations within the home lab. I set up and managed the virtual machines, deployed Sliver as the C2 framework on the Ubuntu machine, and implemented LimaCharlie on the Windows machine as the EDR solution.

### Challenges & Solutions

**Challenge**: Difficulty establishing a connection between the Sliver C2 server on the Ubuntu Linux machine and the Windows 11 machine using Port 80 (HTTP).

**Solution**: After researching and troubleshooting, I realized the issue was due to not having the necessary administrative privileges. By using the `sudo su` command to elevate my permissions on the Ubuntu machine, I was able to successfully establish the connection between the Sliver C2 server and the Windows 11 machine.

### Documentation

This project was executed using a structured approach based on [Eric Capuano's SOC Analyst guide](https://blog.ecapuano.com/p/so-you-want-to-be-a-soc-analyst-intro). While I followed the provided instructions, I also applied my technical skills to resolve unique challenges, such as establishing the Sliver C2 connection on Ubuntu Linux. The experience strengthened my ability to implement cybersecurity solutions in a controlled environment. For a detailed walkthrough of the setup, along with the adjustments I made, visit the [full project documentation on GitHub](https://github.com/michaellu0310/SOC-Analyst-Home-Lab).
