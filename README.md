# Homelab Central

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

Disclaimer: *Portions of the scripts were developed with the assistance of Amazon Q and OpenAI's ChatGPT. All content has been manually reviewed and modified as necessary.*
