
---

# **RustScanner**  
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)  
![License](https://img.shields.io/badge/License-MIT-green)  
![Ethical Use](https://img.shields.io/badge/Ethical%20Use-Required-red)  

**RustScanner** is a Python-based **network reconnaissance toolkit** with **web interface** and **visual traffic analysis**. Designed for **penetration testers**, **sysadmins**, and **security researchers**.  

⚠️ **Legal Notice**:  
> Use only on networks you own or have permission to scan. Unauthorized scanning is illegal.  

---

## **🚀 Key Features**  
### **1. Scanning Capabilities**  
| **Category**         | **Tools**                                  |  
|----------------------|-------------------------------------------|  
| **Host Discovery**   | ICMP/ARP/TCP SYN Scans                    |  
| **Port Scanning**    | SYN (Stealth), Connect, UDP               |  
| **Service Detection**| Banner Grabbing (HTTP/SSH/FTP/SMB)        |  
| **Traffic Analysis** | **EtherApe** Integration (Live Visuals)   |  

### **2. Web Interface** 🌐  
- **Flask-based dashboard** (port `5000`)  
- Real-time scan results  
- Interactive network maps  
- **REST API** for automation  

### **3. Performance**  
- Multi-threaded scans  
- Async I/O for faster results  

---

## **🛠️ Installation**  
### **Automated Setup**  
```bash
git clone https://github.com/yourusername/RustScanner.git
cd RustScanner
chmod +x install.sh
bash install.sh  # Installs Python deps + EtherApe + Nmap
python3 install.py
```

### **Manual Installation**  
```bash
# Debian/Ubuntu
sudo apt install -y python3-pip nmap etherape
pip3 install -r requirements.txt

# Arch Linux
sudo pacman -S python-pip nmap etherape
pip3 install -r requirements.txt

# Fedora
sudo dnf install python3-pip nmap etherape
pip3 install -r requirements.txt
```

---

## **💻 Usage**  
### **Run Command**  
```bash
# Basic scan
sudo python3 main.py
```


## **📊 Output Formats**  
- **Terminal**: Color-coded results  
- **Web Dashboard**: Interactive tables/graphs  
- **Files**: CSV/JSON/TXT exports  

---

## **📜 License**  
MIT License. See [LICENSE](LICENSE).  

--- 

**Happy (ethical) hacking!** 🔍  
