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
