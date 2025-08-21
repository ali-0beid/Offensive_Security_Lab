# Offensive_Security_Lab

My goal is to create an OffSec home lab and to document everything I build/destroy during this setup so that others (and future me) can learn from this experience.  
The lab will cover almost any real life scenario, so at the end of this experiment I can be ready for CEH, OSCP, eCPTX and PNPT. (REALLY COOL CERTS AND BIG NAMES).  

## Topics
In this small lab, I will dive in a lot of topics, from the basic setup all the way to AV evasion, in fact, here are all the stuff I will be doing:
1. Setup a Pentesting Demo Lab
2. Working with Windows & Linux
3. OSINT Techniques
4. Social Engineering
5. Scripting
6. Hacking Tools
7. Gaining a Foothold
8. Windows & Linux Enumeration
9. Web Attacks
10. Hacking Active Directory
11. Privilege Escalation
12. Persistence Techniques
13. Lateral Movement
14. Cloud Exploitation
15. Reverse Engineering
16. Anti-Virus Evasion

## Lab Infrastructure

The lab consists of the following:
  - **Attack machines**:
    - Kali linux [CPU: i5-1335U | Memory: 8GB | Disk: 512GB NVME]
    - CommandoVM [CPU: Ryzen 7 5800x | Memory: 32GB | Disk: 512GB NVME] ***This is overkill, but I ran out of hardware so had to use my gaming PC***
  
  - **Target machines**:
    - ProxMox OS [CPU: i5-8 | Memory: 16GB | Disk: 512GB SSD] ***All the targets are VMs on this device***
    - Metasploitable VM
    - bWAPP VM
    - Windows 2019 DC server
    - Windows IIS + SQL Server
    - 2x Windows VM domain joined DC01
  
  - **Networking**:
    - PfSense VM for virtualization networking
    - Mikrotik for physical networking

**Note**:
  - All target VMs + PfSense are installed on hypervisor, I will use proxmox just because I never used it before and want to be familiar with their system
  - The mikrotik RB is useless here, I can simply connect the hypervisor and my attack machine on the same switch and move on, but since I already have experience with Mikrotik I will use for fun and for monitoring (I know I can monitor packets on pfsense, but ), it could come in handy later.

      
Here is a documentation I made in Visio to demonstrate the infrastructure:

![OffSecLabDoc](https://github.com/user-attachments/assets/1fc51d2a-e6e6-470e-84d6-c7f5a3cee327)



# Day 1

## Setting up the environment

I finished installing Kali on my attacker machine, and now Im installing ProxMox on the target machine laptop. *I give you a tip, use ventoy USB, you can thank me later*
