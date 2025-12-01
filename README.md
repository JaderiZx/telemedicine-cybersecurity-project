Telemedicine Cybersecurity Project (Final Exam, Grade A)

A full cybersecurity implementation designed for a telemedicine environment, focusing on securing remote access, protecting patient data, detecting cyber threats, and meeting GDPR/HIPAA requirements.

This project includes real practical implementation using:
✔ Active Directory (RBAC, OU structure)
✔ Tailscale VPN
✔ Duo MFA
✔ Windows Firewall Segmentation
✔ Threat Simulation (Nmap, Kali Linux)
✔ Phishing Simulation (Gophish)
✔ Log Monitoring (Windows Event Viewer & Firewall Logs)

# Project Overview #

Healthcare systems are high-value targets due to sensitive patient data.
This project demonstrates how to secure a telemedicine infrastructure by:

Hardening remote access

Preventing lateral movement

Strengthening user authentication

Detecting attacks in real time

Training users against phishing

Ensuring compliance with GDPR & HIPAA

This was my final exam project at Noroff Institute of Technology, where I achieved Grade A.

# Lab Environment #

The project was implemented in a virtual lab using VMware:

Machine	Purpose
Server1 (Windows Server)	Active Directory, DNS
Server2 (Windows Server)	RDP, VPN, MFA, Firewall Segmentation
Windows 10 Client	Domain login testing
Kali Linux	Attack machine (Nmap, phishing dashboard)

# Security Measures Implemented #

✔ 1. Active Directory & Role-Based Access Control

Created domain telemed.local

Implemented role separation (Doctors vs IT Admins)

Applied Group Policies for passwords, lockout, login banners

✔ 2. Secure Remote Access

Installed Tailscale VPN (zero-config, encrypted tunnel)

No open ports on firewall (reduces attack surface)

Duo MFA enforced for RDP login

✔ 3. Network Segmentation

Windows Firewall rules used to block traffic from attacker (Kali)

One-way communication allowed only for server administration

Prevents lateral movement inside the network

✔ 4. Threat Simulation

Performed Nmap scans from Kali

Identified exposed services (RDP, SMB, DNS, etc.)

Verified firewall logs blocking attacks

✔ 5. Phishing Simulation

Created phishing email template using Gophish

Sent to test domain user

Demonstrated risks of credential harvesting

✔ 6. Monitoring & Logging

Enabled Windows Firewall logging

Used Event Viewer to track failed logins, scans, MFA attempts

# Proof of Concept (Screenshots) #

All screenshots documenting the work can be found here:

/screenshots/

Screenshots include:

AD user creation

Domain join

VPN setup

MFA enrollment

Firewall rules

Nmap attack scanning

Phishing dashboard

Log evidence

# Key Results #

MFA blocked unauthorized access even when credentials were known

VPN created a secure encrypted tunnel for remote staff

Segmentation prevented attackers (Kali) from scanning or moving laterally

Logs confirmed all attempted attacks were detected and blocked

Phishing test proved user awareness is critical

# Conclusion #

This project successfully demonstrated how a telemedicine company can secure remote operations and patient data by combining:

Strong authentication

Encrypted connections

Least privilege access

Network segmentation

Logging & monitoring

User training

This setup follows modern cybersecurity best practices and aligns with GDPR & HIPAA requirements.
