# RL-Swarm Installer & Updater
This script automates the installation and updates for the RL-Swarm. Including system resource management and service configuration

## 📋 Prerequisites

- **OS Ubuntu**
- **8 Core**
- **16GB RAM**
- **100GB Disk**
- Stable internet connection

## 🚀 Features
Resource Management: Creates a dedicated systemd slice (rl-swarm.slice) to limit the service's CPU and RAM usage, ensuring it doesn't consume all system resources.

CPU: Limits CPU usage to N-1 cores, where N is the total number of cores on the system.

RAM: Reduces total RAM usage by 3GB to leave a buffer for the operating system and other processes.

### 1. One Command Instlation
```bash
bash <(curl -s https://raw.githubusercontent.com/brillianxbt/gensyn/main/systemd.sh)
```

### 2. Login

- Access the login page
- Enter your password
- Complete the login

### Check Logs
```bash
journalctl -u rl-swarm -f -o cat
```
