# 📊 Customer Support Bot with Google Sheets Logging

An advanced customer service automation workflow that uses n8n, AI via OpenRouter, and Google Sheets. It receives support queries, queries AI to produce a reply, and logs the customer interaction details directly to a Google Sheets database.

---

## 📋 Features
- **Spreadsheet Logging:** Automatically creates columns for Timestamp, Customer Email, Inquiry Text, AI Reply, and Category.
- **AI Processing Node:** Classifies the issue and drafts a professional response.
- **HTML Sandbox:** Includes a testing interface (`test.html`) to mock customer requests.

---

## 📂 Included Files
- `Customer Support Bot using sheets.json` — The exported n8n workflow.
- `test.html` — HTML page containing input fields (email, message) linked to the webhook.
- `README.md` — Detailed documentation (this file).

---

## 🛠️ Configuration & Setup

### 1. Setup Google Sheets
1. Create a Google Sheet named `Customer Support Logs`.
2. Add the following headers to row 1:
   `Timestamp`, `Email`, `Inquiry`, `AI_Reply`, `Category`
3. Share access to your Google Sheet with your n8n Google Service Account or authenticate via OAuth2.

### 2. Import and Run the Workflow
1. Import `Customer Support Bot using sheets.json` into n8n.
2. Link the **Google Sheets Node** to your Google Spreadsheet ID.
3. Configure your **OpenRouter Credentials**.
4. Activate the webhook and replace the URL in `test.html`.
