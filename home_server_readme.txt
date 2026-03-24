VIDEO USED: https://www.youtube.com/watch?v=46T4cDQBkDs
CREDIT:TECH BY MATT

🏠 Home Server Setup (Old Laptop)

A self-hosted home server built using an old laptop, designed to run
services, automate workflows, and provide a personal cloud environment.

------------------------------------------------------------------------

🚀 Overview

This project documents how I transformed an old laptop into a fully
functional home server. It is designed to be: - Lightweight -
Cost-effective - Scalable - Easy to maintain

The server runs various self-hosted services and can be accessed
remotely over any network.

------------------------------------------------------------------------

🧰 Tech Stack

-   OS: Linux (e.g. Ubuntu Server / Debian)
-   Containerisation: Docker (CasaOS) 
-   Remote Access: SSH
-   Networking: Local network (ethernet)
- 

Required Tools: USB Drive (8GB+), 2nd Computer

------------------------------------------------------------------------

⚙️ Setup Guide

1.  Prepare the Machines

-   Use an old laptop or PC
-   Ensure it is plugged in to power
-   Connect via Ethernet
-   Turn the laptop off
-   Insert the USB drive into your 2nd Computer (not the server laptop)

2.  Install Operating System

-   Install Ubuntu Server  https://ubuntu.com/server
-   Download balenaEtcher for the operating system of you main computer (NOT THE SERVER'S OS)  https://etcher.balena.io/
-   Open balenaEtcher
-   Click Flash from file -> select the Ubuntu Server file you just downloaded
-   Click Select Target -> choose the usb drive which you plan to use to transfer the OS to the server laptop (EVERYTHING ON THIS USB WILL BE DELETED SO DONT USE A USB WITH ANYTHING IMPORTANT ON IT)
-   Click Flash
-   Once the flash is complete, take the USB drive out of the 2nd Computer and insert it into the server laptop
-   Turn the laptop on, spam f12 or del to eneter the BIOS, then change the main Boot Device to the USB DRIVE

3.  Update System: 
sudo apt update 
sudo apt upgrade -y

4.  Remote Access ssh username@your-server-ip

------------------------------------------------------------------------

📦 Features

-   Reuses old hardware
-   Full control over your data
-   Self-hosted services
-   Low power consumption
-   Great for learning DevOps / networking

------------------------------------------------------------------------

🛠 Future Improvements

-   Set up domain + HTTPS
-   Automate deployments
-   Add monitoring

------------------------------------------------------------------------

⚠️ Notes

-   Keep your system updated
-   Secure your server before exposing it to the internet
-   Monitor temperatures if using a laptop long-term
