 Windows Fundamentals — Security-Focused Overview
 Overview

This repository documents what I learned from the Windows Fundamentals room on TryHackMe, with a focus on how Windows systems work from a security perspective. The goal is to demonstrate understanding of Windows users, permissions, processes, and why misconfigurations can lead to security issues.

 Key Concepts Learned
1. Windows Users & Accounts

Windows uses user accounts to control who can access a system and what actions they’re allowed to perform.

Standard users have limited permissions

Administrators can install software, change system settings, and manage other users

 Why this matters:
If an attacker gains admin access, they effectively control the system.

2. User Groups & Privileges

Users are placed into groups (such as Administrators or Users), which define their permissions.

Permissions are inherited through group membership

Misconfigured group assignments can lead to privilege escalation

 Security risk:
A regular user mistakenly added to the Administrators group gives attackers a shortcut to full system control.

3. Windows Processes & Services

Windows runs many background processes and services to keep the system functioning.

Services often run with elevated privileges

Attackers may abuse vulnerable or misconfigured services to gain persistence

 Security takeaway:
Suspicious or unfamiliar processes can indicate malware or unauthorized activity.

4. File System & Permissions

Windows uses NTFS permissions to control access to files and directories.

Permissions include:

Read

Write

Modify

Full Control

 Why this matters:
Improper permissions can allow attackers to read sensitive data or modify system files.

 Security Relevance

This room helped me understand why Windows systems are common attack targets and how attackers exploit:

Weak user permissions

Excessive admin access

Poorly secured services

Inadequate file permission management

Understanding these basics is essential for:

Incident response

Threat detection

Hardening Windows environments

 Hands-On Experience

Through hands-on labs, I explored:

Windows user and group management

System processes and services

Permission structures within Windows

This reinforced how small configuration mistakes can escalate into serious security vulnerabilities.

 Key Takeaway

Windows security starts with proper user management, least privilege, and monitoring system activity. Many attacks succeed not because of advanced exploits, but because of basic misconfigurations.

 Tools & Platforms

TryHackMe

Windows OS concepts

Virtual lab environments

 Next Steps

Continue expanding Windows security knowledge

Apply concepts to Active Directory environments

Practice identifying misconfigurations and security risks
