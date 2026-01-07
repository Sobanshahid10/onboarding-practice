# n8n Learning Workflows

This directory contains workflows created as part of hands-on learning and experimentation with **n8n automation**.  
The goal of these workflows was to understand core n8n concepts such as triggers, API integration, webhooks, data handling, and custom logic.

---

## Workflow 1: GitHub API Integration

- Triggered manually using the **Manual Trigger** node
- Uses the **HTTP Request** node to call the GitHub public API
- Executes the workflow on demand and retrieves API response data
- Helped build understanding of:
  - API requests in n8n
  - Handling external data sources
  - Manual execution and workflow testing

---

## Workflow 2: Webhook-Based Data Response

- Uses a **Webhook** node to trigger the workflow via a URL
- Accepts incoming HTTP requests
- Uses a **Set** node to define and structure custom data (e.g., name and status)
- Returns the processed data using **Respond to Webhook**
- Helped build understanding of:
  - Webhook triggers
  - Request–response workflows
  - Exposing workflows as lightweight APIs

---

## Workflow 3: Custom Logic with Code Node

- Triggered manually using the **Manual Trigger** node
- Uses the **Code** node to return a custom JSON response
- Demonstrates basic scripting inside n8n workflows
- Helped build understanding of:
  - Using JavaScript logic in n8n
  - Structuring JSON output
  - Extending workflows with custom code

