# Home Lab Infrastructure

## 🎯 Project Overview
Built a virtualized home lab environment using Proxmox VE to develop hands-on skills in cloud computing, cybersecurity, and systems engineering. Im doing this as a learning platform for enterprise technologies and prepares me for roles in cloud security and ML systems engineering.

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
