# TikTok Repost Detector 🔁  
**by @gqpgqpg**

An **async TikTok repost monitoring tool** that continuously tracks a target account and **detects new reposted videos in real time**, sending instant alerts to **Telegram** when a new repost appears.

---

## ✨ Features

### 🔍 Repost Monitoring
- Tracks reposted videos from a target TikTok account
- Detects **new reposts only** (no duplicates)
- Builds an initial baseline on startup
- Persistent repost tracking using `seen.json`

### ⚡ Real-Time Detection
- Continuous polling loop
- Fast async requests using `aiohttp`
- Offset-based pagination for full coverage
- Automatic delay handling to reduce detection issues

### 📬 Telegram Alerts
- Sends instant Telegram messages on new reposts
- Includes:
  - Target username
  - Video ID
  - Original author
  - Caption
  - Direct video link
