# 🤖 Telegram AI Bot - Pucho.ai Assessment

## Overview
An intelligent Telegram bot built with n8n that handles multiple message types and integrates with ClickUp for task management.

## 🚀 Features

### 🎤 Voice Message
- User sends voice message
- Bot converts speech to text using Groq Whisper AI
- AI understands the query and replies with a smart response

### 📝 Text Message
- User sends a text message as a task creation command
- AI extracts task details (name, description, status, priority, assignee)
- Automatically creates a task in ClickUp
- If details are incomplete → replies "Invalid Task Message!!"

### 🖼️ Image / Video
- Bot replies: "Invalid Message type, Please send voice message or text!!"

## 🛠️ Tech Stack
- **n8n** — Workflow automation
- **Groq AI** — LLM (llama-3.3-70b-versatile) + Whisper STT
- **ClickUp API** — Task management
- **Telegram Bot API** — Messaging interface

## 📁 Files
- `bot.json` — n8n workflow export (import this to run the bot)

## ⚙️ Setup Instructions

### 1. Prerequisites
- n8n account (https://app.n8n.cloud)
- Groq API key (https://console.groq.com)
- ClickUp account + API token
- Telegram Bot token (from @BotFather)

### 2. Import Workflow
- Open n8n
- Click `...` → Import from file
- Select `bot.json`

### 3. Add Credentials
- **Telegram** → Add bot token in all Telegram nodes
- **Groq** → Add API key in HTTP Request nodes (Authorization header)
- **ClickUp** → Add API token in Create Task node

### 4. Set Webhook

### 5. Publish & Test!

## 🔄 Flow Diagram


## 👨‍💻 Built By
Rushi Bhatt — Admin & Operations, Dermatouch
AI Automation Assessment for Pucho.ai / Letsenkindle

