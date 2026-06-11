# 🤖 AI Customer Support Bot (n8n + OpenRouter)

This module implements a smart customer support agent using n8n and OpenRouter (AI endpoint). It accepts user questions, utilizes an AI model to answer and categorize the request, and logs the response.

---

## 📋 Features
- **Webhook Trigger:** Receives real-time customer questions via HTTP POST.
- **AI Agent Integration:** Connects to OpenRouter (such as OpenAI GPT or Anthropic Claude) to generate context-aware, helpful replies.
- **HTML Testing Client:** Includes a lightweight frontend (`test.html`) to send requests and display the AI-generated responses.

---

## 📂 Included Files
- `customer-support-bot.json` — The exported n8n workflow configuration.
- `test.html` — A static HTML UI to interact with the webhook.
- `README.md` — Detailed documentation (this file).

---

## 🛠️ How to Use

### 1. Setup the n8n Workflow
1. Open your n8n canvas.
2. Copy the contents of `customer-support-bot.json` and paste (`Cmd+V` / `Ctrl+V`) into n8n.
3. Configure the **OpenRouter API Key** in the chat model node.
4. Activate the workflow and copy the **Production Webhook URL** or **Test Webhook URL**.

### 2. Configure the HTML Client
1. Open `test.html` in your editor.
2. Locate the javascript fetch call and replace the placeholder webhook URL with your actual n8n Webhook URL.
3. Open `test.html` in a web browser, type a support question (e.g., *"How do I reset my password?"*), and hit **Send**.
