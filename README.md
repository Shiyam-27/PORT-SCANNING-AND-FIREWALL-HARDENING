# PORT-SCANNING-AND-FIREWALL-HARDENING
This project automatically scans for open TCP ports on a Windows system using Nmap and blocks them using Windows Defender Firewall. A PowerShell script handles the automation, and a batch file allows one-click execution. It helps improve system security by closing unused and potentially risky ports.


# 🔒 Port Scanning and Firewall Hardening (AutoSecure)

This project automates the process of scanning and blocking open TCP ports on a Windows system. It uses **Nmap** to detect open ports and **Windows Defender Firewall** to block them through a **PowerShell script**, launched easily via a **batch file**.

---

## 🚀 Features

- Scans all TCP ports on `localhost (127.0.0.1)`
- Detects open ports using **Nmap**
- Automatically blocks open ports using **PowerShell**
- One-click execution via a `.bat` launcher
- Saves blocked port list in a timestamped log file

---

## 📁 Files

| File | Description |
|------|-------------|
| `AutoSecure.ps1` | PowerShell script that scans and blocks ports |
| `AutoSecure_Launcher.bat` | Batch file to run the script with one click |
| `Blocked_Ports_YYYYMMDD.txt` | Output log of blocked ports (generated automatically) |

---

## 🛠️ Requirements

- [Nmap](https://nmap.org/) (Add to system PATH)
- Windows PowerShell (pre-installed on Windows)
- Admin privileges to run firewall commands

---

## 📌 How to Use

1. Clone or download the repo.
2. Place both files in the same folder.
3. Right-click `AutoSecure_Launcher.bat` → **Run as administrator**.
4. View the log file for blocked ports.

---

## ⚠️ Notes

- Only TCP ports are scanned.
- Make sure **Nmap** is installed and added to your system PATH.
- Script runs on **localhost (127.0.0.1)** only.

