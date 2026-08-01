<div align="center">

# ⚡ Gourmet Bistro Multi-Agent AI Customer Service & Ordering System

**Category:** `AI Chatbots & Conversational Commerce`  
*Multi-agent LangChain structure for restaurant customer service, RAG vector search, order creation, and kitchen dispatch.*

![n8n](https://img.shields.io/badge/n8n-informational?style=flat-square) ![LangChain Multi-Agent](https://img.shields.io/badge/LangChain_Multi-Agent-informational?style=flat-square) ![Qdrant Vector DB](https://img.shields.io/badge/Qdrant_Vector_DB-informational?style=flat-square) ![Google Sheets](https://img.shields.io/badge/Google_Sheets-informational?style=flat-square) ![Supabase PostgreSQL](https://img.shields.io/badge/Supabase_PostgreSQL-informational?style=flat-square) ![Telegram Bot API](https://img.shields.io/badge/Telegram_Bot_API-informational?style=flat-square)
[![n8n Compatible](https://img.shields.io/badge/n8n-Workflow-FF6D5A?style=flat-square&logo=n8n&logoColor=white)](https://n8n.io)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=flat-square)](LICENSE)

[Main Portfolio Hub](https://github.com/Sohila-Khaled-Abbas/n8n-production-queue-setup) · [How to Import](#-how-to-import-and-run) · [Workflow Architecture](#-workflow-architecture)

</div>

---

## 💡 Business Case & Value

Enforces strict business rules (phone validation, delivery checks, 5-minute cancellation grace period) while reducing front-of-house customer service load by up to 80%.

---

## 🛠️ Tech Stack & Integrations

- **Workflow Orchestrator:** n8n Automation Engine
- **Integrations:** n8n, LangChain Multi-Agent, Qdrant Vector DB, Google Sheets, Supabase PostgreSQL, Telegram Bot API
- **Total Workflow Nodes:** `32`
- **Active Node Types:** `telegramTrigger`, `set`, `lmChatOllama`, `switch`, `embeddingsOllama`, `memoryPostgresChat`, `vectorStoreSupabase`, `googleSheets`, `code`, `if`, `telegram`, `agent`, `supabase`, `telegramTool`, `timeSaved`, `chainLlm`, `informationExtractor`
- **Triggers:** `Telegram Trigger`

---

## 📐 Workflow Architecture & Nodes

This repository contains the production-grade n8n workflow exported as standard JSON (`workflow.json`). 

### Core Components
1. **Trigger Layer:** Executes automatically based on incoming events, webhooks, or scheduled crons.
2. **AI & Processing Layer:** Processes natural language or payload data, enforcing validation rules and error retries.
3. **Storage & Notification Layer:** Persists state to database systems (PostgreSQL, MSSQL, Google Sheets) and alerts relevant channels (Telegram, Email, Notion).

---

## 🚀 How to Import and Run

To import this workflow into your n8n instance:

1. **Download Workflow JSON:**
   Download the [`workflow.json`](workflow.json) file from this repository.

2. **Import into n8n:**
   - Open your n8n Editor UI.
   - Click on the **Workflow menu** (top right) -> **Import from File...** (or copy raw JSON content and paste directly into canvas with `Ctrl + V` / `Cmd + V`).

3. **Configure Credentials:**
   - Set up required API credentials in n8n for the respective integrations (n8n, LangChain Multi-Agent, Qdrant Vector DB).

4. **Activate:**
   - Toggle the workflow switch to **Active** and test execution.

---

## 🔗 Related Portfolio Workflows

This workflow is part of the **Production n8n Workflow Portfolio**. Explore more production-grade workflows in the primary repository:
👉 **[https://github.com/Sohila-Khaled-Abbas/n8n-production-queue-setup](https://github.com/Sohila-Khaled-Abbas/n8n-production-queue-setup)**

---

## 📄 License
This workflow is open-source and released under the [MIT License](LICENSE).
