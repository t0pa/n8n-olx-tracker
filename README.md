# n8n-olx-tracker
Moto Scraper (n8n Workflow)

Personal project -  n8n workflow that monitors **OLX.ba** for motorcycles. It logs data to Google Sheets and sends real-time alerts via Telegram.

## ✨ Features
- **Smart Tracking**: Detects new listings and removes sold/deleted items.
- **Auto-Sync**: Syncs price, title, and URL to Google Sheets.
- **Telegram Alerts**: Immediate notifications for new finds.
- **Scheduled**: Runs automatically every 12 hours.

## 🚀 Setup
1. **Import**: Load `n8n-olx-scraper.json` into n8n.
2. **Credentials**: Connect your Telegram Bot and Google Sheets account.
3. **Configure**: Replace placeholders (`YOUR_URL`, `YOUR_CHAT_ID`, If needded also `YOUR_WEBHOOK_ID` ) with your actual data.

## 📋 Sheet Format
Required headers: `id`, `title`, `price`, `url`.


NOTE: If you don't want to host, you can use the webhook and make it run everytime you do a certain activity on your machine using Task Scheduler. 


---
*For personal use only. Use responsibly.*
