# Embedded-chatbot-with-GymFAQ

An **embedded chat interface** that connects to an n8n webhook workflow, designed for a Gym FAQ assistant. Users can chat directly on your website, messages are sent to your n8n workflow for processing, and replies are returned seamlessly in the chat widget.

---

## 🚀 Features

- Fully responsive chat widget that can be embedded on any website  
- Sends user messages to a configured n8n webhook  
- Supports session tracking via `sessionId` for multi-turn conversations  
- Expects structured JSON response from the workflow (e.g., `{ "output": "…" }`)  
- Friendly fallback when no valid reply is received  
- Easily customizable styling and behavior to match your brand

---

## 📦 What’s Included

| File | Description |
|------|-------------|
| `index.html` | The chat widget HTML + CSS + JavaScript ready to embed |
| `README.md`     | This documentation file |
| `assets/`       | Folder for optional images/icons used in widget |
| `workflow/`     | (Optional) n8n workflow export JSON for the Gym FAQ agent |

---

## 🛠 Setup & Installation

1. Copy the `index.html` (or widget HTML) file into your website project (e.g., footer or chat page).  
2. In the widget code, edit the `webhookUrl` variable to your n8n webhook endpoint:
   ```js
   const webhookUrl = 'https://YOUR_N8N_DOMAIN/webhook/YOUR_WEBHOOK_ID';
