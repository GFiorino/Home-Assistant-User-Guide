# Home Assistant Installation Guide  

This guide will walk you through installing Home Assistant on different platforms: **Raspberry Pi, Docker, and Windows**.  

## 📌 System Requirements  
Before you begin, ensure you have:  
- A **Raspberry Pi 4 (Recommended) or higher** with a microSD card (for Pi installations)  
- **Docker installed** (for Docker setup)  
- **Windows 10/11** (for Windows installations)  
- A stable **internet connection**  

---

## 🖥️ Installation on Raspberry Pi  
### **1️⃣ Download Home Assistant OS**  
1. Download the latest **Home Assistant OS** image for Raspberry Pi from [here](https://www.home-assistant.io/installation/raspberrypi).  
2. Flash the image onto a **microSD card** using [balenaEtcher](https://www.balena.io/etcher/).  

### **2️⃣ Insert the microSD card & Boot**  
1. Insert the microSD card into the **Raspberry Pi** and power it on.  
2. Wait for the installation to complete (this may take a few minutes).  

### **3️⃣ Access Home Assistant**  
1. Once installed, open a browser and visit:  
http://homeassistant.local:8123
2. Follow the on-screen setup wizard to complete the installation.  

---

## 🐳 Installation with Docker  
### **1️⃣ Install Docker**  
If you don’t have Docker installed, follow [this guide](https://docs.docker.com/get-docker/).  

### **2️⃣ Run the Home Assistant Container**  
Run the following command in your terminal:  
```sh
docker run -d \
--name homeassistant \
--restart unless-stopped \
-v /path/to/your/config:/config \
--network=host \
ghcr.io/home-assistant/home-assistant:stable
```

👉 Replace /path/to/your/config with a valid directory on your system.

### **3️⃣ Access Home Assistant**
Once the container is running, visit:

```arduino
http://localhost:8123
```

---

## 🪟 Installation on Windows

### **1️⃣ Install Home Assistant via Virtual Machine**
Download and install VirtualBox from here.
Download the Home Assistant VDI image from the official site.
Create a new VM in VirtualBox and attach the Home Assistant disk.

### **2️⃣ Start Home Assistant**

1-Power on the VM and wait for Home Assistant to boot.

2-Open a browser and go to:

```arduino
http://homeassistant.local:8123
```
3-Follow the setup wizard.

---

### 🎯 Next Steps
Once installed, move to Configuration & Setup to connect your smart devices!

