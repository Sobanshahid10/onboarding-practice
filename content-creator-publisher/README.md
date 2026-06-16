# AI Content Creator & Publisher

## 📝 Project Description
An automated AI workflow that transforms a simple topic into a fully-formatted social media post. The system generates content via AI, logs the data into a Google Sheets Content Calendar, and sends a notification to a Slack channel.

## 🚀 What it Does
1. **Trigger:** Receives a topic and platform via a Webhook (using the included `test.html`).
2. **Generate:** Uses an AI Agent (Llama 3.2 via OpenRouter) to write the post and suggest hashtags.
3. **Store:** Appends the date, topic, platform, and content into a Google Sheet.
4. **Notify:** Sends a "New Content Created" alert to the #content-alerts Slack channel.

## 🛠 Technologies Used
* **n8n:** Workflow automation platform.
* **OpenRouter (Llama 3.2):** Large Language Model for content generation.
* **Google Sheets API:** For cloud-based data storage.
* **Slack API:** For real-time team notifications.
* **JavaScript/HTML:** For the test control panel.

## 📂 Files Included
* `Content Creator & Publisher.json`: The full n8n workflow for import.
* `test.html`: A custom-built UI to trigger the bot from your browser.
* `README.md`: Project documentation and setup guide.

## ⚙️ Setup Steps
1. **Import Workflow:** Open n8n, click "Import from File," and select the `.json` file.
2. **Add Credentials:** - Connect your **OpenRouter** API key.
   - Connect your **Google Sheets** account via OAuth2.
   - Connect your **Slack** Bot Token.
3. **Update Nodes:** - In the Google Sheets node, paste your specific Spreadsheet URL.
   - In the Slack node, ensure the channel is set to `#content-alerts`.
4. **Test:** Open `test.html` and submit a topic to see the automation in action!

## 💡 Example Topics to Try
- "Benefits of AI in small business"
- "Top 5 travel tips for digital nomads"
- "Why Python is great for automation"
