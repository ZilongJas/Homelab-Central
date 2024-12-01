# Homelab Central

A modular command-line tool for managing your home lab. Fetch weather data, monitor web server status, and more. (Coming soon)

*TODO:* 

0. Make an install/uninstall script as another option

1. Centralized System Info

    homelab status: Show an overview of system health (CPU, memory, disk usage, temperatures, and active services).
    homelab check: Run a health check for your homelab services (e.g., checking Docker containers, web servers, and databases).

2. Service Management

    homelab services: List, start, stop, or restart services like web servers, databases, etc.
    homelab deploy: Simplified deployment of a web server, database, or app.

3. Backup and Restore

    homelab backup: Run backups for specific directories, services, or databases.
    homelab restore: Restore from the most recent backup.

4. Network Tools

    homelab network: Run network diagnostics (ping, traceroute, check bandwidth usage).
    homelab ports: Show open ports and active connections.

5. Custom Scripts and Automation

    homelab schedule: Create cron jobs easily for automated tasks.
    homelab scripts: Run or manage custom scripts through the tool.

6. Monitoring and Alerts

    homelab monitor: Set up resource usage thresholds and receive alerts.
    homelab logs: Tail and filter system or application logs from a centralized location.

7. Docker/Kubernetes Integration

    homelab containers: Manage Docker containers (start, stop, status).
    homelab k8s: Interact with a Kubernetes cluster (view pods, apply configs).

8. Environment Provisioning

    homelab provision: Automate creating VMs, installing software, or setting up services.

![image](https://github.com/user-attachments/assets/38722e89-23b0-4eb8-83bb-c83ab92c6ff5)

---

## Setup Instructions

Follow these steps to set up `Homelab` on your system:

### 1. Clone the Repository
Clone this repository into your home directory:
```bash
git clone https://github.com/ZilongJas/Homelab-Central.git
```
### 2. Make it executable
```bash
sudo chmod +x ~/Homelab-Central/Homelab/homelab && sudo chmod +x ~/Homelab-Central/Homelab/modules/*
```
### 3. Add `Homelab` to Your PATH
Update your `PATH` environment variable to include the `Homelab` directory by running:
```bash
echo 'export PATH="$PATH:$HOME/Homelab-Central/Homelab"' >> ~/.bashrc
```

### 4. Reload Your Shell Configuration
Apply the changes to your current shell session:
```bash
source ~/.bashrc
```

### 5. Verify the Installation
Check if `homelab` is now accessible:
```bash
which homelab
```

The output should return the path to the `homelab` script:
```
/home/your-username/Homelab-Central/Homelab/homelab
```
---

## Uninstallation

To remove `Homelab` from your system:

1. Delete the repository:
   ```bash
   rm -rf ~/Homelab-Central
   ```
2. Remove the `PATH` entry from `~/.bashrc`. Open the file in a text editor:
   ```bash
   nano ~/.bashrc
   ```
   Find and delete this line:
   ```bash
   export PATH="$PATH:$HOME/Homelab-Central/Homelab"
   ```
3. Reload your shell configuration:
   ```bash
   source ~/.bashrc
   ```
