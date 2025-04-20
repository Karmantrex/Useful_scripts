# 🕒 Timezone Enforcer for macOS

This script enforces the system timezone to **America/New_York (EST)** on macOS using a LaunchAgent and helper script.

---

## ⚙️ Before You Start

Before running the script, disable the following options under:

> **System Settings → General → Date & Time**

- [ ] Set date and time automatically  
- [ ] 24-Hour Time  
- [ ] Set time zone automatically using your current location  

These features must be turned off for the script to take full control of timezone settings.

---

## 🛠 Setup Instructions

1. **Save the script** with the following name:

    ```bash
    timezone_enforcer.sh
    ```

2. **Make it executable**:

    ```bash
    chmod +x timezone_enforcer.sh
    ```

3. **Start the timezone enforcement**:

    ```bash
    ./timezone_enforcer.sh start
    ```

4. **Stop and clean up if needed**:

    ```bash
    ./timezone_enforcer.sh stop
    ```

---

## ✅ What This Script Does

- Forces the timezone to **America/New_York**
- Reapplies the correct timezone every 30 minutes using a LaunchAgent
- Prevents user or system processes from changing it back
- Prompts for admin access only once per execution

---

## 💡 Pro Tip

If the timezone keeps reverting:
- Ensure **“Set time zone automatically using your current location”** is disabled
- Consider also turning off network time:
    ```bash
    sudo systemsetup -setusingnetworktime off
    ```
- SIP or MDM policies may override manual changes — confirm those are not interfering

---
