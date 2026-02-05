# MEMORY.md

> This file contains long-term memories, decisions, and important context.

## User Preferences
- **Name:** PuJie (inferred from WeCom username)
- **Timezone:** Asia/Shanghai (UTC+8)
- **Role:** 小红书创作者 / AI 运营者

## Projects & Tasks

### 📰 AI 情报局 (AI News Board)
- **Website:** http://129.226.95.57:3333
- **Local Path:** `news_board/index.html`
- **Function:** Auto-fetches top 3 AI news from Hacker News/Hugging Face every 8 hours.
- **Style:** "Little Red Book" (XiaoHongShu) style copy + 3 images per news item.
- **Features:** 
  - Bento grid layout for images.
  - "Copy Copywriting" button.
  - "Download Images" button (batch downloads 3 images).
- **Automation:** Cron job `auto-news-updater` runs every 8 hours.
- **Service:** Systemd service `newsboard` ensures high availability.

### 📝 Content Strategy
- **Structure:**
  1. 💥 Explosive Title (Emoji included)
  2. 🤔 What happened (Plain language)
  3. 🎯 Who needs it / Use cases
  4. 💡 Deep insight / Future outlook (Personal touch)
  5. 📢 Call to Action (Group invite)
  6. Tags (#AI ...)

## System Configuration
- **GitHub Repo:** https://github.com/PuJes/my-clawdbot
- **Cron Jobs:** 
  - `auto-news-updater` (Every 8 hours): Updates news board content using a sub-agent.
