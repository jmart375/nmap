![download](https://github.com/jmart375/nmap/assets/91294710/cb0903ac-7bee-4588-aee5-ba753e6c4ca6)

# Nmap Overview

Nmap, short for "Network Mapper," is an open-source tool for network exploration and security auditing. It is widely used for discovering devices on a network, identifying open ports, and determining the services running on those ports.

## Key Features

1. **Network Discovery:**
   - Discover hosts and services on a computer network.
   - Map the network topology to identify active hosts and open ports.

2. **Port Scanning:**
   - Perform various types of port scans, including TCP connect, SYN, and UDP scans.
   - Identify open ports on target systems.
![image](https://github.com/jmart375/nmap/assets/91294710/f6f72127-cf44-4d2a-8551-b883fedf0a90)

![image](https://github.com/jmart375/nmap/assets/91294710/c69aafd8-1eec-4063-a7fd-a92d6cf1fee1)


3. **Service and Version Detection:**
   - Detect the services and their versions running on open ports.
   - Assess the security posture of a system by understanding the services in use.
•	What version of OpenSSH is running?
Once we ran the appropriate command, which scanned for the TCP services, we discovered  	OpenSSH 4.7p1 Debian 8ubuntu1 (protocol 2.0). The image below shows the results.
•	What version of the FTP server is running?
The FTP was found to be vsftpd 2.3.4. 
![image](https://github.com/jmart375/nmap/assets/91294710/aee1b50a-27a7-4094-aeca-a2d8c5e1eb25)

4. **OS Detection:**
   - Guess the operating system of a target host based on network characteristics.
   - Enhance understanding of the target environment.
•	The following command is used to find the host through Nmap “sudo Nmap -O 192.168.182.131.”
•	What is the information that Nmap discovers, including the “Device type,” the “OS CPE” (common platform enumeration), and the “OS details”? 
Upon running the command, it was shown Device Type: general purpose, OS CPE: /		o:Linux:linux_kernel:2.6 and the OS details are Linux 2.6.9 - 2.6.33. An illustration is provided below.
•	What is the range of possible kernel versions that Nmap thinks is running on the target host?
The range of possible kernel versions was determined to be anywhere from 2.6.9 - 2.6.33.
•	 What version of Linux is the target system running (on the Metasploitable2 VM, run the “uname -a” command)?
•	When we ran the command (uname -a), the Kali Linux 5.18.0-kali5-amd64 #1 SMP PREEMPT_DYNAMIC Debian 5.18.5-1kali6 (2022-07-07) x86_64 GNU/Linux
![image](https://github.com/jmart375/nmap/assets/91294710/f3c3e02b-7a9c-40af-af6a-72f345c3b94c)

5. **Scripting Engine (NSE):**
   - Execute scripts to perform specific tasks during scanning.
   - Use NSE scripts for vulnerability detection, exploitation, and information gathering.

6. **Output Formats:**
   - Generate output in various formats, including plain text, XML, and grepable formats.
   - Customize output for integration into other tools and workflows.

## Getting Started

### Prerequisites
- Install Nmap on your system. [Nmap Installation Guide](https://nmap.org/book/inst-windows.html)

### Usage Examples
- Basic TCP connect scan: `nmap -sT target`
- OS detection: `nmap -O target`
- Service version detection: `nmap -sV target`


