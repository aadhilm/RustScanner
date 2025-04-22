
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
./install.sh  # Installs Python deps + EtherApe + Nmap
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
### **1. CLI Mode**  
```bash
# Basic scan
python3 rustscanner.py --target 192.168.1.0/24

# Advanced scan (SYN + OS detection)
python3 rustscanner.py --target 10.0.0.1 --scan-type syn --os-detection
```

### **2. Web Interface**  
```bash
python3 webapp.py  # Starts at http://localhost:5000
```
![Web Interface Preview](https://i.imgur.com/example.png)  

### **3. EtherApe Integration**  
Visualize live traffic:  
```bash
sudo etherape -i eth0 -f "host 192.168.1.100"  # Filter specific host
```
![EtherApe Demo](https://i.imgur.com/example2.png)  

---

## **📊 Output Formats**  
- **Terminal**: Color-coded results  
- **Web Dashboard**: Interactive tables/graphs  
- **Files**: CSV/JSON/TXT exports  

---

## **📜 License**  
MIT License. See [LICENSE](LICENSE).  

---

## **🔗 Extras**  
- **[REST API Docs](api.md)**  
- **[Sample Reports](samples/)**  

**Happy (ethical) hacking!** 🔍  

--- 

### **Key Additions**:  
1. **Web Interface Section** - Added details about Flask dashboard  
2. **EtherApe Integration** - Instructions for traffic visualization  
3. **Screenshots** - Placeholder links for UI previews  
4. **REST API** - Mentioned for automation  

For actual screenshots, replace the placeholder Imgur links with your tool's images.
