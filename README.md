# MineIdle

**MineIdle** is a modern, web-based control panel for managing multiple Minecraft accounts on private or authorized servers. It allows users to launch lightweight, headless Minecraft sessions in the cloud, simulate presence, automate idle behaviors, and monitor real-time activity all from a user friendly dashboard.

Designed for reliability, scalability, and ease of use, MineIdle is ideal for users who want their Minecraft accounts to remain online 24/7 without keeping their PC running.

> ⚠️ MineIdle is currently in **active development** and is intended for **personal or authorized use only**. All features are developed in compliance with Mojang’s [End User License Agreement (EULA)](https://www.minecraft.net/en-us/eula) and [Usage Guidelines](http://aka.ms/mcusageguidelines).

---

##  Overview

MineIdle lets users securely authenticate their Minecraft accounts via Microsoft OAuth2 and launch idle sessions on trusted servers. These sessions are managed through an interactive dashboard and are perfect for testing, presence simulation, or server maintenance roles.

Each session operates without rendering the Minecraft client and consumes minimal system resources. All settings are stored per user and persist between sessions.

---

##  Key Features

- 🌐 **Web Dashboard** – Full control of your accounts through a clean interface
- 🔐 **Secure Microsoft Login** – OAuth2 + refresh token support via MSAL
- 🧠 **Idle / Anti-AFK Actions** – Move, swing, chat, look, jump automatically
- 🔁 **Auto-Reconnect** – Reconnect agents after server disconnects
- 💬 **Join & World Events** – Broadcast messages when entering worlds or joining servers
- 📡 **Live Monitoring** – Real-time position tracking (X, Y, Z)
- 🌍 **Proxy Support** – Route traffic via HTTPS or SOCKS5 proxies
- ☁️ **Persistent User Data** – Profiles and settings saved across sessions

---

##  Architecture

MineIdle uses a clean, modular architecture:

| Layer      | Technology                  | Purpose                             |
|------------|-----------------------------|-------------------------------------|
| Backend    | Node.js, Express            | API routing, bot session control    |
| Frontend   | React *(external repo)*     | Real-time web interface             |
| Bot Engine | mineflayer                  | Minecraft protocol automation       |
| Auth       | Microsoft OAuth2 + MSAL     | Secure login, token refresh         |
| Database   | MongoDB                     | Stores user profiles & bot configs  |

---

## ☁ Hosting & Scaling Strategy

MineIdle is designed for **cloud deployment** and will run on **dedicated VPS infrastructure or scalable cloud services** depending on demand.

Initial launch will be deployed on high-uptime VPS instances, with long-term plans to support:

- Horizontal scaling via Docker/Kubernetes
- Load balancing per user session cluster
- Geo-distributed nodes for latency-sensitive performance

Users will manage their accounts from anywhere through **https://mineidle.xyz**.

Dashboard (not finished):

![image](https://github.com/user-attachments/assets/f5a693c1-1b6f-49ac-9892-f298411a3b8a)
![image](https://github.com/user-attachments/assets/c2968ee4-a799-4cf8-a8a5-d1a92547c7e5)
![image](https://github.com/user-attachments/assets/c2a162ea-d267-4ea5-a471-fb47e1d36250)
![image](https://github.com/user-attachments/assets/10bfa187-751a-4890-8549-4ff3376fe653)
![image](https://github.com/user-attachments/assets/1a5c7b9f-db0b-4701-8bc1-942bca940ac9)







---

##  Subscription Model

MineIdle will operate as a **subscription-based service**:

- ✅ Users register accounts on the platform
- ✅ Add Microsoft-authenticated Minecraft accounts
- ✅ Configure session behaviors per account
- ✅ Monitor activity & manage sessions remotely

All data is isolated per user and stored securely.

> Subscription plans will be announced after public release. Currently in private alpha.

---

## 🚀 Roadmap

| Status | Feature                                          
|--------|------------------------------------------------- 
| ✅     | Microsoft OAuth2 login w/ refresh token support  
| ✅     | Headless Minecraft sessions via mineflayer       
| ✅     | Per-user MongoDB integration                     
| ✅     | Proxy and AFK simulation features                
| ⏳      | Final React dashboard & mobile support           
| ⏳      | AppID approval request from Microsoft to allow seamless server connections without the need for device authcode         
| ⏳      | Public SaaS launch with monthly billing          

---

##  Security & Compliance

- Uses **official Microsoft APIs** — no spoofing or license circumvention
- Refresh tokens are **securely encrypted at rest**
- All network traffic is protected using HTTPS
- Fully adheres to Mojang's EULA and developer guidelines

MineIdle is not a cheat client and is intended only for idle use, account presence, or personal server management.

---

##  License & Usage

MineIdle is provided for **personal, educational, and authorized use only**.

NOT AN OFFICIAL MINECRAFT SERVICE. NOT APPROVED BY OR ASSOCIATED WITH MOJANG OR MICROSOFT.

Do not use it on public servers that forbid alternate accounts, bots, or automated play. Always respect server rules.

---

##  Acknowledgements

- [PrismarineJS](https://github.com/PrismarineJS) – for the mineflayer bot engine
- [Microsoft Identity Platform](https://learn.microsoft.com/en-us/azure/active-directory/develop/) – for secure user auth
- [MongoDB Atlas](https://www.mongodb.com/) – for hosted document database support




