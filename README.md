# Offensive_Security_Lab
Keeping track of my offensive security lab progress

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
