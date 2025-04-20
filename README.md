# 🕒 Timezone Enforcer for macOS

This script enforces the system timezone to **America/New_York (EST)** on macOS using a LaunchAgent and helper script.

## ⚙️ Before You Start

Before running the script, make sure to **disable the following options** in:

> **System Settings → General → Date & Time**

- [ ] Set date and time automatically  
- [ ] 24-Hour Time  
- [ ] Set time zone automatically using your current location  

These features must be turned off for the script to take full control of timezone settings.

---

## 🔧 Setup Instructions

1. **Save the script** with the following name:
   ```bash
   timezone_enforcer.sh
