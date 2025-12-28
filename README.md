# 🌐 Web Server Hardening & Logging for Security Monitoring

## 🔐 Objective
Secure a Linux-based Apache (or Nginx) web server using hardening techniques and implement logging/monitoring to detect suspicious activity.

## 🛠️ Security Controls Implemented
- Disabled unused services and default modules
- Configured firewall rules (UFW/firewalld) to restrict access
- Enforced TLS/HTTPS and disabled insecure protocols
- Applied file and directory permission hardening
- Implemented logging with syslog and auditd
- Monitored logs for intrusion indicators (failed login attempts, suspicious traffic)


## 📦 What You'll Learn
* Install Apache2 using the APT package manager
* Start and enable the Apache service
* Verify the Apache default page at `http://localhost`
* Manage Apache using (`systemctl`)commands 
* Check network configuration with `ip a`

## 🚀 Quick Start
1. Make the script executable
```bash
chmod +x scripts/install_apache.sh
```
<img width="753" height="555" alt="Apache Installation Output" src="https://github.com/user-attachments/assets/c3fe48ff-d709-4aa0-8bb0-36d3d90fdfd3" />

2. Run the installation script
```bash
sudo bash scripts/install_apache.sh
```
<img width="752" height="372" alt="Apache Service Status" src="https://github.com/user-attachments/assets/a1b4a169-570e-4079-9213-5fa3f8dab9c5" />

3. Verify Apache is running
Open your web browser and navigate to:
 - http://localhost
 - Or use your system's IP address (find it with ip a)
 <img width="1122" height="703" alt="Apache Browser Default Page" src="https://github.com/user-attachments/assets/123fd0d9-24a9-42ad-8485-a6a346355c58" />

4. View your IP address
`ip a`
<img width="753" height="351" alt="Kali Network IP Configuration" src="https://github.com/user-attachments/assets/1d3bb55b-4dc3-464e-8ba0-564847776889" />

## ✅ Expected Result
You should see the Apache2 Default Page confirming successful installation.
🛠️ Useful Commands
 - Check Apache status
```bash
sudo systemctl status apache2
```

- Stop Apache
```bash
sudo systemctl stop apache2
```

-  Restart Apache
 ```bash
sudo systemctl restart apache2
```

## 🧰 Tools & Technologies
- Linux (Ubuntu/CentOS)
- Apache/Nginx
- UFW / firewalld
- Auditd / Syslog
- SSH Hardening (Fail2Ban optional)

## 🚨 SOC/Blue Team Relevance
This project demonstrates:
- Server security configuration
- Log-based threat detection
- Attack surface reduction
- Incident monitoring foundations
