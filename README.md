# AWS EC2 OpenVPN Server

A secure, self-hosted OpenVPN server deployed on an AWS EC2 instance. This project demonstrates cloud networking, security group configuration, and VPN administration.

## 🚀 Features
- Hosted on AWS EC2 (Ubuntu 24.04 LTS)
- Secured via AWS Security Groups (Custom UDP/TCP ports)
- OpenVPN protocol with strong encryption (AES-256-GCM)
- Automated client configuration generation

## 🛠️ Architecture
- **Provider:** AWS
- **Instance Type:** t3.micro
- **Firewall:** Security groups restricting traffic except for the OpenVPN port and SSH.

## 📋 Setup & Installation Instructions
1. **Launch EC2 Instance:**
2. **Configure Security Groups:**
   - Inbound: Allow UDP on port 1194 (default OpenVPN port).
   - Inbound: Allow SSH on port 22 (restricted to your IP).
3. **Install OpenVPN:**
4. sudo ./openvpn-install.sh install
   ./openvpn-install.sh interactive
