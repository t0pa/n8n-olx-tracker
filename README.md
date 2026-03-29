# n8n OLX Moto Workflow

This repository contains an n8n workflow for monitoring new motorcycle listings on OLX and sending notifications to Telegram and Google Sheets.

## Features

- Scheduled HTTP requests to OLX API for new motorcycle listings
- Compares new data with existing Google Sheets entries
- Sends Telegram notifications for new listings
- Appends or updates Google Sheets with new data

## Setup

1. **Import the sanitized workflow**: Use `n8n-olx-moto.sanitized.json` in your n8n instance.
2. **Configure credentials**:
   - Replace all placeholder values (e.g., `YOUR_GOOGLE_SHEET_URL`, `YOUR_TELEGRAM_CHAT_ID`, `YOUR_CREDENTIAL_ID`, etc.) with your actual credentials and URLs in n8n.
3. **Set up Google Sheets and Telegram**:
   - Ensure you have a Google Sheet ready and a Telegram bot/chat for notifications.
4. **Activate the workflow** in n8n.

## Security

- **No secrets or private data are included** in the sanitized workflow file.
- Always keep your credentials and sensitive data out of public repositories.

## License

MIT
