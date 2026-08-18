# Nmap-Network-Scanning-Enumeration-Lab

## 📌 Project Overview

This project demonstrates the use of Nmap (Network Mapper) for network discovery, port scanning, service enumeration, and basic OS detection in an authorized cybersecurity lab environment.

## 🎯 Objectives
-Discover active hosts on a network
-Identify open ports
-Detect running services and their versions
-Perform basic OS detection
-Use Nmap NSE scripts for enumeration
-Save and analyze scan results

## 🧪 Lab Environment

-OS: Kali Linux
-Target: Metasploitable 2
-Tool: Nmap
-Virtualization: VMware / VirtualBox
-Network: Isolated lab network

## 🛠️ Nmap Commands Used

### 1. Check target connectivity

Command:
ping -c 4 <target_ip>

<img width="575" height="298" alt="Screenshot 2026-08-18 133503" 

Target Connectivity: Verified that the target machine is reachable from Kali Linux before starting the Nmap scan.

### 2. Host Discovery

Command:
nmap -sn <target_ip>

<img width="566" height="127" alt="Screenshot 2026-08-18 134131" src="https://github.com/user-attachments/assets/c672b20f-d401-4384-920a-7b50888f9bd1" />

Host Discovery: Nmap was used to determine whether the target host was active on the network.

### 3. Basic Port Scan

Command:
nmap <target_ip>

<img width="574" height="549" alt="Screenshot 2026-08-18 134648" src="https://github.com/user-attachments/assets/a62aa275-0834-43dc-850f-deaad9e46f60" />

Port Scanning: A basic Nmap scan was performed to identify commonly used open TCP ports on the target.

### 4. Service & Version Detection

Command:
nmap -sV <target_ip>

<img width="993" height="520" alt="Screenshot 2026-08-18 135354" src="https://github.com/user-attachments/assets/3fd29fa7-7c89-4ca2-bb21-515a2262f5a0" />

Service Enumeration: Nmap service detection was used to identify the services running on open ports and their detected versions.

### 5. OS Detection

Command:
sudo nmap -O <target_ip>

<img width="549" height="584" alt="Screenshot 2026-08-18 140230" src="https://github.com/user-attachments/assets/44642d1a-5b11-48e0-8ae0-8e12728e179b" />

OS Detection: Nmap was used to perform operating system fingerprinting and identify the probable operating system of the target.

### 6️. Default NSE Script Scan

Command:
nmap -sC <target_ip>

<img width="1156" height="524" alt="image" src="https://github.com/user-attachments/assets/98355fac-982e-4420-8341-94f9a9430592" />


NSE Enumeration: Default Nmap Scripting Engine (NSE) scripts were executed to gather additional information about the target services.




                          src="https://github.com/user-attachments/assets/9f26425d-b7ad-4e2c-8142-1b6486bb478f" />
