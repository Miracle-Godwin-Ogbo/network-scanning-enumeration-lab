# Network Scanning & Enumeration Lab

## Objective
To perform network scanning and service enumeration on a target system in a controlled lab environment using Nmap.

## Tools Used
- Nmap
- Kali Linux
- Metasploitable

## Target
- IP Address: 192.168.222.131

## Scanning Techniques

### 1. Basic Scan
Command:
nmap 192.168.222.131

Purpose:
To identify open ports on the target system.

### 2. Service Version Detection
Command:
nmap -sV 192.168.222.131

Purpose:
To detect running services and their versions.

### 3. Aggressive Scan
Command:
nmap -A 192.168.222.131

Purpose:
To perform OS detection, version detection, script scanning, and traceroute.

### 4. Full Port Scan
Command:
nmap -p- 192.168.222.131

Purpose:
To scan all 65535 ports for hidden services.

### 5. Specific port scan
command:
nmap -p443 192.168.222.131

purpose:
To scan if port 443 is open

### 6. Range port scan
command:
nmap -p1-100 192.168.222.131

purpose:
To scan from port 1 to port 100

## Findings
- Identified multiple open ports including FTP, SSH, and HTTP
- Detected outdated services which may be vulnerable
- Observed potential entry points for further exploitation

  ## Screenshots

### Basic Scan
![Basic Scan](screenshots_basic-scan.png)

### Service Detection
![Service Detection](screenshots_service-Version.png)

### Aggressive Scan
![Aggressive Scan](Screenshot_Aggressive scan.png)

### All port scan
![All Port](screenshots_All-port.png)

### Range Scan
![Range Scan](Screenshots_Range-Scan.png)

### Specific Port Scan
![Specific Port](Screenshots_Specific-Port.png)

## Mitigation
- Close unused ports
- Update outdated services
- Implement firewall rules to restrict access
