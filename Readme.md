🧭 How to Use the timezone_enforcer on macOS
Before running the script, make sure to disable the following options in System Settings → Date & Time:

Set date and time automatically

24-Hour Time

Set time zone automatically using your current location

🔧 Setup Instructions
Save the script with the name:

bash
Copy
Edit
timezone_enforcer.sh
Make it executable by running:

bash
Copy
Edit
chmod +x timezone_enforcer.sh
Start the enforcement:

bash
Copy
Edit
./timezone_enforcer.sh start
Stop and clean up if needed:

bash
Copy
Edit
./timezone_enforcer.sh stop
