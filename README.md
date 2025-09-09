# NMAP-WARRIOR-TOOL
Here’s a **properly formatted GitHub README.md** version for your **Nmap Warrior Python Script**. This format follows professional open-source project conventions with clean sections, code blocks, and tables for better readability.

---

# 🔎 Nmap Warrior – Automated Host Discovery & Scanning

## 📖 Description

**Nmap Warrior** is a Python script that automates the process of identifying live hosts from a specified list or a single target.

When additional options are provided, the script extends its functionality to include:

* ✅ Open port scanning
* ✅ Service version detection
* ✅ Scanning of the most commonly used UDP ports

Designed for **cross-platform compatibility**, it works on both **Linux** and **Windows** systems.
This script significantly reduces manual effort, making it an **invaluable tool for security professionals** to efficiently collect information about hosts in their scope.

---

## ⚡ What makes this script effective?

It uses **four methods** to detect live hosts:

1. **Ping scan**
2. **TCP SYN ping scan**
3. **TCP ACK ping scan**
4. **UDP ping scan**

It also provides results in multiple formats:

* 📂 `xml`
* 📂 `nmap`
* 📂 `gnmap`
* 📂 Other grabbable formats

### 🔧 Additional Scanning Features:

* 🔍 Open port scanning
* 🔍 Service version detection
* 🔍 Scanning of commonly used UDP ports

---

## 📦 Installation

### 1. Clone the Repository

```bash

```

### 2. Install Dependencies

Install the required Python packages:

```bash
pip3 install colorama
```

For **Windows only**:

```bash
pip3 install pywin32
```

### 3. Prerequisites

* Python 3
* Nmap
* Notify (optional)

---

## 🚀 Usage

```bash
python3 nmap-warrior.py [-t|--target TARGET] [-l|--list LIST] [Options]
```

### ⚙️ Options

| Flag                | Description                                                      |
| ------------------- | ---------------------------------------------------------------- |
| `-t, --target`      | Specify a target domain or IP address.                           |
| `-l, --list`        | Provide a file containing a list of target hosts (one per line). |
| `-o, --output`      | Define an output folder (default: `nmap_outputs`).               |
| `-s, --silent`      | Disable banner display.                                          |
| `-p, --portscan`    | Perform an open port scan.                                       |
| `-v, --versionscan` | Perform service version detection (requires root privileges).    |
| `-u, --udpscan`     | Perform UDP port scans with version detection.                   |

---

## 📌 Examples

### 🔹 Scan a single target

```bash
python3 nmap-warrior.py -t 192.168.1.1
```

### 🔹 Scan multiple targets from a file & save results in a specific directory

```bash
python3 nmap-warrior.py -l targets.txt -o /path/directory
```

### 🔹 Perform a port scan on live hosts

```bash
python3 nmap-warrior.py -t 192.168.1.1 -p
```

### 🔹 Perform version detection

```bash
python3 nmap-warrior.py -t 192.168.1.1 -p -v
```

### 🔹 Perform a UDP scan

```bash
python3 nmap-warrior.py -t 192.168.1.1 -u
```

---

## ✅ Features Recap

* Multi-method **host discovery**
* **Open port scanning**
* **Service & version detection**
* **UDP scanning**
* Multiple **output formats**

---


