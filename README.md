# GWN Manager - Enterprise Network Management

## 📌 Overview
This repository documents the deployment and configuration of **GWN Manager**, a centralized enterprise-grade network management system. The primary goal of this project was to unify the administration, monitoring, and maintenance of all company network devices (Access Points, Switches, etc.) into a single, robust local control panel.

By migrating from standalone device management to a centralized local server, we achieved better visibility, streamlined firmware updates, and laid the foundation for comprehensive network topology mapping.

## 🏗️ Infrastructure & Deployment
To ensure high availability, scalability, and efficient resource utilization, the GWN Manager was deployed on our on-premise **Proxmox VE Cluster**. 

### Installation
The deployment was streamlined utilizing Proxmox community scripts. The GWN Manager LXC (Linux Container) was provisioned directly via the Proxmox shell using the following command:

```bash
bash -c "$(curl -fsSL https://raw.githubusercontent.com/community-scripts/ProxmoxVE/main/ct/gwn-manager.sh)"
```

## 🚀 Project Phases & Milestones

### 1. Server Provisioning & Setup ✅
- Configured the Proxmox cluster environment.
- Deployed the GWN Manager container seamlessly.
- Established network connectivity and assigned a static IP for the management interface.

### 2. Device Adoption & Firmware Upgrades ✅
- Discovered primary network devices, including core Switches and Wireless Access Points.
- Performed critical firmware updates on all edge devices to ensure full compatibility and stability with the new GWN Manager.
- Successfully adopted and integrated all company network devices into the centralized dashboard.

### 3. Network Topology Mapping (In Progress) ⏳
- Currently drawing and mapping the physical and logical layout of the network.
- Visualizing the interconnections between the core switch, edge switches, and APs to facilitate easier troubleshooting and future network scaling.

## 📸 Screenshots
Here are some visual captures from the deployment and configuration process:
![Screenshot 1](https://github.com/islamsayed0/gwn/blob/main/Screenshot%202026-05-18%20at%2011.00.19%E2%80%AFAM.png?raw=true)
![Screenshot 2](https://github.com/islamsayed0/gwn/blob/main/Screenshot%202026-05-18%20at%2011.00.53%E2%80%AFAM.png?raw=true)
![Screenshot 3](https://github.com/islamsayed0/gwn/blob/main/Screenshot%202026-05-18%20at%2011.01.01%E2%80%AFAM.png?raw=true)
![Screenshot 4](https://github.com/islamsayed0/gwn/blob/main/Screenshot%202026-05-18%20at%2011.01.13%E2%80%AFAM.png?raw=true)

## 💡 Key Learnings & Takeaways
Implementing this project provided profound hands-on experience and valuable insights into:
- Virtualization and lightweight container deployment utilizing Proxmox VE.
- Enterprise network device management, adoption processes, and centralized provisioning.
- Firmware life-cycle management for critical IT infrastructure.
- The importance of accurate network topology design and visualization.
