
# Smart Customer Support Bot

An automated customer support system using n8n, OpenRouter (Llama 3.2), and Google Sheets.

## Included Files
- `customer-support-bot.json`: The n8n workflow export.
- `test.html`: A frontend testing interface.

## Setup Instructions
1. **Import Workflow:** Open n8n, click 'Import from File', and select the `.json` file.
2. **Credentials:** Add your OpenRouter API Key and connect your Google Account via OAuth.
3. **Google Sheet:** Update the Google Sheets node with your own Spreadsheet URL.
4. **Webhook:** Copy your Webhook URL and paste it into the `test.html` fetch function.

## How to Test
Open `test.html` in any browser, type a question, and click "Send". The AI will respond, and the interaction will be logged to Google Sheets.
