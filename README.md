# Homelab

A modular command-line tool for managing your home lab. Fetch weather data, monitor web server status, and more.

---

## Setup Instructions

Follow these steps to set up `Homelab` on your system:

### 1. Clone the Repository
Clone this repository into your home directory:
```bash
git clone https://github.com/ZilongJas/Homelab-Central.git
```

### 2. Add `Homelab` to Your PATH
Update your `PATH` environment variable to include the `Homelab` directory by running:
```bash
echo 'export PATH="$PATH:$HOME/Homelab-Central/Homelab"' >> ~/.bashrc
```

### 3. Reload Your Shell Configuration
Apply the changes to your current shell session:
```bash
source ~/.bashrc
```

### 4. Verify the Installation
Check if `homelab` is now accessible:
```bash
which homelab
```

The output should return the path to the `homelab` script:
```
/home/your-username/Homelab-Central/Homelab/homelab
```

### 5. Run `Homelab`
Use the `homelab` command to perform various tasks:

- **Fetch Weather Data:**
  ```bash
  homelab -weather "Los Angeles"
  ```
- **Check Web Server and Storage Status:**
  ```bash
  homelab -web info
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
