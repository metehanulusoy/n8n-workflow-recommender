# 🤖 n8n Workflow Recommender

[![GitHub Pages](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-blue?style=for-the-badge&logo=github)](https://metehanulusoy.github.io/n8n-workflow-recommender)
[![Workflows](https://img.shields.io/badge/Workflows-2055-green?style=for-the-badge)](https://github.com/metehanulusoy/awesome-n8n-workflows)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](LICENSE)

An AI-powered chatbot that recommends n8n automation workflows based on your needs. Just describe what you want to automate in plain English — the recommender finds the best matching workflows from a library of **2055+ workflows**.

🔗 **Live Demo:** [metehanulusoy.github.io/n8n-workflow-recommender](https://metehanulusoy.github.io/n8n-workflow-recommender)

---

## ✨ Features

- 💬 **Chat Interface** — Natural language input, just describe your automation goal
- 🔍 **Smart Keyword Matching** — Detects services and actions from your message
- 📦 **2055+ Workflows** — Sourced from the [awesome-n8n-workflows](https://github.com/metehanulusoy/awesome-n8n-workflows) collection
- ⬇️ **One-Click Download** — Download any recommended workflow as JSON
- 🐍 **Convert to Python** — Send workflow directly to the [n8n-workflow-to-python](https://github.com/metehanulusoy/n8n-workflow-to-python) converter
- ⚡ **No API Key Needed** — Runs 100% in the browser, no backend required
- 💡 **Suggestion Chips** — Quick-start prompts for common automation scenarios

---

## 🚀 How to Use

1. Visit the [live demo](https://metehanulusoy.github.io/n8n-workflow-recommender)
2. Type what you want to automate (e.g. *"Send Slack alerts when a form is submitted"*)
3. The bot returns the top matching workflows
4. Click **Download JSON** to get the workflow file
5. Import it into your n8n instance — done!

---

## 💡 Example Queries

| You type... | What it finds |
|---|---|
| `send slack notification` | Slack messaging workflows |
| `scrape website data` | HTTP Request + data extraction flows |
| `automate email with gmail` | Gmail automation workflows |
| `connect postgres to google sheets` | Database + spreadsheet sync flows |
| `webhook trigger` | Webhook-based automation workflows |

---

## 🛠️ How It Works

The recommender uses a **keyword scoring algorithm** — no AI API needed:

1. Your message is tokenized into keywords
2. Keywords are matched against a service/action map (Slack, Gmail, HTTP, Cron, etc.)
3. Each workflow in the library is scored based on how many keywords appear in its filename
4. Top 6 highest-scoring workflows are returned as recommendations

```
User Input → Keyword Extraction → Service Detection → Score Workflows → Return Top 6
```

---

## 📁 Project Structure

```
n8n-workflow-recommender/
└── index.html        # Single-file app — chat UI + recommendation engine
```

---

## 🔗 Related Projects

| Project | Description |
|---|---|
| [awesome-n8n-workflows](https://github.com/metehanulusoy/awesome-n8n-workflows) | Searchable library of 2055+ n8n workflows |
| [n8n-workflow-to-python](https://github.com/metehanulusoy/n8n-workflow-to-python) | Convert n8n workflows to Python scripts |

---

## 📄 License

MIT License — free to use, modify, and distribute.

---

> Built by [metehanulusoy](https://github.com/metehanulusoy) • Powered by [n8n](https://n8n.io)
