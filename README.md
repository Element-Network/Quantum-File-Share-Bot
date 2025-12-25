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

## 🧪 **Experience the Flow: Live Demonstration**

Interact with a fully deployed instance to understand the elegant user experience and powerful backend logic.

* 🔗 **Engage Now:** [`@Daisuke_Kambebot`](https://t.me/Daisuke_Kambebot)
* *Validate the force-subscription consent process, test short-lived link generation, and review premium status checks.*

---

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
* **Batch Capabilities:** Users can batch up to 20 files from their own channels if the bot is an admin there.

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
public_batch - ᴄʀᴇᴀᴛᴇꜱ ᴀ ʙᴀᴛᴄʜ ʟɪɴᴋ ꜰᴏʀ ᴜᴘ ᴛᴏ 20 ꜰɪʟᴇꜱ (ᴘᴜʙʟɪᴄ ᴍᴏᴅᴇ).
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
public_batch - ᴄʀᴇᴀᴛᴇꜱ ᴀ ʙᴀᴛᴄʜ ʟɪɴᴋ ꜰᴏʀ ᴜᴘ ᴛᴏ 20 ꜰɪʟᴇꜱ (ᴘᴜʙʟɪᴄ ᴍᴏᴅᴇ).
publicmode_help - ᴅɪꜱᴘʟᴀʏꜱ ᴛʜᴇ ɢᴜɪᴅᴇ ᴏɴ ʜᴏᴡ ᴛᴏ ᴜꜱᴇ ᴘᴜʙʟɪᴄ ᴍᴏᴅᴇ.
```

## 💻 **Configuration and Setup**

The system relies on a modular setup for robust deployment:

### `setup.json` (Multi-Bot Configuration Array)
Each object defines a **fully isolated bot instance**.

```json
/* Example entry defining a single bot's universe */
[
   
   {
        "session": "ses",  // unique session name for this bot
        "token": "YOUR_BOT_TOKEN",
        "api_id": "YOUR_API_ID",
        "api_hash": "YOUR_API_HASH",
        "workers": 8,
        "db_name": "Cluster0",
        "fsubs": [[-100000008034, false, 0], [-1003201992157, true, 5]], // [channel_id, request_enabled, link_expiry_in_minutes]
        "db": -10022000033431,  // logs or updates group
        "auto_del": 0,  // auto delete message time in seconds (0 = disabled)
        "messages": {
            "START": "<blockquote expandable><b>┏━━━━━━━━━━━━━━━━━━━━━┓\n◉ Hi {mention}, I am advance file store bot. \n◉ ID 🪪 : {id} \n◉ Username : {username} \n◉ Powered By :  @Element_Network \n┗━━━━━━━━━━━━━━━━━━━━━┛</b></blockquote>",
            "FSUB": "<blockquote expandable><b>Join Force-Sub Channels To Get All The Episodes Note = Force-Sub link 🖇️ will reset in every 5 minutes so join the chnl within time.</b></blockquote>",
            "ABOUT": "<blockquote expandable><b>┏━━━━━━━━━━━━━━━━━━━━━┓\n╔◉ 🧑🏻‍💻Dᴇᴠᴇʟᴏᴩᴇʀ : [𓆩ᗩӄ𓆪](https://t.me/Shadow_Blank) \n╠◉ 📚Lɪʙʀᴀʀy : [Pʏʀᴏɢʀᴀᴍ](https://github.com/pyrogram) \n╠◉ 📝Lᴀɴɢᴜᴀɢᴇ : [Pʏᴛʜᴏɴ 3](https://www.python.org/) \n╠◉ ✒️Aᴅᴍɪɴ Nᴏᴛᴇ : [Sᴛᴀᴛᴇᴍᴇɴᴛ](https://telegra.ph/STATEMENT-07-31-9) \n╠◉ 👥Sᴜᴘᴘᴏʀᴛ : [Eʟᴇᴍᴇɴᴛꜱ Aᴅᴍɪɴ](https://t.me/Element_Admin_Robot) \n╚◉ 📢 Uᴘᴅᴀᴛᴇ : [Eʟᴇᴍᴇɴᴛ Nᴇᴛᴡᴏʀᴋ ](https://t.me/Element_Network) \n┗━━━━━━━━━━━━━━━━━━━━━┛</b></blockquote>",
            "REPLY": "<blockquote expandable><b>You Are Not My Master</b></blockquote>",
            "START_PHOTO": "https://i.ibb.co/TD8Y4rCq/thumb.jpg",  // image URL or Telegram file ID
            "FSUB_PHOTO": "https://i.ibb.co/JRYYZkFy/b1.jpg",  // image URL or Telegram file ID
            "Short": "<blockquote><b>📊 ʜᴇʏ {mention},\n\n‼️ ⌯ ʏᴏᴜʀ ʟɪɴᴋ ɪꜱ ʀᴇᴀᴅʏ, ᴋɪɴᴅʟʏ ᴄʟɪᴄᴋ ᴏɴ ᴏᴘᴇɴ ʟɪɴᴋ ʙᴜᴛᴛᴏɴ..‼️ \n\n𝗡𝗼𝘁𝗲: ɪꜰ ᴛʜᴇ ᴄᴏᴜɴᴛᴅᴏᴡɴ ɪꜱ ɴᴏᴛ ᴡᴏʀᴋɪɴɢ ᴏᴘᴇɴ ᴛʜᴇ ʟɪɴᴋ ʙʏ ɢᴏᴏɢʟᴇ ᴄʜʀᴏᴍᴇ..</b></blockquote>",
            "SHORT_PHOTO": "https://i.ibb.co/JRYYZkFy/b1.jpg". // image URL or Telegram file ID
        },
        "admins": [0987654321, 12345678909],  // To add multiple admins use [{id 1}, {id 2},{id 3}, so on]
        "disable_btn": true,
        "protect": false,  // To toggle protect mode ON or OFF 📴 
        "shortner_link": ["https://{website 1}/api?api=67cdced1b10hrudd7du{}", "https://{website 2}/api?api=67cdced1b10hrudd7du{}"],  // By this you can multiple shortner
        "token_system": true
  },
  {
        "session": "ses2",  // unique session name for this bot
        "token": "YOUR_BOT_TOKEN",  
        "api_id": "YOUR_API_ID",
        "api_hash": "YOUR_API_HASH",
        "workers": 8,
        "db_name": "Filestoreage01_bot",
        "fsubs": [[-100000008034, false, 0], [-1003201992157, true, 5]], // [channel_id, request_enabled, link_expiry_in_minutes]
        "db": -10022000033431,  // logs or updates group
        "auto_del": 0,  // auto delete message time in seconds (0 = disabled)
        "messages": {
            "START": "<blockquote expandable><b>┏━━━━━━━━━━━━━━━━━━━━━┓\n◉ Hi {mention}, I am advance file store bot. \n◉ ID 🪪 : {id} \n◉ Username : {username} \n◉ Powered By :  @Element_Network \n┗━━━━━━━━━━━━━━━━━━━━━┛</b></blockquote>",
            "FSUB": "<blockquote expandable><b>Join Force-Sub Channels To Get All The Episodes. \n\nNote = Force-Sub link 🖇️ will reset in every 5 minutes so join the chnl within time.</b></blockquote>",
            "ABOUT": "<blockquote expandable><b>┏━━━━━━━━━━━━━━━━━━━━━┓\n╔◉ 🧑🏻‍💻Dᴇᴠᴇʟᴏᴩᴇʀ : [𓆩ᗩӄ𓆪](https://t.me/Shadow_Blank) \n╠◉ 📚Lɪʙʀᴀʀy : [Pʏʀᴏɢʀᴀᴍ](https://github.com/pyrogram) \n╠◉ 📝Lᴀɴɢᴜᴀɢᴇ : [Pʏᴛʜᴏɴ 3](https://www.python.org/) \n╠◉ ✒️Aᴅᴍɪɴ Nᴏᴛᴇ : [Sᴛᴀᴛᴇᴍᴇɴᴛ](https://telegra.ph/STATEMENT-07-31-9) \n╠◉ 👥Sᴜᴘᴘᴏʀᴛ : [Eʟᴇᴍᴇɴᴛꜱ Aᴅᴍɪɴ](https://t.me/Element_Admin_Robot) \n╚◉ 📢 Uᴘᴅᴀᴛᴇ : [Eʟᴇᴍᴇɴᴛ Nᴇᴛᴡᴏʀᴋ ](https://t.me/Element_Network) \n┗━━━━━━━━━━━━━━━━━━━━━┛</b></blockquote>",
            "REPLY": "<blockquote expandable><b>You Are Not My Master</b></blockquote>",
            "START_PHOTO": "https://i.ibb.co/mF88FGhn/b1.jpg",  // image URL or Telegram file ID
            "FSUB_PHOTO": "https://i.ibb.co/vxzpq1KJ/b2.jpg",  // image URL or Telegram file ID
            "Short": "<blockquote><b>📊 ʜᴇʏ {mention},\n\n‼️ ⌯ ʏᴏᴜʀ ʟɪɴᴋ ɪꜱ ʀᴇᴀᴅʏ, ᴋɪɴᴅʟʏ ᴄʟɪᴄᴋ ᴏɴ ᴏᴘᴇɴ ʟɪɴᴋ ʙᴜᴛᴛᴏɴ..‼️ \n\n𝗡𝗼𝘁𝗲: ɪꜰ ᴛʜᴇ ᴄᴏᴜɴᴛᴅᴏᴡɴ ɪꜱ ɴᴏᴛ ᴡᴏʀᴋɪɴɢ ᴏᴘᴇɴ ᴛʜᴇ ʟɪɴᴋ ʙʏ ɢᴏᴏɢʟᴇ ᴄʜʀᴏᴍᴇ..</b></blockquote>",
            "SHORT_PHOTO": "https://i.ibb.co/vxzpq1KJ/b2.jpg". // image URL or Telegram file ID
        },
        "admins": [0987654321, 12345678909],  // To add multiple admins use [{id 1}, {id 2},{id 3}, so on]
        "disable_btn": true,
        "protect": false,  // To toggle protect mode ON or OFF 📴 
        "shortner_link": ["https://{website 1}/api?api=67cdced1b10hrudd7du{}", "https://{website 2}/api?api=67cdced1b10hrudd7du{}"],  // By this you can multiple shortner
        "token_system": true
  }
   
]
```

---

### 🌟 **Dynamic Placeholders**

Customize messages like a pro. These variables are automatically replaced with real-time user/bot data:

| Placeholder | Scope | Purpose |
| :--- | :--- | :--- |
| `{mention}` | `START`, `ABOUT` | **Clickable User Mention** (highest personalization). |
| `{first}`, `{last}` | `START`, `ABOUT` | User's first and last name. |
| `{username}` | `START`, `ABOUT` | User's `@username`. |
| `{id}` | `START`, `ABOUT` | Telegram user ID. |
| `{owner_id}`, `{bot_username}` | `ABOUT` | Key operational identifiers. |

> ⚠️ **Note:** Force Subscribe messages **do not support** placeholders.

### 🚀 **Quick Start Guide**

Follow these three steps to deploy the bot on your server:

1.  **Clone & Setup:** Clone the repository and install dependencies.
    ```bash
    git clone 
    cd FileStoreBot
    pip install -r requirements.txt
    ```
2.  **Configure:** Edit `config.py` (for global settings like `OWNER_ID`) and define your bot instances in the `setup.json` array (Tokens, DB URI, Channels, Admins).
3.  **Launch:** Run the main Python file to start the bot(s).
    ```bash
    python3 main.py
    ```

---

# License

# 🛑 Element-Network Proprietary License (ENPL)

This document is the official license for the source code contained within this repository (the "Software"). **Please read this carefully.**

---

## 📜 1. The Basics: What You CAN Do (Grant of License)

The owner grants you a limited, personal license to the Software:

* **Allowed Use:** You may use and modify the Software.
* **Scope:** This is strictly for your **personal use** or **internal business use only**.
* **Transferability:** This license is **non-exclusive** and **non-transferable**. You cannot give or sell the license to anyone else.

---

## 🚫 2. Strict Prohibitions: What You MUST NOT Do

The following actions are **STRICTLY PROHIBITED** and will result in the immediate termination of your license.

| Prohibited Action | Description |
| :--- | :--- |
| **❌ Redistribution** | You may **not** publish, upload, or make the Software, in whole or in part, available to any third party. |
| **❌ Resale** | You may **not** sell the Software, whether by itself or integrated into another product, without a separate, written Resale Agreement from the owner. |
| **❌ Unauthorized Sharing** | You may **not** share the source code or any works derived from it with anyone outside of your immediate licensed environment. |
| **❌ Reverse Engineering** | You may **not** decompile, reverse engineer, or attempt to extract the source code from any compiled versions of the Software. |

---

## 📞 3. Questions, Support, and Commercial Use

If you need to discuss purchasing, custom services, support, or require explicit permission to perform any restricted action above, please contact the owner directly:

* **Telegram:** [`៚𓄂ᗩӄ‌᭄`](https://t.me/Shadow_Blank)

---

## 🛡️ 4. Ownership and Intellectual Property

You acknowledge that all rights, title, and interest in the Software, including all copyrights and intellectual property, belong **exclusively to the original owner.** This document grants you only the right to use the Software as specified above.

## 💀 5. Termination

* **Effective Date:** This license is active from the moment you acquire the Software.
* **Immediate Termination:** If you fail to comply with any term or restriction in this license, the license is **immediately terminated** without notice.
* **Upon Termination:** You must stop all use of the Software immediately and destroy all copies of the Software and its source code.
