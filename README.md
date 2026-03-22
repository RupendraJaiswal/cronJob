⏰ Render Login Ping Cron Job Setup

This cron job is configured using cron-job.org to periodically ping the application login endpoint and prevent the Render free-tier service from going idle.

📌 Purpose

Render’s free-tier services may go to sleep after inactivity.
To keep the application active, a scheduled request is sent every 14 minutes to the login endpoint.

🔗 Ping URL
https://samaprk.onrender.com/login
🕒 Schedule

The cron job runs every 14 minutes.

Example cron expression:

*/14 * * * *
⚙️ Configuration Steps (cron-job.org)
Go to https://console.cron-job.org/
Login to your account
Click Create Cronjob

Configure:

Title

Render Login Ping

URL

https://samaprk.onrender.com/login

Schedule

Every 14 minutes
Save the cron job ✅
📡 Expected Behavior
Sends HTTP request every 14 minutes
Keeps Render service active
Reduces cold start delays
Improves application responsiveness
🛠 Use Case

Useful for:

Render free-tier apps
Demo environments
Portfolio projects
Spring Boot / JSP hosted apps like Sampark
