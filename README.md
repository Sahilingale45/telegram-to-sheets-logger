# telegram-to-sheets-logger
A real-time Make.com automation blueprint that listens to Telegram bot updates and automatically logs incoming chat messages as new rows in a Google Sheet.
# Telegram Bot to Google Sheets Data Logger

This repository contains a Make.com (formerly Integromat) scenario blueprint that builds a real-time data collection and logging pipeline between a Telegram Bot and a Google Sheets spreadsheet.

## 🚀 How It Works
1. **Trigger (Telegram Bot - Watch Updates):** Instantly captures user text messages, bot interaction logs, or custom slash commands as soon as they are sent to your bot via webhooks.
2. **Action (Google Sheets - Add a Row):** Extracts essential data points from the incoming payload (e.g., sender name, chat ID, text content, date) and appends them cleanly as a new entry row into a destination spreadsheet.

## 📦 What's Included
* `/blueprints/telegram-to-sheets-logger.json`: The complete exported Make.com scenario blueprint configuration file.

## 🔧 Setup Instructions
1. Open your **Make.com** dashboard.
2. Create a new scenario, click the three dots (`...`) located on the bottom navigation panel, and choose **Import Blueprint**.
3. Upload the `.json` blueprint file from this repository.
4. Establish your connections and parameters:
   * **Telegram Bot Module:** Generate an API Token from Telegram's `@BotFather` and create a connection in Make to activate the live webhook listener.
   * **Google Sheets Module:** Connect your Google Drive account, choose your primary tracking spreadsheet, and select the specific sheet tab.
5. Map the incoming Telegram fields (like `Message Text`, `Sender Username`, and `Date`) directly into your corresponding spreadsheet columns.
6. Save the configuration and flip the main scheduling toggle switch to **ON**.
