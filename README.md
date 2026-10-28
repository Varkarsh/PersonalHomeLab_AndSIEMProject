# PersonalHomeLab_AndSIEMProject
Tracking personal homelab and potential SIEM environment. For professional development

This is a personal project I have been wanting to do for a while, since getting my Cybersecurity Degree back in 2020. However, a lot of my time is normally taken up by work, and also continuing education. I want to make this git repository to better track and document my progress. Show where I ran into issues, log and ticket certain troubles from the other users in my household, and ensure proper retention of the skills I have learned from my IT career.

Experience:
I have worked for two years as a Help Desk Technician Tier II at a local credit union, so I have some basic understanding of AD, MDM, IAM, and networking troubleshooting. Printer Tech for Ricoh, so I understand basic printer configuration for enterprise networks especially in a healthcare environment. IT tech for a EMS billing, which was my first job in IT. Unfortunately, very little experience gained, as my entire job was building NUCs for people to work from home during COVID.

Education:
Associates in Cybersecurity at Olympic College, Comptia Security + Expected no later than Feb 2027.

Goals:
1. Personal NAS - storing a lot of my larger sized files on the network such as 3d print files, books, ISOs for Virtual Environments, and also store other files for the household (three users total in the household, perform basic file permissions, and map network drive to each user correctly) - Hardware: Either a old desktop I gathered from E-Waste, or a NAS enclosure I got off Newegg years ago, with minimum 4TB of storage. If using NAS enclosure since it is only two bays, use RAID 1, but if I use a old desktop where I can add more than 2 drives, use RAID 6 (If using old computer, install TrueNAS)
2. Networking - Re-do the entire home network with the homelab. Utilize a Star Topology with a central 24 port switch separated into 4 VLANs (Asymmetrical VLAN configuration based on the needs of the users at home. 8 ports for the homelab, rest will be updated and determined once I discuss with the household, as I will likely place unmanaged switches into each persons configuration, preventing latency as much as I can while still giving them access to many switchports), firewall configuration to understand firewall concepts and protection at the barest form.
3. VPN - More for personal use, but good to understand basic VPN concepts at a Command Line level if I use Wireguard on Linux, idea is to place all my music in the lab, using OpenMediaVault to allow myself to stream my own music with ease without using Samsung or Spotify Music Apps.
4. SIEM (THIS ONE FOR WORK) - Creating a virtual SIEM lab, to log and record traffic, attacks, and mitigation techniques, for the better understanding of how blue team operates at an enterprise level for the sole purpose of getting hired into the field.
Hardware for Goals 2 to 4 - Currently, a Lenovo ThinkCentre M720q with an i7 - 8400T, 16GB of RAM, and 1TB of main OS storage (Utilizing ProxMox for containers for the apps and lab)
More will be added as I continue down this path


Below will be timestamps of what I have done currently in regards to my homelab.

10-26-2026: Lenovo ThinkCentre M720q has been delivered from EBay, bought another 8GB of DDR4 SODIMM RAM at 2666MHz (As the current system has no AC, only 8GB of RAM, and no SSD, currently save up to buy SSD with ridiculous SSD prices in today's market). Created this Github Repository.

10-27-2026: Created a step by step plan to implement this:
<img width="740" height="558" alt="image" src="https://github.com/user-attachments/assets/9d6b6ba8-c4da-4007-b8be-71d341eb0962" />

Lenovo specs plan:
32GB of RAM, 1TB SSD (FIND ONE FOR CHEAP)

Using Wazuh integrated in Ubuntu, Sysmon in Win11, Kali for attacking.

Resource Allocation:
1. The SIEM / SOC	Ubuntu Server 22.04	Wazuh (All-in-one SIEM/XDR)	2 vCPUs, 8 GB to 12 GB RAM, 50 GB Storage
2. The Target Endpoint	Windows 10 / 11 Pro	Sysmon (advanced Windows logging) + Wazuh Agent	2 vCPUs, 6 GB to 8 GB RAM, 40 GB Storage
3. The Attacker	Kali Linux	Nmap, Hydra, Metasploit (to generate attack traffic)	1 vCPU, 2 GB to 4 GB RAM, 30 GB Storage


I plan to try to use Wazuh All-In-One Approach with ELK Stack
The concept and utilization justification: - SIEM & Endpoint Detection Automation Project (Homelab)

1. Engineered an enterprise-grade SIEM cluster utilizing an all-in-one Wazuh ecosystem built on a bare-metal Proxmox hypervisor layer.
2. Optimized data pipelines via OpenSearch logging nodes, configuring ingestion parameters for system event logs, process creation tracking, and network sockets.
3. Designed custom detection matrices mapping threat vectors directly to the MITRE ATT&CK framework, facilitating clear auditing of mock brute-force and privilege escalation attacks.
4. Analyzed raw security telemetry to isolate indicator-of-compromise (IoC) data points, significantly shortening simulated triage and response windows.


