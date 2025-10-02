# Social Media & News Monitoring System (n8n)

## 📌 Overview
This project is an **automated monitoring workflow** built with [n8n](https://n8n.io/).  
It collects news articles mentioning selected keywords (e.g., *AI, Microsoft, scam, fraud, excellent, amazing*), classifies their sentiment (positive, negative, neutral), and routes the results to different channels for tracking and alerts.

## ⚙️ Features
- ⏱️ Runs every **15 minutes** via a schedule trigger  
- 🌐 Fetches real-time news articles using **Serper.dev (Google News API)**  
- 🧠 Classifies content into **positive, negative, or neutral** based on keywords  
- 📊 Logs all results to **Google Sheets** for record keeping  
- 📲 Sends **negative alerts to Telegram** for immediate action  
- 📂 Stores **positive articles in Airtable** for insights and reporting  

## 📂 Files
- `workflow.json` → Exported n8n workflow definition  
- `screenshot.png` → Visual representation of the workflow  

## 🛠️ Tools & Services Used
- **n8n** → Workflow automation  
- **Serper.dev** → Google News API  
- **Google Sheets** → Logging of all articles  
- **Telegram Bot API** → Instant negative sentiment alerts  
- **Airtable** → Archiving of positive sentiment articles  

## 🚀 How It Works
1. **Trigger** → A schedule runs every 15 minutes.  
2. **Data Collection** → Fetches latest news from Google News via Serper.dev.  
3. **Processing** → A custom code node classifies each article by sentiment.  
4. **Logging** → All articles (title, snippet, link, sentiment, date) are appended to Google Sheets.  
5. **Routing** →  
   - Negative → Sent to Telegram as an alert.  
   - Positive → Stored in Airtable for analysis.  
   - Neutral → Logged only in Google Sheets.  

## 📸 Workflow Example
*(insert screenshot.png here once available)*  

---

✅ This workflow can be adapted to monitor any topic or brand across online news sources, helping teams quickly identify risks and opportunities.
