# RustScanner
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)  
![License](https://img.shields.io/badge/License-MIT-green)  
![Ethical Use](https://img.shields.io/badge/Ethical%20Use-Required-red)  

**Net Scanner** is a powerful Python-based tool for network reconnaissance, designed to discover active hosts, open ports, and running services. Ideal for **penetration testers**, **sysadmins**, and **security enthusiasts**.  

⚠️ **Disclaimer**:  
> This tool is for **authorized security testing only**. Unauthorized scanning may violate laws. Use responsibly!  

---

## **🎯 Introduction**  
A lightweight yet robust network scanner that combines:  
- **Host discovery** (ICMP/ARP/TCP SYN scans)  
- **Port scanning** (SYN, Connect, UDP)  
- **Service detection** (Banner grabbing)  
- **OS fingerprinting** (Nmap integration)  


---

## **🔧 Features**  
| **Category**         | **Tools/Functions**                          |  
|----------------------|---------------------------------------------|  
| **Host Discovery**   | ICMP Ping, ARP Scan, TCP SYN Scan           |  
| **Port Scanning**    | SYN (Stealth), Connect, UDP Scans           |  
| **Service Detection**| Banner grabbing (HTTP, SSH, FTP, etc.)      |  
| **Reporting**        | Export results to CSV, JSON, TXT            |  
| **Performance**      | Multi-threaded for faster scans             |  

All in a **user-friendly CLI/GUI** interface.  

---

### **System Integration**  
- **Auto-detects** your Linux distro (Debian/Arch/Fedora)  
- **Installs all dependencies** (Python packages + system tools)  
- **Verifies installations** before execution
  

## **📦 Installation**  
### **Prerequisites**  
- Python 3.8+  
- Root/Admin access (for raw packets)  

### **1. Clone the Repository**  
```bash  
git clone https://github.com/yourusername/net-scanner.git  
cd net-scanner  
```  

### **2. Install Dependencies**  
**Automated Install:**  
```bash  
chmod +x install.sh  
./install.sh  
```
```python
python install.py  
```  

### ** Manual Installation (If Needed)**  
```bash
# For Debian/Ubuntu:
sudo apt update && sudo apt install -y python3-pip arp-scan nmap
pip3 install -r requirements.txt

# For Arch:
sudo pacman -Syu python-pip arp-scan nmap
pip3 install -r requirements.txt

# For Fedora:
sudo dnf install python3-pip arp-scan nmap
pip3 install -r requirements.txt
```

### **3. Run Net Scanner**  
```bash  
python net_scanner.py
```  
---

## **📋 Tool Categories**  
### **1. Host Discovery**  
- **ICMP Ping**: Check live hosts.  
- **ARP Scan**: Local network device discovery.  
- **TCP SYN Scan**: Stealthy host detection.  

### **2. Port Scanning**  
- **SYN Scan**: Fast and stealthy.  
- **UDP Scan**: For DNS, SNMP, etc.  

### **3. Service Detection**  
- Fetch banners (e.g., `Apache/2.4.41`).  

### **4. Reporting**  
- Export to CSV/JSON for further analysis.  

---

## **📝 License**  
MIT License. See [LICENSE](LICENSE).  

---

## **🤝 Contributing**  
1. **Report bugs** via Issues.  
2. **Suggest features** (e.g., GUI, API integration).  
3. **Submit PRs** (follow PEP 8 guidelines).

---
**Happy Scanning!** 🚀  
---
