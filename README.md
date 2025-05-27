# MineIdle

**MineIdle** is a web-based control panel and agent manager for Minecraft accounts. It allows users to connect idle agents to their own Minecraft servers to simulate presence, send messages, perform anti-AFK actions, and manage reconnects — all through a web interface.

> ✅ MineIdle **does not bypass authentication or license checks**, and is intended only for **personal use**, such as testing or managing agents on your own servers or servers where you have **explicit permission**. This project respects Mojang’s [EULA](https://www.minecraft.net/en-us/eula) and [Usage Guidelines](https://aka.ms/mcusageguidelines).

---

## 🧩 Features

- 🌐 Control your Minecraft agents via web dashboard
- 🔐 Microsoft OAuth2 login (securely manages authentication tokens)
- 🧠 Simulate presence with idle movement, chat, jump, swing, etc.
- 🔁 Automatic reconnect support
- 💬 Join/world change messages
- 📡 View current in-game position of agents
- 🔒 Proxy support (SOCKS5, HTTPS)
- ☁️ MongoDB for saving user preferences

---

## ⚙️ Tech Stack

- **Backend:** Node.js + Express
- **Frontend:** React (via separate repo)
- **Minecraft Agent Engine:** [mineflayer](https://github.com/PrismarineJS/mineflayer)
- **Database:** MongoDB
- **Authentication:** Microsoft Azure OAuth2 (via [msal-node](https://github.com/AzureAD/microsoft-authentication-library-for-js))

