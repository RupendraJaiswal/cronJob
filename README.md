# ⏰ Render Keep‑Alive Cron Job Setup (Sampark Project)

## 📌 Overview

This README explains how to configure a cron job using **cron-job.org**
to keep the **Sampark application** awake on Render free tier by pinging
the login endpoint every **14 minutes**.

Render free-tier services automatically sleep after inactivity. This
scheduler prevents cold starts and ensures the application stays
responsive.

------------------------------------------------------------------------

## 🌐 Application Endpoint

Ping URL:

https://samaprk.onrender.com/login

This endpoint is triggered automatically every 14 minutes.

------------------------------------------------------------------------

## 🕒 Schedule Configuration

Cron Expression:

*/14 * \* \* \*

Meaning:

Runs once every 14 minutes continuously throughout the day.

------------------------------------------------------------------------

## ⚙️ Cron Job Platform

Scheduler used:

https://console.cron-job.org/

This service allows automated HTTP endpoint triggering at defined
intervals.

------------------------------------------------------------------------

## 🚀 Setup Instructions

Follow these steps:

1.  Open https://console.cron-job.org/
2.  Login or create an account
3.  Click **Create Cronjob**
4.  Enter details below:

Title: Render Login Ping

URL: https://samaprk.onrender.com/login

Schedule: Every 14 minutes

Cron Expression (Advanced Mode): */14 * \* \* \*

5.  Save the cron job

Setup completed successfully ✅

------------------------------------------------------------------------

## 📡 Expected Behavior

After configuration:

• Sends HTTP request every 14 minutes\
• Prevents Render service sleep\
• Reduces cold-start delays\
• Keeps application demo-ready 24×7

------------------------------------------------------------------------

## 🛠 Use Cases

Recommended for:

• Render free-tier deployments\
• Portfolio projects\
• Spring Boot applications\
• JSP-based applications\
• Recruiter demonstrations\
• Continuous uptime monitoring

------------------------------------------------------------------------

## 📍 Project Details

Application Name: Sampark

Deployment Platform: Render

Scheduler: cron-job.org

Ping Frequency: Every 14 minutes

------------------------------------------------------------------------

## ✅ Result

With this cron scheduler active, the **Sampark application stays awake
continuously**, ensuring faster response time and smoother
demonstrations without Render sleep interruptions.
