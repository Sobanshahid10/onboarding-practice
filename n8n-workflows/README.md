# 🔌 Core n8n Foundational Workflows

This module houses three basic n8n workflows designed to build familiarity with fundamental n8n nodes: HTTP Requests, Webhooks, and custom JavaScript execution blocks.

---

## 📂 Included Workflows

### 1. HTTP Request Practice
*File: `workflow-1-http-request.json`*
- **Nodes Covered:** Cron Trigger, HTTP Request node, Set Node.
- **Concepts:** Learn how to fetch data from an external REST API (e.g., JSONPlaceholder or random user APIs), filter properties, and pass them downstream.

### 2. Webhook Trigger Practice
*File: `workflow-2-webhook.json`*
- **Nodes Covered:** Webhook Trigger node, Respond to Webhook node.
- **Concepts:** Learn how to configure webhook triggers, parse path variables and JSON query parameters, and return custom HTML or JSON responses directly to clients.

### 3. JavaScript Execution Block
*File: `workflow-3-code.json`*
- **Nodes Covered:** Code node (JavaScript).
- **Concepts:** Practice writing custom JavaScript logic in n8n (using the `$input` API) to format dates, map array structures, or filter objects that are complex for standard nodes.
