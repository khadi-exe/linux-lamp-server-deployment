# linux-lamp-server-deployment
📌 Project Overview

This project demonstrates the deployment, configuration, and hardening of a Linux-based LAMP stack (Apache, MySQL, PHP) in a virtualized environment. The server was configured with custom DNS resolution, HTTPS using a self-signed SSL certificate, least-privilege service accounts, and secured database access. Functionality was validated from a separate Kali Linux client.

This project was completed as part of a systems and network administration course and reflects real-world Linux server administration and security practices.

🛠 Technologies Used

Operating Systems: Ubuntu/Xubuntu (Server), Kali Linux (Client)
Web Server: Apache2
Database: MySQL
Backend: PHP
Management Tool: phpMyAdmin
Security: SSL/TLS (Self-Signed Certificate)
Networking: Local DNS, Port Verification
Environment: Virtual Machines

🧱 System Architecture

Server VM: Hosts Apache, MySQL, PHP, and phpMyAdmin

Client VM (Kali Linux): Used to remotely access the web application and phpMyAdmin

Local DNS: Custom domain mapped via /etc/hosts

HTTPS: Enabled using a self-signed SSL certificate

⚙️ Key Features & Configuration
Apache
Installed and configured Apache2
Replaced default www-data user/group with a custom least-privilege service account
Created a custom document root
Configured virtual hosts with a personalized DNS name
Enabled HTTPS using a self-signed SSL certificate
Modified core Apache configuration files:
apache2.conf
ports.conf
envvars
sites-available/
sites-enabled/
