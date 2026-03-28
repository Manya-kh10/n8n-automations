# n8n Automation Workflows

A collection of automation workflows built with [n8n](https://n8n.io/) — an open-source workflow automation tool. This repo is a growing library of practical automations I'm building as I learn, ranging from simple data pipelines to locally-run AI agents.

---

## Workflows

| Workflow | Description | Tools Used |
|---|---|---|
| [Form Discount Logger](./form-discount-logger/) | Captures form submissions, applies conditional discount logic for positive feedback, and logs to Google Sheets | n8n, Google Sheets |
| [Email Code Reviewer](./email-code-reviewer/) | Receives code via email, analyzes it using a local LLM, and replies with inline comments + a summary | n8n, Ollama, Phi-3, Gmail |

---

## How to Use

1. Install and run n8n locally or on a server — [n8n docs](https://docs.n8n.io/)
2. Clone this repo
3. In n8n, go to **Settings → Import workflow** and upload the `workflow.json` file from the folder of your choice
4. Set up the required credentials (Google Sheets, Gmail, etc.) in your n8n instance
5. Activate and run

> Each workflow folder has its own README with setup instructions specific to that workflow.

---

## Stack

- **n8n** — workflow automation
- **Ollama** — local LLM inference (no API costs, data stays on your machine)
- **Phi-3** — local language model used for code analysis
- **Google Sheets / Gmail** — for data logging and email handling

---

## About

I'm a 3rd year B.Tech CSE (AI & ML) student learning automation by building real workflows. This repo documents that journey — starting simple and getting progressively more complex.

More workflows coming soon.
