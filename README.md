# Offensive_Security_Lab

My goal is to create an OffSec home lab and to document everything I build/destroy during this setup so that others (and future me) can learn from this experience.
The lab will cover almost any real life scenario, so at the end of this experiment I can be ready for CEH, OSCP, eCPTX and PNPT. (REALLY COOL CERTS AND BIG NAMES)
In this small lab, I will dive in a lot of topics, from the basic setup all the way to AV evasion, in fact, here are all the stuff I will be doing:
Setup a Pentesting Demo Lab
Working with Windows & Linux
OSINT Techniques
Social Engineering
Scripting
Hacking tools
Gaining a Foothold
Windows & Linux Enumeration
Web Attacks
Hacking Active Directory
Privilege Escalation
Persistence Techniques
Lateral Movement
Cloud Exploitation
Reverse Engineering
Anti-Virus Evasion

The lab consists of the following:
  - Attack machines: - Kali linux
                     - CommandoVM
  
  - Target machines: - Metasploitable VM
                     - bWAPP VM
                     - Windows 2019 DC server
                     - Windows IIS + SQL Server
                     - 2x Windows VM domain joined DC01
  
  - Networking:      - PfSense VM for virtualization networking
                     - Mikrotik for physical networking

Note: - All target VMs + PfSense are installed on hypervisor, I will use proxmox just because I never used it before and want to be familiar with their system
      - The mikrotik RB is useless here, I can simply connect the hypervisor and my attack machine on the same switch and move on, but since I already have experience with Mikrotik I will use for fun and for monitoring (I know I can monitor packets on pfsense, but ), it could come in handy later.
      
Here is a documentation I made in Visio to demonstrate the infrastructure:
![OffSecLabDoc](https://github.com/user-attachments/assets/ba850ccc-f008-45ce-a56c-21ae1931c86f)

