
# AI Inventory Management System for Grocery Stores 🛒⚡

An intelligent no-code solution built with **n8n** that automates stock tracking, generates real-time alerts, and updates inventory via AI-powered chat. Perfect for small businesses looking to streamline operations.

![Workflow Demo](screenshots/demo.gif) *(Replace with your screenshot)*

## 🔥 Key Features
- **AI Chat Assistant**: Natural language interface for inventory queries/updates
- **Real-time Sync**: Auto-updates Google Sheets inventory on changes
- **Smart Alerts**: Detects low stock levels automatically
- **Demand Forecasting**: Powered by Mistral AI via OpenRouter

## 🛠️ Technical Stack
- **Core Platform**: [n8n](https://n8n.io/) (v1.1+)
- **AI Model**: `mistralai/mistral-small-3.1-24b-instruct` (OpenRouter)
- **Data Storage**: Google Sheets (Live sync)
- **Memory**: Conversation history tracking

## 🚀 Quick Setup
1. **Import Workflow**  
   - Download `AI_Inventory_Management_System.json`
   - In n8n: *Workflows > "+" > Import*

2. **Configure Credentials**  
   - Connect your [Google Sheets API](https://console.cloud.google.com/)
   - Add [OpenRouter API key](https://openrouter.ai/keys)

3. **Customize Nodes**:
   ```json
   // Example: Change inventory sheet ID
   "documentId": "YOUR_NEW_SHEET_ID"
