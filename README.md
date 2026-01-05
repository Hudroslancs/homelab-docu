# Home Lab Infrastructure

## 🎯 Project Overview
Built a virtualized home lab environment using Proxmox VE to develop hands-on skills in cloud computing, cybersecurity, and systems engineering. This infrastructure serves as a learning platform for enterprise technologies and prepares me for roles in cloud security and ML systems engineering.

## 🏗️ Architecture

### Hardware Specifications
- **Server Node:**
  - CPU: Intel i5 (6 cores)
  - GPU: NVIDIA RTX 3060 Ti (12GB VRAM) - for future CUDA/ML workloads
  - RAM: 32GB DDR4
  - Storage: 
    - 240GB SATA SSD (Hypervisor boot drive)
    - 1TB HDD (VM storage and data)
  - Network: Gigabit Ethernet

### Software Stack
- **Hypervisor:** Proxmox VE 8.x (Type-1 bare-metal hypervisor)
- **Virtualization:** KVM/QEMU
- **Storage:** LVM-Thin provisioning for efficient disk usage
- **Network:** Bridged networking for VM internet access

## 📋 Implemented Services

### 1. NextCloud Private Cloud Server
**Purpose:** Replace Google Drive with self-hosted solution, reduce cloud storage costs

**Technical Details:**
- **VM Specs:** Ubuntu 24.04 LTS Server (4GB RAM, 2 vCPUs, 100GB disk)
- **Web Stack:** Apache2, MariaDB, PHP 8.x
- **Features Implemented:**
  - File synchronization across devices
  - Web-based file management interface
  - User authentication and access control
  - Database-backed storage management

**Skills Demonstrated:**
- Linux server administration
- LAMP stack deployment and configuration
- Database setup and management (MariaDB)
- Web server configuration (Apache)
- Network services deployment

**Configuration Process:**
```bash
# Key installation steps performed
sudo apt install apache2 mariadb-server php php-mysql libapache2-mod-php
sudo mysql_secure_installation
# Created dedicated database and user with proper permissions
# Configured Apache virtual host for NextCloud
# Set appropriate file permissions for web server
```

## 🛠️ Technical Skills Developed

### Infrastructure & Virtualization
- Bare-metal hypervisor installation and configuration
- Virtual machine provisioning and lifecycle management
- Storage pool configuration (LVM-Thin)
- Network bridge configuration for VM connectivity
- Resource allocation and optimization

### Linux System Administration
- Ubuntu Server installation and hardening
- Package management (apt)
- User and permission management
- SSH configuration for secure remote access
- Service management with systemd

### Networking
- Static IP configuration
- Network troubleshooting (ping, ip, route commands)
- Port forwarding concepts
- DNS configuration
- Firewall basics (planned)

### Database Management
- MariaDB/MySQL installation
- Database and user creation
- Permission management with GRANT statements
- Basic SQL operations

### Web Technologies
- Apache web server installation and configuration
- Virtual host setup
- PHP configuration for web applications
- SSL/TLS concepts (to be implemented)

## 🔄 Current Status & Next Steps

### ✅ Completed
- [x] Proxmox installation and initial configuration
- [x] Storage pool setup with LVM-Thin
- [x] Ubuntu Server VM deployment
- [x] NextCloud installation and configuration
- [x] File synchronization testing
- [x] Network connectivity verification

### 🚀 Planned Implementations

#### Phase 2: Security & Monitoring
- [ ] Deploy Kali Linux VM for penetration testing practice
- [ ] Set up VPN server (WireGuard/OpenVPN)
- [ ] Implement network segmentation with VLANs
- [ ] Deploy SIEM solution (Wazuh or ELK stack)
- [ ] Configure fail2ban for intrusion prevention

#### Phase 3: Machine Learning & GPU Computing
- [ ] Install NVIDIA CUDA toolkit and drivers
- [ ] Deploy Ubuntu VM with CUDA for ML workloads
- [ ] Set up Jupyter Notebook for ML experiments
- [ ] Test PyTorch/TensorFlow on RTX 3060 Ti
- [ ] Practice ML model training and inference

#### Phase 4: Container Orchestration
- [ ] Deploy Kubernetes cluster (K3s or microk8s)
- [ ] Learn container networking and storage
- [ ] Deploy containerized applications
- [ ] Practice rolling updates and scaling

#### Phase 5: Infrastructure as Code
- [ ] Learn Terraform for VM provisioning
- [ ] Implement Ansible for configuration management
- [ ] Version control infrastructure code
- [ ] Practice GitOps workflows

## 📊 Learning Outcomes

### Practical Experience Gained
1. **Infrastructure Design:** Planned and implemented multi-tier architecture with separation of concerns (boot, compute, storage)
2. **Problem Solving:** Troublehooted hardware compatibility, network connectivity, and storage issues
3. **Documentation:** Maintained detailed notes of configurations and troubleshooting steps
4. **Best Practices:** Implemented security basics (SSH keys, non-root users, firewalls)

### Relevance to Career Goals
This home lab directly supports my transition into:
- **Cloud Security:** Understanding virtualization, network security, and access control
- **Systems Engineering:** Hands-on experience with Linux, automation, and infrastructure management
- **ML Engineering:** GPU passthrough preparation for CUDA programming and model training

**Long-term Goal:** Systems Engineer or ML Infrastructure role at NVIDIA

## 🔗 Certifications
- AWS Certified Cloud Practitioner
- EC-Council Certified Ethical Hacker (CEH)

## 📸 Screenshots
*Coming soon: Dashboard views, network topology diagram, service interfaces*

## 🤝 Acknowledgments
Built as part of continuous learning in cloud computing, cybersecurity, and systems engineering.

---

**Last Updated:** January 2025
```

---

### **Step 3 - Save and Commit**

1. Scroll down
2. **Commit message:** `Initial homelab documentation`
3. Click **"Commit changes"**

---

### **Step 4 - Add More Files (Optional but Impressive)**

Create new files in repo:

**`network-diagram.md`** - Draw out your network topology
**`troubleshooting-log.md`** - Document issues you solved (like the NVMe, ethernet port, etc.)
**`nextcloud-setup.md`** - Detailed NextCloud installation steps

---

## **PART 2: RESUME**

### **Where to Add:**

**Under "Projects" or "Technical Experience" section:**
```
HOME LAB INFRASTRUCTURE | Proxmox Virtual Environment
January 2025 - Present

- Designed and deployed enterprise-grade home lab using Proxmox VE bare-metal hypervisor on dedicated hardware (Intel i5, 32GB RAM, NVIDIA RTX 3060 Ti)

- Implemented NextCloud private cloud server on Ubuntu 24.04 LTS VM, replacing commercial cloud storage and demonstrating full-stack deployment (LAMP stack: Apache, MariaDB, PHP)

- Configured LVM-Thin storage pools and network infrastructure with static IP addressing for production-like environment

- Established foundation for hands-on learning in cybersecurity penetration testing, CUDA/ML development, and container orchestration

Technologies: Proxmox VE, Linux (Ubuntu), KVM/QEMU, Apache, MariaDB, PHP, LVM, Networking (TCP/IP, SSH)
```

**That's 4 bullet points - perfect length!**

---

### **Alternative Shorter Version (if space limited):**
```
HOME LAB SERVER | Proxmox Virtualization Environment
Jan 2025

- Built virtualized home lab with Proxmox VE for hands-on practice in cloud infrastructure, cybersecurity, and ML/CUDA development (i5, RTX 3060 Ti, 32GB RAM)

- Deployed self-hosted NextCloud private cloud on Ubuntu VM with full LAMP stack configuration

Technologies: Proxmox, Linux, KVM, Apache, MariaDB, Virtualization, Networking
```

---

## **PART 3: LinkedIn POST (Bonus!)**

Post this on LinkedIn for visibility:
```
🚀 Just completed my first major home lab project!

Built a virtualized infrastructure using Proxmox VE to develop hands-on skills for my transition into cloud security and systems engineering.

What I implemented:
✅ Proxmox bare-metal hypervisor
✅ Ubuntu Server VMs with proper resource allocation
✅ Self-hosted NextCloud (LAMP stack) as Google Drive replacement
✅ Network configuration with static IPs and SSH access

This lab will serve as my learning platform for:
🔐 Cybersecurity & penetration testing
☁️ Cloud infrastructure concepts
🤖 ML/CUDA development on RTX 3060 Ti
🐳 Container orchestration (Kubernetes)

Coming from a mechanical engineering background, every step of this build taught me something new about Linux, networking, and virtualization.

Next up: Deploying security tools and setting up CUDA for ML workloads!

GitHub: [link to your repo]

#Homelab #CloudComputing #Cybersecurity #CareerTransition #ITInfrastructure #Linux #Proxmox

---
Anyone else running home labs? Would love to connect and exchange ideas! 💡
