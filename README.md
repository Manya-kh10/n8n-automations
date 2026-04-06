# n8n Automation Workflows
A collection of automation workflows built with [n8n](https://n8n.io/) — an open-source workflow automation tool. This repo is a growing library of practical automations I'm building as I learn, ranging from simple data pipelines to AI-powered digest systems.

---

## Workflows

| Workflow | Description | Tools Used |
|---|---|---|
| [Form Discount Logger](./form-discount-logger/) | Captures form submissions, applies conditional discount logic for positive feedback, and logs to Google Sheets | n8n, Google Sheets |
| [Email Code Reviewer](./email-code-reviewer/) | Receives code via email, analyzes it using a local LLM, and replies with inline comments + a summary | n8n, Ollama, Phi-3, Gmail |
| [GitHub Weekly Digest](./github-weekly-digest/) | Runs every Monday, fetches commits from active repos in the last 7 days, generates an AI summary, and sends a formatted email digest | n8n, GitHub API, Groq, Gmail |
| [HN Notion Digest](./hn-notion-digest/) | Runs daily, fetches top 10 Hacker News stories, generates per-story AI summaries, and saves everything to a Notion database | n8n, Hacker News API, Groq, Notion API |

---

## How to Use
1. Install and run n8n locally or on a server — [n8n docs](https://docs.n8n.io/)
2. Clone this repo
3. In n8n, go to **Settings → Import workflow** and upload the `workflow.json` file from the folder of your choice
4. Set up the required credentials (Google Sheets, Gmail, GitHub, Groq, Notion etc.) in your n8n instance
5. Activate and run

> Each workflow folder has its own README with setup instructions specific to that workflow.

---

## Stack
- **n8n** — workflow automation
- **Ollama** — local LLM inference (no API costs, data stays on your machine)
- **Phi-3** — local language model used for code analysis
- **Groq API** — cloud
