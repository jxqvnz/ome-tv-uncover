<div align="center">

# 🎥 OmeTV Uncover

### WebRTC peer-IP detection & geolocation for OmeTV video chat

**Pure JavaScript userscript · Zero dependencies · Paste & run**

[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](LICENSE)
[![Dependencies](https://img.shields.io/badge/Dependencies-ZERO-success?style=for-the-badge)]()
[![Platform](https://img.shields.io/badge/Platform-Chromium%20Browsers-lightgrey?style=for-the-badge)]()
[![API](https://img.shields.io/badge/API-IPGeolocation-blue?style=for-the-badge)](https://ipgeolocation.io/)

> *"On the Internet, nobody knows you're a dog." — Peter Steiner, The New Yorker*

</div>

---

## 🚀 Features

| 🛰️ Detection | 🌍 Geolocation | 🎥 Capture | 🎨 Interface |
|---|---|---|---|
| WebRTC **ICE candidate analysis** — reveals the remote peer's public IP | Country, region, city, ISP & timezone via the **IPGeolocation API** | Automatic **snapshot** of the remote video stream | Modern **draggable** floating panel |
| Pure client-side — **no server, no install** | IP → location enrichment with **latitude & longitude** | Square preview refreshed per peer | **Minimize** and **close** controls |

### ✨ Highlights

- 🎯 **WebRTC-based detection** — reads the remote peer's public IP straight from the ICE negotiation
- 🗺️ **Rich geolocation** — country, region, city, ISP, languages, timezone, UTC offset
- 📸 **Auto video snapshot** — captures the remote stream the moment it starts playing
- 🧲 **Draggable UI** — move, minimize, or close the panel whenever you want
- ⚡ **Lightweight & fast** — zero dependencies, paste and go

---

## 📦 Requirements

- A modern **Chromium-based browser** (Chrome, Edge, Brave, Opera…)
- An **IPGeolocation API key** (free tier available)
- An **OmeTV account**

---

## 🔧 Setup Guide

### 1. Create an IPGeolocation account

Head over to [https://ipgeolocation.io/](https://ipgeolocation.io/) and register a **free account**.

### 2. Copy your API key

After signing in, open your **dashboard** and copy your API key:

```
IPGeolocation API Key: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
```

### 3. Configure the script

Inside the script, replace:

```javascript
let apiKey = "";
```

with:

```javascript
let apiKey = "YOUR_API_KEY";
```

### 4. Open OmeTV

Go to [https://ome.tv/](https://ome.tv/) and sign in.

### 5. Open Developer Tools

Press **F12** or **Ctrl + Shift + I**.

### 6. Open the Console

Select the **Console** tab.

If Chrome shows:

> ⚠️ *Warning: Don't paste code into the DevTools Console…*

type:

```text
allow pasting
```

and press **Enter**.

### 7. Run the script

Paste the **entire script** into the Console and press **Enter**.

### 8. Start using OmeTV Uncover

Once you're connected to another user, the floating panel automatically displays all available information.

---

## 📊 Information Displayed

| 🌐 Network | 🗺️ Location | ⏰ Time |
|---|---|---|
| Public IP address | Country | Current local time |
| ISP | Region / State | UTC offset |
| | City | Timezone |
| | Languages | |
| | Latitude & Longitude | |
| | 🎥 Remote video snapshot | |

---

## 📸 Real Output

```
┌─ OmeTV Uncover ───────────────────────────────┐
│                                              │
│   🎥 [ remote video snapshot ]               │
│                                              │
│   🌐 IP        203.0.113.42                  │
│   🌍 Country   Czechia                       │
│   📍 Region    Prague                        │
│   🏙️ City      Prague                        │
│   🏢 ISP       Example ISP                   │
│   ⏰ Time      14:32:05 (UTC+2)              │
│                                              │
│   [ — ]  [ ✕ ]                               │
└──────────────────────────────────────────────┘
```

---

## 🧠 How It Works

1. **Monitor** — hooks into the WebRTC connection that OmeTV creates for each video chat
2. **Detect** — extracts the remote peer's **public IP** from the ICE candidate exchange
3. **Enrich** — queries the **IPGeolocation API** for approximate geolocation data
4. **Capture** — snapshots the remote video stream as soon as it becomes available
5. **Display** — renders everything in a modern draggable floating panel

> 📌 This project displays **approximate IP-based geolocation** using publicly available network information. The reported location is an *estimate* and should **not** be considered the user's exact physical location.

---

## ⚠️ Legal Notice

This tool is intended for **educational and authorized security testing only**. You are **solely responsible** for complying with applicable laws and the **OmeTV Terms of Service**.

- 🔒 Only use this on connections you are authorized to inspect
- 🎓 Use it to understand WebRTC privacy implications and IP-leak risks
- ⚖️ The author is **not responsible** for anything done with this program

**Use it only for legal, ethical, and educational purposes.**

---

## 📄 License

Distributed under the **MIT License**. See `LICENSE` for more information.

---

<div align="center">

**Made with 🖤 by [your-username](https://github.com/your-username)**

*Star ⭐ this repo if you found it useful!*

</div>
