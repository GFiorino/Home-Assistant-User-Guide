# Home Assistant Automation Guide  

Automations in Home Assistant allow you to create **smart actions** based on triggers like time, motion, or device states. This guide explains how to set up automations using both the **UI** and **YAML configuration**.  

---

##  What Are Automations?  

Automations consist of three parts:  
1️⃣ **Triggers** – Events that start the automation (e.g., motion detected, sunset, button press).  
2️⃣ **Conditions** – (Optional) Conditions that must be met (e.g., only run at night).  
3️⃣ **Actions** – The result of the automation (e.g., turn on lights, send a notification).  

---

##  Creating Automations via UI (Beginner-Friendly)  

1. Go to **Settings > Automations & Scenes**.  
2. Click **Create Automation** and choose:  
   - **Start with a blueprint** (predefined templates)  
   - **Create from scratch** (manual setup)  
3. Configure the **Trigger**, **Condition (optional)**, and **Action**.  
4. Click **Save & Enable** to activate the automation.  

### **Example: Turn on Lights at Sunset**  
- **Trigger**: Sunset  
- **Condition**: None  
- **Action**: Turn on living room lights  

---

## 📝 Creating Automations via YAML (Advanced Users)  

For more flexibility, automations can be written in **YAML** inside `automations.yaml`.  

### **Example: Turn on Lights When Motion is Detected**  
Add the following to `automations.yaml`:  

```yaml
- alias: 'Turn on lights when motion is detected'
  trigger:
    - platform: state
      entity_id: binary_sensor.motion_sensor
      to: 'on'
  action:
    - service: light.turn_on
      target:
        entity_id: light.living_room
```

How to Apply Changes:

1-Save the file.

2-Restart Home Assistant to apply the automation.

---

##  Next Steps
Move on to Troubleshooting & FAQs to solve common automation issues.
