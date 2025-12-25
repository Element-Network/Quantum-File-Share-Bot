# 🌐 **QuantumShare: The Next-Gen Telegram File Share Bot**
### **Empowering Communities with Secure, Scalable, and Inclusive Access Management**

**QuantumShare** is a powerful, ethically engineered platform that redefines Telegram bot functionality. Built for dynamic communities and modern business models, it delivers instant file delivery, sophisticated access gating, and comprehensive management tools with a focus on fairness and transparency.

[![Python](https://img.shields.io/badge/Language-Python%203.10%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Telegram Bot](https://img.shields.io/badge/Platform-Telegram%20Bot-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://core.telegram.org/bots)
[![Data Integrity](https://img.shields.io/badge/Data-MongoDB%20Backed-47A248?style=for-the-badge&logo=mongodb)](https://www.mongodb.com/)
[![Element-Network](https://img.shields.io/badge/License-Element--Network-blue?style=for-the-badge&logo=opensource)](#-License)


<h3 align="center">
    ─「 sᴜᴩᴩᴏʀᴛ 」─
</h3>

<p align="center">
<a href="https://t.me/Element_Support"><img src="https://img.shields.io/badge/-Support%20Group-blue.svg?style=for-the-badge&logo=Telegram"></a>
</p>
<p align="center">
<a href="https://t.me/Element_Bots"><img src="https://img.shields.io/badge/-Support%20Channel-blue.svg?style=for-the-badge&logo=Telegram"></a>
</p>

---

## 🚀 **New Features (v2.0 Update)**

| Feature | Description |
| :--- | :--- |
| **🌍 Public Mode** | Democratize file sharing! Toggle `/public_mode` to allow non-admins to store files. Includes a robust **Public Batch** system. |
| **📦 Public Batch** | Users can now create batch links for up to **50 files** at once using their own channels. |
| **📜 System Logging** | Full access to bot logs via `/log` and `/clear_log` for debugging and monitoring directly from Telegram. |
| **📂 File-Based Reporting** | Large lists (Users, Bans, Admins) are now generated as **.txt files** to bypass Telegram message limits. |
| **📊 System Stats** | Detailed server resource monitoring via `/usage` (CPU, RAM, Swap, Disk, Network). |

---

## ⚡️ **Feature Deep Dive**

### 🔐 **Access Control & Monetization**
* **Smart Force Subscription (FSUB):** Supports **unlimited** verification channels. Access is granted through a unique, **request-based** link.
* **Time-Bound Resources:** Configure links with mandatory **auto-expiry timers** (configurable in `setup.json`).
* **Premium User Management:** Full lifecycle management using `/add_premium`, `/remove_premium`, and `/list_premiums`.

### 🌍 **Public Mode (New!)**
* **Toggleable Access:** Admins can turn public uploading on/off.
* **Smart Footers:** When a public user uploads a file, their info is stamped on the file caption in the DB. When retrieved by others, the footer is **cleanly removed**.
* **Batch Capabilities:** Users can batch up to 50 files from their own channels if the bot is an admin there.

### 📈 **Data & Communication**
* **Real-time Analytics:** Track metrics via `/stats` (Database) and `/usage` (Server Resources).
* **Mass Broadcast:** Engage your user base with `/broadcast` (photo + caption) and `/pbroadcast` (pins the message).
* **Logs & Lists:** Fetch comprehensive lists of users, admins, or banned members as files.

---

## 🛠️ **BotFather Setup (Copy & Paste)**

Use these sections to configure your bot's command menu in **[@BotFather](https://t.me/BotFather)**.

### 1️⃣ Admin Commands (Full List)
*Use this list if you want to see ALL commands, including restricted tools.*

```text
start - ɪɴɪᴛɪᴀᴛᴇꜱ ᴏʀ ʀᴇꜱᴛᴀʀᴛꜱ ᴛʜᴇ ʙᴏᴛ ꜱᴇʀᴠɪᴄᴇ.
usage - ᴅɪꜱᴘʟᴀʏꜱ ᴄᴜʀʀᴇɴᴛ ʙᴏᴛ ᴜꜱᴀɢᴇ ꜱᴛᴀᴛɪꜱᴛɪᴄꜱ.
myplan - ᴄʜᴇᴄᴋꜱ ᴛʜᴇ ꜱᴛᴀᴛᴜꜱ ᴏꜰ ᴛʜᴇ ᴜꜱᴇʀ'ꜱ ᴘʀᴇᴍɪᴜᴍ ᴘʟᴀɴ.
list_allcmd - ᴅɪꜱᴘʟᴀʏꜱ ᴀ ʟɪꜱᴛ ᴏꜰ ᴀʟʟ ᴀᴠᴀɪʟᴀʙʟᴇ ᴄᴏᴍᴍᴀɴᴅꜱ.
public_batch - ᴄʀᴇᴀᴛᴇꜱ ᴀ ʙᴀᴛᴄʜ ʟɪɴᴋ ꜰᴏʀ ᴜᴘ ᴛᴏ 50 ꜰɪʟᴇꜱ (ᴘᴜʙʟɪᴄ ᴍᴏᴅᴇ).
publicmode_help - ᴅɪꜱᴘʟᴀʏꜱ ᴛʜᴇ ɢᴜɪᴅᴇ ᴏɴ ʜᴏᴡ ᴛᴏ ᴜꜱᴇ ᴘᴜʙʟɪᴄ ᴍᴏᴅᴇ.
users - [ᴀᴅᴍɪɴ] ᴅɪꜱᴘʟᴀʏꜱ ᴛʜᴇ ᴛᴏᴛᴀʟ ɴᴜᴍʙᴇʀ ᴏꜰ ʀᴇɢɪꜱᴛᴇʀᴇᴅ ᴜꜱᴇʀꜱ.
ban - [ᴀᴅᴍɪɴ] ʀᴇꜱᴛʀɪᴄᴛꜱ ᴀ ꜱᴘᴇᴄɪꜰɪᴇᴅ ᴜꜱᴇʀ ꜰʀᴏᴍ ᴜꜱɪɴɢ ᴛʜᴇ ʙᴏᴛ.
unban - [ᴀᴅᴍɪɴ] ʀᴇᴍᴏᴠᴇꜱ ʀᴇꜱᴛʀɪᴄᴛɪᴏɴꜱ ᴏɴ ᴀ ꜱᴘᴇᴄɪꜰɪᴇᴅ ᴜꜱᴇʀ.
broadcast - [ᴀᴅᴍɪɴ] ꜱᴇɴᴅꜱ ᴀ ᴍᴇꜱꜱᴀɢᴇ ᴛᴏ ᴀʟʟ ʙᴏᴛ ᴜꜱᴇʀꜱ.
pbroadcast - [ᴀᴅᴍɪɴ] ꜱᴇɴᴅꜱ ᴀ ᴍᴇꜱꜱᴀɢᴇ ᴛᴏ ᴀʟʟ ᴜꜱᴇʀꜱ ᴀɴᴅ ᴘɪɴꜱ ɪᴛ.
genlink - [ᴀᴅᴍɪɴ] ɢᴇɴᴇʀᴀᴛᴇꜱ ᴀ ꜱɪɴɢʟᴇ ꜰɪʟᴇ ꜱʜᴀʀᴇᴀʙʟᴇ ʟɪɴᴋ.
batch - [ᴀᴅᴍɪɴ] ɢᴇɴᴇʀᴀᴛᴇꜱ ᴍᴜʟᴛɪᴘʟᴇ ꜰɪʟᴇ ʟɪɴᴋꜱ ꜱɪᴍᴜʟᴛᴀɴᴇᴏᴜꜱʟʏ.
req - [ᴀᴅᴍɪɴ] ᴄʀᴇᴀᴛᴇꜱ ᴀ ʀᴇQᴜᴇꜱᴛ ʟɪɴᴋ ꜰᴏʀ ᴀ ꜱᴘᴇᴄɪꜰɪᴇᴅ ᴄʜᴀɴɴᴇʟ.
add_premium - [ᴀᴅᴍɪɴ] ɢʀᴀɴᴛꜱ ᴘʀᴇᴍɪᴜᴍ ᴍᴇᴍʙᴇʀꜱʜɪᴘ ꜱᴛᴀᴛᴜꜱ ᴛᴏ ᴀ ᴜꜱᴇʀ.
remove_premium - [ᴀᴅᴍɪɴ] ʀᴇᴠᴏᴋᴇꜱ ᴘʀᴇᴍɪᴜᴍ ᴍᴇᴍʙᴇʀꜱʜɪᴘ ꜱᴛᴀᴛᴜꜱ.
list_premiums - [ᴀᴅᴍɪɴ] ʀᴇᴛʀɪᴇᴠᴇꜱ ᴀ ʟɪꜱᴛ ᴏꜰ ᴀʟʟ ᴘʀᴇᴍɪᴜᴍ ᴍᴇᴍʙᴇʀꜱ.
list_ban - [ᴀᴅᴍɪɴ] ʀᴇᴛʀɪᴇᴠᴇꜱ ᴀ ʟɪꜱᴛ ᴏꜰ ᴀʟʟ ʙᴀɴɴᴇᴅ ᴜꜱᴇʀꜱ.
list_users - [ᴀᴅᴍɪɴ] ɢᴇɴᴇʀᴀᴛᴇꜱ ᴀ ᴛᴇxᴛ ꜰɪʟᴇ ᴏꜰ ᴀʟʟ ᴜꜱᴇʀꜱ.
list_admins - [ᴀᴅᴍɪɴ] ᴅɪꜱᴘʟᴀʏꜱ ᴀ ʟɪꜱᴛ ᴏꜰ ʙᴏᴛ ᴀᴅᴍɪɴɪꜱᴛʀᴀᴛᴏʀꜱ.
log - [ᴀᴅᴍɪɴ] ꜱᴇɴᴅꜱ ᴛʜᴇ ꜱʏꜱᴛᴇᴍ ʟᴏɢ ꜰɪʟᴇ.
clear_log - [ᴀᴅᴍɪɴ] ᴄʟᴇᴀʀꜱ ᴛʜᴇ ꜱʏꜱᴛᴇᴍ ʟᴏɢ ꜰɪʟᴇ.
restart - [ᴀᴅᴍɪɴ] ʀᴇꜱᴛᴀʀᴛꜱ ᴛʜᴇ ʙᴏᴛ ꜱᴇʀᴠᴇʀ.
stats - [ᴀᴅᴍɪɴ] ᴅɪꜱᴘʟᴀʏꜱ ᴅᴀᴛᴀʙᴀꜱᴇ ꜱᴛᴀᴛɪꜱᴛɪᴄꜱ.
public_mode - [ᴀᴅᴍɪɴ] ᴛᴏɢɢʟᴇꜱ ᴘᴜʙʟɪᴄ ᴜᴘʟᴏᴀᴅ ᴍᴏᴅᴇ (ᴏɴ/ᴏꜰꜰ).
```

### 2️⃣ User Commands (Public Menu)
*Use this list to provide a clean interface for normal users.*

```text
start - ɪɴɪᴛɪᴀᴛᴇꜱ ᴏʀ ʀᴇꜱᴛᴀʀᴛꜱ ᴛʜᴇ ʙᴏᴛ ꜱᴇʀᴠɪᴄᴇ.
usage - ᴅɪꜱᴘʟᴀʏꜱ ᴄᴜʀʀᴇɴᴛ ʙᴏᴛ ᴜꜱᴀɢᴇ ꜱᴛᴀᴛɪꜱᴛɪᴄꜱ.
myplan - ᴄʜᴇᴄᴋꜱ ᴛʜᴇ ꜱᴛᴀᴛᴜꜱ ᴏꜰ ᴛʜᴇ ᴜꜱᴇʀ'ꜱ ᴘʀᴇᴍɪᴜᴍ ᴘʟᴀɴ.
list_allcmd - ᴅɪꜱᴘʟᴀʏꜱ ᴀ ʟɪꜱᴛ ᴏꜰ ᴀʟʟ ᴀᴠᴀɪʟᴀʙʟᴇ ᴄᴏᴍᴍᴀɴᴅꜱ.
public_batch - ᴄʀᴇᴀᴛᴇꜱ ᴀ ʙᴀᴛᴄʜ ʟɪɴᴋ ꜰᴏʀ ᴜᴘ ᴛᴏ 50 ꜰɪʟᴇꜱ (ᴘᴜʙʟɪᴄ ᴍᴏᴅᴇ).
publicmode_help - ᴅɪꜱᴘʟᴀʏꜱ ᴛʜᴇ ɢᴜɪᴅᴇ ᴏɴ ʜᴏᴡ ᴛᴏ ᴜꜱᴇ ᴘᴜʙʟɪᴄ ᴍᴏᴅᴇ.
```

## 💻 **Configuration (`setup.json`)**

The system relies on a modular setup for robust deployment. Each object in the array defines a **fully isolated bot instance**, allowing you to run multiple bots from one codebase.

```json
[
   {
        "session": "ses",
        "token": "YOUR_BOT_TOKEN",
        "api_id": "YOUR_API_ID",
        "api_hash": "YOUR_API_HASH",
        "workers": 8,
        "db_name": "Cluster0",
        "fsubs": [[-100000008034, false, 0]],
        "db": -10022000033431,
        "auto_del": 0,
        "messages": {
            "START": "Hi {mention}, Welcome to {username}",
            "FSUB": "Join Force-Sub Channels...",
            "ABOUT": "Developer: [𓆩ᗩӄ𓆪](https://t.me/Shadow_Blank)",
            "REPLY": "You Are Not My Master",
            "START_PHOTO": "[https://i.ibb.co/TD8Y4rCq/thumb.jpg](https://i.ibb.co/TD8Y4rCq/thumb.jpg)",
            "FSUB_PHOTO": "[https://i.ibb.co/JRYYZkFy/b1.jpg](https://i.ibb.co/JRYYZkFy/b1.jpg)",
            "Short": "Your link is ready...",
            "SHORT_PHOTO": "[https://i.ibb.co/JRYYZkFy/b1.jpg](https://i.ibb.co/JRYYZkFy/b1.jpg)"
        },
        "admins": [1234567890],
        "disable_btn": true,
        "protect": false,
        "shortner_link": ["[https://shortner.com/api?api=xyz](https://shortner.com/api?api=xyz){}"],
        "token_system": true
  }
]

