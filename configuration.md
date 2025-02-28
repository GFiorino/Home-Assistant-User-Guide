# Home Assistant Configuration & Setup Guide  

After installing Home Assistant, the next step is **configuring it to connect smart devices** and **customizing your dashboard** for better control.  

---

## 🏠 Accessing the Home Assistant UI  

1. Open your browser and go to:  
http://homeassistant.local:8123
2. Log in using the credentials you created during installation.  
3. You will see the **Home Assistant dashboard**, where you can start adding devices.  

---

## 🔌 Adding Smart Devices  

### **1️⃣ Auto-Discovery (Recommended)**  
Home Assistant can automatically detect supported smart devices on your network.  

1. Navigate to **Settings > Devices & Services**.  
2. If a device is detected, click **Configure** and follow the setup process.  

👉 Supported devices include smart bulbs, sensors, thermostats, and more.  

### **2️⃣ Manually Adding a Device**  
If a device is not auto-detected, you can add it manually:  

1. Go to **Settings > Integrations**.  
2. Click **Add Integration** and search for the device type (e.g., Philips Hue, MQTT, Z-Wave).  
3. Follow the setup instructions for the integration.  

---

## 🎨 Customizing Your Dashboard  

### **1️⃣ Accessing the Dashboard**  
1. Click **Overview** in the sidebar to see the default dashboard.  
2. Click the three dots (⋮) in the top right and select **Edit Dashboard**.  

### **2️⃣ Adding Cards & Widgets**  
1. Click **Add Card** to choose from various widgets (e.g., temperature, lights, cameras).  
2. Drag and arrange cards for a custom layout.  
3. Save your changes.  

👉 You can also use **Lovelace UI** for advanced dashboard customization.  

---

## 🎯 Next Steps  

Now that your devices are connected and the dashboard is set up, move on to:  
👉 **[Automation Guide](./automation.md)** – Learn how to create automations for your smart home!  
