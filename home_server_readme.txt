🏠 Home Server Setup (Old Laptop)

A self-hosted home server built using an old laptop, designed to run
services, automate workflows, and provide a personal cloud environment.

------------------------------------------------------------------------

🚀 Overview

This project documents how I transformed an old laptop into a fully
functional home server. It is designed to be: - Lightweight -
Cost-effective - Scalable - Easy to maintain

The server runs various self-hosted services and can be accessed
remotely over the network.

------------------------------------------------------------------------

🧰 Tech Stack

-   OS: Linux (e.g. Ubuntu Server / Debian)
-   Containerisation: Docker
-   Remote Access: SSH
-   Networking: Local network + port forwarding (optional)

Optional Tools: - Docker Compose - Portainer - Tailscale / VPN

------------------------------------------------------------------------

⚙️ Setup Guide

1.  Prepare the Machine

-   Use an old laptop or PC
-   Ensure it is plugged in
-   Connect via Ethernet

2.  Install Operating System

-   Install a lightweight Linux distro
-   Enable SSH

3.  Update System sudo apt update && sudo apt upgrade -y

4.  Install Docker sudo apt install docker.io -y sudo systemctl enable
    docker sudo systemctl start docker

Optional: sudo apt install docker-compose -y

5.  Deploy Services docker run -d -p 8080:80 nginx

6.  Remote Access ssh username@your-server-ip

------------------------------------------------------------------------

📦 Features

-   Reuses old hardware
-   Full control over your data
-   Self-hosted services
-   Low power consumption
-   Great for learning DevOps / networking

------------------------------------------------------------------------

🛠 Future Improvements

-   Add reverse proxy
-   Set up domain + HTTPS
-   Automate deployments
-   Add monitoring

------------------------------------------------------------------------

⚠️ Notes

-   Keep your system updated
-   Secure your server before exposing it to the internet
-   Monitor temperatures if using a laptop long-term
