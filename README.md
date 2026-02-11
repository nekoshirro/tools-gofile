# Gofile Upload Automation Script

This script automatically uploads a specified file to Gofile and sends detailed status notifications to Telegram.

---

## 🚀 Features
- Uploads any file provided as an argument directly to Gofile.
- Sends a Telegram notification when the upload process begins.
- Sends a separate notification with the Gofile download link and MD5 hash upon completion.
- Nicely formatted notification messages (bold text and newlines) for better readability.
- Lightweight and requires only `curl` as a primary dependency.

---

## ⚙️ Setup Instructions

### 1. Prerequisites
- A Linux-based system (like Ubuntu, Debian, etc.) with `bash`.
- `curl` must be installed (it is included by default on most Linux distributions).

### 2. Configuration
Open the `go-up` script and edit the variables at the top:

```bash
# =========================================================
# CONFIGURATION
# Set your Telegram bot token and chat IDs here.
# =========================================================
TG_BOT_TOKEN="your_bot_token_here"
TG_MAIN_CHAT_ID="your_main_chat_id"      # Receives "start" and "error" notifications
TG_DOWNLOAD_CHAT_ID="your_download_chat_id" # Receives the final download link
