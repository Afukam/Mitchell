# Mitchell

**Mitchell** is an automated Bash-based security and system auditing toolkit designed for learning, experimentation, and workflow automation on Linux systems.

---

## 📋 Table of Contents
- [⚠️ Security Disclaimer](#️-security-disclaimer)
- [📥 Installation](#-installation)
- [🖱️ Usage](#️-usage)
- [🚀 Features](#-features)
- [🧠 How It Works](#-how-it-works)
- [🛠️ Prerequisites](#️-prerequisites)
- [📂 Project Structure](#-project-structure)

---
## ⚠️ Security Disclaimer

- **This project was created for educational purposes and shell scripting practice.

- **Legal Notice:
Unauthorized scanning of networks or systems may be illegal in many jurisdictions.
---
## 📥 Installation
-Clone or download this repository.
-Navigate to the project directory.
-Make the script executable:
`chmod +x mitchell_tool.sh

---
## 🖱️ Usage
- **Run the tool with root privileges (required for network and hardware operations):
``sudo ./mitchell_tool.sh

- **Ordering Tasks

When prompted, enter tasks as a space-separated list.
- **Example Input:
``2 1 3

- **Execution Order

- Change MAC address

- Simulate IP change

- Launch network scan
---
## 🚀 Features

- **IP Rotation Module**  
  Fetches real-world IPv4 subnets from the RIPE database based on a randomly selected country to simulate network presence across regions.

- **MAC Spoofing**  
  Interfaces directly with the Linux networking stack to randomize the system’s MAC address using `macchanger`.

- **Nmap Auditing Suite**  
  Automated TCP, UDP, and vulnerability scans (NSE), with real-time logging.

- **Process Snapshot**  
  Generates hierarchical “forest” views of running system processes and identifies top memory consumers.

- **Anti-RockYou Password Generator**  
  Uses `/dev/urandom` to generate high-entropy passwords resistant to dictionary-based attacks.

---

## 🧠 How It Works

Mitchell uses **Sequential Execution Logic**.

When a user provides an ordered list of tasks (e.g. `2 1 5`), the script processes each module sequentially using a loop. This ensures each security or system operation completes before the next begins.

---


## 🛠️ Prerequisites

The following utilities must be installed on a Linux system:

- Bash
- `jq`
- `macchanger`
- `nmap`
- `curl`

---

### Install Dependencies

```bash
sudo apt update
sudo apt install jq macchanger nmap curl -y



---

