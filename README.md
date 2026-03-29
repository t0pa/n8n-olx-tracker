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

   **Google Sheets API Setup:**
   - Go to [Google Cloud Console](https://console.cloud.google.com/).
   - Create a new project (or select an existing one).
   - Enable the "Google Sheets API" for your project.
   - Go to "APIs & Services" > "Credentials".
   - Click "Create Credentials" > "Service account".
   - Download the JSON key file.
   - Share your target Google Sheet with the service account email (from the JSON file).

   **Telegram Bot Setup:**
   - Open Telegram and search for "BotFather".
   - Start a chat and use /newbot to create a bot.
   - Follow the prompts to name your bot and get the API token.
   - Save the API token for your code.
   - Add your bot to the desired chat/group and get the chat ID.

4. **Activate the workflow** in n8n.

   -You could add a scheduler to automate everything. 

<img width="1063" height="371" alt="image" src="https://github.com/user-attachments/assets/f6fa17c7-3abc-4528-8362-160ed3ca44b6" />



