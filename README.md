# MineIdle

**MineIdle** is a secure, web-based platform designed to help users manage their own Minecraft accounts efficiently. It allows individuals to launch lightweight, headless Minecraft sessions via a browser-controlled dashboard—ideal for staying connected to personal or authorized servers without running the full Minecraft client locally.

> ⚠️ MineIdle is in active development. It is intended strictly for **personal or authorized use only** and fully complies with Mojang’s [EULA](https://www.minecraft.net/en-us/eula) and [Usage Guidelines](http://aka.ms/mcusageguidelines).

---

## Overview

MineIdle enables users to securely authenticate their Minecraft accounts via Microsoft OAuth2 and manage session behavior from a personal dashboard. These sessions consume minimal resources and are ideal for testing, keeping farms loaded, or simulating idle activity on servers where alternate accounts are allowed.

---

## Key Features

- **Web Dashboard** – Manage Minecraft accounts via an intuitive UI
- **Microsoft Login (OAuth2)** – Secure login flow with refresh token support
- **Idle / Anti-AFK** – Configure behaviors like movement, jumping, looking, etc.
- **Auto-Reconnect** – Recover from disconnects automatically
- **World Event Messages** – Custom messages on join, respawn, or world change
- **Live Coordinates** – Track position in real time (X, Y, Z)
- **Proxy Support** – Route connections via SOCKS5 or HTTPS proxies
- **Persistent User Settings** – Per-user config stored securely in the database

---

## Architecture

| Layer      | Technology              | Purpose                               |
|-----------|--------------------------|----------------------------------------|
| Backend   | Node.js, Express         | API routing, session orchestration     |
| Frontend  | React *(external repo)*  | Real-time user interface               |
| Bot Engine| [mineflayer](https://github.com/PrismarineJS/mineflayer) | Minecraft protocol control             |
| Auth      | Microsoft OAuth2 + MSAL  | Secure login and token management      |
| Database  | MongoDB                  | Persistent storage for user data       |

---

## ☁ Hosting & Scaling

MineIdle is built for deployment on modern infrastructure and will initially run on dedicated VPS instances. As demand increases, we plan to support:

- Docker-based horizontal scaling
- Kubernetes orchestration
- Geo-distributed deployment for latency optimization

All users access the service securely via [https://mineidle.xyz](https://mineidle.xyz), managing their sessions from anywhere.

---

## Subscription Model

MineIdle is offered as a **monthly subscription service**. Each user can:

- Register securely on the platform
- Add and authenticate their own Minecraft accounts
- Configure behaviors and proxy use per account
- Launch and monitor idle sessions in real time

> Subscription tiers will be announced at public launch. The service is currently in private alpha.

Dashboard (not finished):

![image](https://github.com/user-attachments/assets/f5a693c1-1b6f-49ac-9892-f298411a3b8a)
![image](https://github.com/user-attachments/assets/c2968ee4-a799-4cf8-a8a5-d1a92547c7e5)
![image](https://github.com/user-attachments/assets/c2a162ea-d267-4ea5-a471-fb47e1d36250)
![image](https://github.com/user-attachments/assets/10bfa187-751a-4890-8549-4ff3376fe653)
![image](https://github.com/user-attachments/assets/1a5c7b9f-db0b-4701-8bc1-942bca940ac9)



## 🚀 Roadmap

| Status | Feature                                                                 |
|--------|-------------------------------------------------------------------------|
| ✅     | Microsoft OAuth2 login with refresh support                             |
| ✅     | Headless Minecraft sessions with mineflayer                             |
| ✅     | Per-user MongoDB integration                                            |
| ✅     | Anti-AFK actions and proxy routing                                      |
| ✅     | In-browser chat interface and monitoring                                |
| ⏳     | Final UI polish + mobile-friendly dashboard                             |
| ⏳     | AppID whitelisting (Microsoft) for seamless access without device code  |
| ⏳     | Public SaaS launch with billing system                                  |

---

## 🔐 Security & Compliance

- Microsoft tokens encrypted at rest using AES-256
- All traffic encrypted via HTTPS
- No token spoofing, license bypassing, or unauthorized automation
- Fully aligns with Mojang’s EULA and Microsoft’s OAuth guidelines

MineIdle is **not a modded client**, **not a cheat tool**, and **not for public server abuse**. It is built strictly for idle presence on servers that allow such use.

---

## ⚠ Usage Notice

This service is:

- For educational, personal, and server-authorized purposes only
- Not affiliated with Mojang, Microsoft, or the official Minecraft brand
- Not to be used on servers that prohibit alternate accounts or automation

Respect all server rules and use this tool responsibly.

---

## 🙌 Acknowledgements

- [PrismarineJS](https://github.com/PrismarineJS) – for mineflayer
- [Microsoft Identity Platform](https://learn.microsoft.com/en-us/azure/active-directory/develop/) – for secure OAuth2 login
- [MongoDB Atlas](https://www.mongodb.com/) – for hosted database support

---

**Not an official Minecraft product. Not approved by or associated with Mojang or Microsoft.**




