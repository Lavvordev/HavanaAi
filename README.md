<div align="center">
  
  <img src="https://i.postimg.cc/FHT2zVKY/xbotlogo.png" alt="HavanaAi Logo" width="250"/>
  
  # 🤖 HavanaAi WhatsApp Bot
  
  ### *Your Ultimate WhatsApp Assistant | Special for Music*
  
  [![Version](https://img.shields.io/badge/Version-1.00.1-blue.svg)](https://github.com/LavvorStudio/HavanaAi)
  [![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
  [![Node](https://img.shields.io/badge/Node-20%2B-brightgreen.svg)](https://nodejs.org)
  [![Baileys](https://img.shields.io/badge/Baileys-7.0.0--rc.9-orange.svg)](https://github.com/WhiskeySockets/Baileys)
  [![Railway](https://img.shields.io/badge/Deploy-Railway-purple.svg)](https://railway.app)
  [![Heroku](https://img.shields.io/badge/Deploy-Heroku-blueviolet.svg)](https://heroku.com)
  [![Render](https://img.shields.io/badge/Deploy-Render-black.svg)](https://render.com)
  [![VPS](https://img.shields.io/badge/Deploy-VPS-red.svg)](https://www.digitalocean.com)
  
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

## 🚀 **Local Installation**

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

## 🚀 **Deployment Guides**

### 📦 **1. Deploy on Railway (Recommended - Easy & Free)**

Railway is a modern deployment platform that offers a free tier with 500 hours/month.

**Step 1:** Create Railway Account
- Go to [railway.app](https://railway.app)
- Sign up using GitHub account

**Step 2:** Deploy from GitHub
- Click "New Project" → "Deploy from GitHub repo"
- Select your `HavanaAi` repository
- Railway will auto-detect Node.js

**Step 3:** Add Environment Variables
- Go to your project dashboard
- Click "Variables" tab
- Add these variables:

| Variable | Value |
|----------|-------|
| `BOT_NAME` | HavanaAi |
| `OWNER_NUMBER` | Your WhatsApp number |
| `PREFIX` | . |
| `CHANNEL_LINK` | Your channel link |

**Step 4:** Deploy
- Railway auto-deploys on every git push
- Click "Deploy" if not auto-deployed

**Step 5:** Get QR Code
- Go to "Deployments" tab
- Click "View Logs"
- Look for QR code in logs
- Scan with WhatsApp

**Step 6:** Keep Bot Alive
- Railway keeps bot running 24/7
- No additional config needed

---

### 📦 **2. Deploy on Heroku**

Heroku is a popular cloud platform (requires paid tier for 24/7).

**Step 1:** Create Heroku Account
- Go to [heroku.com](https://heroku.com)
- Sign up and verify email

**Step 2:** Install Heroku CLI
```bash
npm install -g heroku
heroku login
```

**Step 3:** Create Heroku App
```bash
heroku create havanaai-bot
```

**Step 4:** Add `Procfile`
Create file named `Procfile`:
```text
worker: node havana.js
```

**Step 5:** Set Environment Variables
```bash
heroku config:set BOT_NAME=HavanaAi
heroku config:set OWNER_NUMBER=923001234567
heroku config:set PREFIX=.
heroku config:set CHANNEL_LINK=https://whatsapp.com/channel/...
```

**Step 6:** Deploy
```bash
git push heroku main
```

**Step 7:** Scale Worker
```bash
heroku ps:scale worker=1
```

**Step 8:** View Logs
```bash
heroku logs --tail
```

**Note:** Heroku free tier is discontinued. Use paid tier ($5/month) or switch to Railway.

---

### 📦 **3. Deploy on Render (Free Tier Available)**

Render offers a free tier with 750 hours/month.

**Step 1:** Create Render Account
- Go to [render.com](https://render.com)
- Sign up with GitHub

**Step 2:** Create Web Service
- Click "New +" → "Web Service"
- Connect GitHub repository

**Step 3:** Configure Service
| Field | Value |
|-------|-------|
| Name | havanaai-bot |
| Environment | Node |
| Build Command | `npm install` |
| Start Command | `node havana.js` |
| Instance Type | Free |

**Step 4:** Add Environment Variables
Add the same variables as Railway

**Step 5:** Deploy
- Click "Create Web Service"
- Wait for deployment

**Step 6:** View Logs
- Go to "Logs" tab
- Look for QR code
- Scan with WhatsApp

**Note:** Free tier spins down after 15 minutes of inactivity. Upgrade to paid for 24/7.

---

### 📦 **4. Deploy on Koyeb (Free Alternative)**

Koyeb offers a generous free tier.

**Step 1:** Create Koyeb Account
- Go to [koyeb.com](https://koyeb.com)
- Sign up with GitHub

**Step 2:** Create App
- Click "Create App"
- Select GitHub repository

**Step 3:** Configure
| Field | Value |
|-------|-------|
| Name | havanaai |
| Source | GitHub |
| Build Command | `npm install` |
| Run Command | `node havana.js` |

**Step 4:** Add Secrets
Add all environment variables in "Secrets" section

**Step 5:** Deploy
- Click "Deploy"
- Check logs for QR code

---

### 📦 **5. Deploy on VPS (Ubuntu/Debian)**

Best for 24/7 reliability and full control.

**Step 1:** Get a VPS
- [DigitalOcean](https://digitalocean.com) - $4/month
- [Vultr](https://vultr.com) - $2.50/month
- [Linode](https://linode.com) - $5/month

**Step 2:** Connect to VPS
```bash
ssh root@your-vps-ip
```

**Step 3:** Update System
```bash
sudo apt update && sudo apt upgrade -y
```

**Step 4:** Install Node.js 20+
```bash
curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash -
sudo apt install -y nodejs
node --version
```

**Step 5:** Install PM2 (Process Manager)
```bash
sudo npm install -g pm2
```

**Step 6:** Clone Repository
```bash
git clone https://github.com/LavvorStudio/HavanaAi.git
cd HavanaAi
```

**Step 7:** Install Dependencies
```bash
npm install
```

**Step 8:** Create `.env` file
```bash
nano .env
```

Add:
```env
BOT_NAME=HavanaAi
OWNER_NUMBER=923001234567
PREFIX=.
CHANNEL_LINK=https://whatsapp.com/channel/...
SESSION_ID=
```

**Step 9:** Start with PM2
```bash
pm2 start havana.js --name "HavanaAi"
pm2 save
pm2 startup
```

**Step 10:** PM2 Commands
| Command | Description |
|---------|-------------|
| `pm2 status` | Check bot status |
| `pm2 logs HavanaAi` | View logs (get QR) |
| `pm2 restart HavanaAi` | Restart bot |
| `pm2 stop HavanaAi` | Stop bot |
| `pm2 delete HavanaAi` | Delete bot |

**Step 11:** Install UFW Firewall (Optional)
```bash
sudo ufw allow 22
sudo ufw allow 80
sudo ufw enable
```

---

### 📦 **6. Deploy on Cyclic.sh (Free & Easy)**

Cyclic offers free deployment with no downtime.

**Step 1:** Create Cyclic Account
- Go to [cyclic.sh](https://cyclic.sh)
- Sign up with GitHub

**Step 2:** Link Repository
- Click "Link Your Own"
- Select HavanaAi repository

**Step 3:** Configure
| Field | Value |
|-------|-------|
| Build Command | `npm install` |
| Start Command | `node havana.js` |

**Step 4:** Add Environment Variables
Add all required variables

**Step 5:** Deploy
- Click "Deploy"
- Check logs for QR code

---

### 📦 **7. Deploy on Replit (Free & Simple)**

**Step 1:** Create Replit Account
- Go to [replit.com](https://replit.com)
- Sign up

**Step 2:** Import Repository
- Click "Create Repl" → "Import from GitHub"
- Paste repository URL

**Step 3:** Configure
- Replit auto-installs dependencies
- Add `.env` file with variables

**Step 4:** Run
- Click "Run"
- QR code appears in console

**Note:** Replit free tier has limited uptime. Use UptimeRobot to keep alive.

---

## 📁 **Project Structure**

```
HavanaAi/
├── havana.js           # Main bot file
├── index.js            # Bot loader
├── package.json        # Dependencies
├── .env               # Configuration
├── Procfile           # Heroku process file
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

## 🚨 **Troubleshooting**

| Problem | Solution |
|---------|----------|
| Bot not responding | Check if bot is running: `pm2 status` |
| QR code not showing | Check logs: `pm2 logs HavanaAi` |
| Session expired | Delete `auth_info` folder and restart |
| Bad MAC error | Delete `auth_info` folder, restart, scan new QR |
| Heroku worker not starting | Run `heroku ps:scale worker=1` |
| Railway deployment failed | Check logs in Railway dashboard |
| VPS connection refused | Check firewall: `sudo ufw status` |

---

## 📊 **Deployment Comparison**

| Platform | Free Tier | 24/7 Uptime | Ease of Use | Recommended |
|----------|-----------|-------------|-------------|-------------|
| **Railway** | 500 hrs/month | ✅ | ⭐⭐⭐⭐⭐ | ✅ Best |
| **Render** | 750 hrs/month | ❌ (spins down) | ⭐⭐⭐⭐ | ✅ Good |
| **Heroku** | No (paid only) | ✅ | ⭐⭐⭐⭐ | ⭐ Paid |
| **Koyeb** | ✅ Yes | ✅ | ⭐⭐⭐ | ✅ Good |
| **VPS** | No ($4+/month) | ✅ | ⭐⭐ | ✅ Best for 24/7 |
| **Cyclic** | ✅ Yes | ✅ | ⭐⭐⭐⭐ | ✅ Good |
| **Replit** | ✅ Yes | ❌ (needs ping) | ⭐⭐⭐⭐⭐ | ⭐ Simple |

---

<div align="center">
  
  *Made with ❤️ by LavvorStudio*
  
</div>
