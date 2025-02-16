# 🔍 Open Port Scanner using Nmap & Sockets

This project demonstrates **two methods** to scan open ports on a target host:
1. **Using Nmap** (`portScannerusingNmap.py`) → Leverages the **Nmap** library for scanning.
2. **Using Sockets** (`usingSocket.py`) → Implements a basic port scanner using **Python sockets**.

---
---

## 🛠️ Prerequisites
- **Python 3.x** installed
- Install dependencies using:
  ```sh
  pip install python-nmap
  ```
  # 1️⃣ Port Scanning using Nmap

## 📝 Introduction
Nmap (Network Mapper) is a powerful network scanning tool used to detect open ports, services, and security vulnerabilities.  
This script utilizes the `python-nmap` library to automate Nmap scanning.

## ⚙️ How It Works
1. Defines a port range (`begin=50, end=500`).
2. Specifies a target IP address (`target='15.207.169.232'`).
3. Uses `nmap.PortScanner()` to scan each port in the range.
4. Extracts the port status (open/closed) from the scan results.
5. Displays the output.

## 🚀 Run the Script
To run the script, execute the following command in your terminal:

```bash
python portScannerusingNmap.py
```
# 2️⃣ Port Scanning using Python Sockets

## 📝 Introduction
Python's socket module allows direct interaction with network services.  
This script performs a basic port scan without requiring external tools like Nmap.

## ⚙️ How It Works
1. Prompts the user to input a target hostname.
2. Resolves the IP address of the target.
3. Iterates through ports 9039 to 9050.
4. Attempts to establish a TCP connection to each port.
5. If successful, marks the port as open; otherwise, it is closed.
6. Prints the time taken to complete the scan.

## 🚀 Run the Script
To run the script, execute the following command in your terminal:

```bash
python usingSocket.py
```