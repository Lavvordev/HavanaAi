<div align="center">
  
  <img src="https://postimg.cc/VJb7HMnw/4d440a75" alt="HavanaAi Logo" width="200"/>
  
  # 🤖 HavanaAi WhatsApp Bot
  
  ### *Your Ultimate WhatsApp Assistant | Special for Music*
  
  [![Version](https://img.shields.io/badge/Version-1.00.1-blue.svg)](https://github.com/LavvorStudio/HavanaAi)
  [![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
  [![Node](https://img.shields.io/badge/Node-20%2B-brightgreen.svg)](https://nodejs.org)
  [![Baileys](https://img.shields.io/badge/Baileys-7.0.0--rc.9-orange.svg)](https://github.com/WhiskeySockets/Baileys)
  
</div>

---

## 📌 **About**

**HavanaAi** is an advanced WhatsApp bot with message protection, status automation, and smart triggers. Built with Baileys. Special for music.

---

## ✨ **Features**

### 🎵 Music & Audio
| Command | Description |
|---------|-------------|
| `.ytplay <song>` | Search and download audio from YouTube |
| `.ytmp3 <url>` | Download YouTube audio as MP3 |
| `.ytalbum <name>` | Download entire YouTube album |
| `.ytplaylist <url>` | Download YouTube playlist |
| `.yttrending` | Get trending songs |
| `.ytlyrics <song>` | Get song lyrics |
| `.spotify <song>` | Search and download from Spotify |

### 🎬 Video & Image
| Command | Description |
|---------|-------------|
| `.ytmp4 <url>` | Download YouTube video with quality selection |
| `.ytthumb <url>` | Get YouTube thumbnail |
| `.tiktok <url>` | Download TikTok video |
| `.insta <url>` | Download Instagram video/reel |
| `.fb <url>` | Download Facebook video |
| `.movie <name>` | Search and download movie trailer |

### 🔍 Info & Search
| Command | Description |
|---------|-------------|
| `.yts <query>` | Search YouTube |
| `.tts user <username>` | Get TikTok user info |
| `.tts videos <username>` | Get TikTok user videos |

### 😼 Havana & Ai
| Command | Description |
|---------|-------------|
| `.havana who` | About Havana |
| `.havana motivation` | Get motivational quotes |
| `.havana mindcontrol` | Mind control tips |
| `.havana deepthink` | Deep thinking |
| `.havana overtaking` | Overtaking limits |
| `.havana anxiety` | Anxiety relief |
| `.havana mindset` | Mindset shift |
| `.havana joke` | Get funny jokes |
| `.havana takecontrol` | Take control motivation |

### 🛡️ Message Protection
| Command | Description |
|---------|-------------|
| `.antideletecmd on/off` | Enable/disable Anti-Delete |
| `.antieditcmd on/off` | Enable/disable Anti-Edit |
| `.antitoggle` | View all settings |

### 📱 Status Automation
| Command | Description |
|---------|-------------|
| `.autoread on/off` | Auto-read messages |
| `.autotyping on/off` | Show typing indicator |
| `.autorecording on/off` | Show recording indicator |
| `.autostatus on/off` | Auto-view statuses |

### 🔐 Smart Triggers
| Command | Description |
|---------|-------------|
| `.wavv set emoji 😂` | Set emoji trigger |
| `.wavv set text wow` | Set text trigger |
| `.wavv list` | List all triggers |
| `.wavv stats` | Show statistics |
| `.vv` | Save view-once media (reply to message) |

### ⚙️ System Commands
| Command | Description |
|---------|-------------|
| `.ping` | Check bot latency |
| `.uptime` | Bot uptime |
| `.info` | Bot information |
| `.update` | Check for updates |
| `.mode public/private` | Change bot mode |
| `.setprefix <prefix>` | Change command prefix |
| `.setowner <number>` | Set owner number |
| `.menu` | Show all categories |

---

## 📋 **Prerequisites**

| Requirement | Version |
|-------------|---------|
| Node.js | 20.0 or higher |
| npm | 9.0 or higher |
| WhatsApp Account | Active |

---

## 🚀 **Installation**

### 1. Clone the repository
```bash
git clone https://github.com/LavvorStudio/HavanaAi.git
cd HavanaAi
```

### 2. Install dependencies
```bash
npm install
```

### 3. Create `.env` file
```env
BOT_NAME=HavanaAi
OWNER_NUMBER=923001234567
PREFIX=.
CHANNEL_LINK=https://whatsapp.com/channel/your_channel
SESSION_ID= # optional
```

### 4. Run the bot
```bash
npm start
```

### 5. Scan QR Code
- Open WhatsApp → Settings → Linked Devices → Link a Device
- Scan the QR code shown in terminal

---

## 🎯 **Quick Start Commands**

After bot connects, type:

```
.menu - Show all categories
.havana motivation - Get motivation
.ytmp3 <song> - Download music
```

---

## 📁 **Project Structure**

```
HavanaAi/
├── havana.js           # Main bot file
├── index.js            # Bot loader
├── package.json        # Dependencies
├── .env               # Configuration
├── auth_info/         # Session storage
├── media/             # Downloaded media
│   ├── status/        # Saved statuses
│   └── viewonce/      # Saved view-once media
└── temp/              # Temporary files
```

---

## 🔧 **Advanced Setup Commands**

### Anti-Delete Setup
```bash
.antideletecmd on              # Enable anti-delete
.antideletecmd off             # Disable anti-delete
.antideletecmd loggroup 123@g.us  # Set log group
```

### Anti-Edit Setup
```bash
.antieditcmd on                # Enable anti-edit
.antieditcmd off               # Disable anti-edit
.antieditcmd mode private      # Send to owner only
.antieditcmd mode chat         # Send in same chat
.antieditcmd mode both         # Send to both
```

### ViewOnce Triggers
```bash
.wavv set emoji 😂             # Set emoji trigger
.wavv set text wow             # Set text trigger
.wavv list                     # List triggers
.wavv remove emoji 😂          # Remove trigger
.wavv stats                    # Show statistics
```

---

## 🛡️ **Features Explained**

| Feature | How it works |
|---------|--------------|
| **Anti-Delete** | Saves all messages. When deleted, restores original content |
| **Anti-Edit** | Tracks message edits. Shows original + new text |
| **Status Viewer** | Automatically saves all status updates to owner |
| **ViewOnce Saver** | Saves view-once media. Trigger with emoji/text to resend |
| **AutoRead** | Automatically marks messages as read |
| **AutoTyping** | Shows typing indicator when responding |
| **AutoRecording** | Shows recording indicator when responding |
| **AutoStatus** | Auto-views WhatsApp statuses |

---

## 📝 **Environment Variables**

| Variable | Required | Default | Description |
|----------|----------|---------|-------------|
| `BOT_NAME` | No | HavanaAi | Bot display name |
| `OWNER_NUMBER` | No | Auto-detect | Bot owner number |
| `PREFIX` | No | `.` | Command prefix |
| `CHANNEL_LINK` | No | - | WhatsApp channel link |
| `SESSION_ID` | No | - | Session ID for reuse |

---

## 🤝 **Contributing**

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📜 **License**

Distributed under the MIT License. See `LICENSE` file for more information.

---

## 👨‍💻 **Developer**

| Name | Role |
|------|------|
| **Lavvordev** | Developer |
| **LavvorStudio** | Company |

---

## 🌟 **Show your support**

Give a ⭐️ if this project helped you!

---

## 📞 **Contact**

- **WhatsApp Channel**: [Join Here](https://whatsapp.com/channel/0029Vb7hmuC5fM5eo0fV9c3z)
- **Developer**: [Lavvordev](https://github.com/Lavvordev)

---

<div align="center">
  
  *Made with ❤️ by LavvorStudio*
  
</div>
