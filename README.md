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
<img width="654" height="567" alt="image" src="https://github.com/user-attachments/assets/64ef959e-3b23-4475-994c-41e126d0adac" />
<img width="789" height="312" alt="image" src="https://github.com/user-attachments/assets/6d573278-e05a-4059-bcfe-3ad7262d87b1" />



NSE Enumeration: Default Nmap Scripting Engine (NSE) scripts were executed to gather additional information about the target services.

### 7. UDP Scan

Command:
sudo nmap -sU <target_ip>

<img width="749" height="448" alt="image" src="https://github.com/user-attachments/assets/09378bf0-1a62-40b0-b819-5c3c8018b316" />

UDP Scan: Nmap scanned the target for open or filtered UDP ports and identified available UDP services.

### 8. FIN Scan

Command:
sudo nmap -sF <target_ip>

<img width="558" height="508" alt="image" src="https://github.com/user-attachments/assets/e9e87375-904a-4524-895a-182f26b987ca" />
<img width="486" height="73" alt="image" src="https://github.com/user-attachments/assets/6a8f0d13-cfef-4066-a837-8950923a64dc" />

FIN Scan: A TCP FIN scan was performed to analyze the target's response to FIN packets and identify possible open or filtered ports.

### 9. Xmas Scan

Command:
sudo nmap -sX <target_ip>

<img width="533" height="515" alt="image" src="https://github.com/user-attachments/assets/800cd659-33f6-4b6a-b489-975eb5c8f3cc" />

Xmas Scan: A TCP Xmas scan was performed using FIN, PSH, and URG flags to analyze the target's response to specially crafted TCP packets.

### 10. Comprehensive Scan

Command:
sudo nmap -sC -sV -O <target_ip>

<img width="1270" height="496" alt="image" src="https://github.com/user-attachments/assets/78b539cd-d184-4a05-ae00-705193b3e14c" />
<img width="1057" height="514" alt="image" src="https://github.com/user-attachments/assets/a41c72cf-13d4-4b98-bb00-bc034f91b9c1" />
<img width="898" height="308" alt="image" src="https://github.com/user-attachments/assets/84d67c08-af58-4d49-b7f6-736053b9637d" />

Comprehensive Scan: This scan combines service detection, version detection, operating system detection, and NSE scripts to perform detailed enumeration of the target.

### 11.Save Scan Results

Command:
nmap -sC -sV -O <target_ip> -oN scan-results.txt

<img width="878" height="190" alt="image" src="https://github.com/user-attachments/assets/49aa8bd0-be9c-4850-9196-c383355dacaa" />

Report Generation: The scan results were saved to a text file for documentation and future analysis.

## 📌 Learning Outcomes

After completing this project, I learned how to:

-Verify target connectivity
-Discover active hosts
-Perform TCP and UDP port scanning
-Detect services and versions
-Identify the target operating system
-Use Nmap NSE scripts for enumeration
-Perform FIN and Xmas stealth scans
-Save scan results for reporting
-Document a network scanning assessment in a professional GitHub project










                          src="https://github.com/user-attachments/assets/9f26425d-b7ad-4e2c-8142-1b6486bb478f" />
