# n8n workflow templates

Ten free, tested [n8n](https://n8n.io) workflows you can import in a minute. Each one has a setup note on the canvas, uses only standard n8n nodes and contains no credentials.

Built and imported on n8n 2.35. Templates with their own logic (filters, code and branches) were also test-run with sample data.

| Template | What it does | Apps | File | Guide |
| --- | --- | --- | --- | --- |
| Website form to Google Sheets and Slack | Sends contact form leads to a sheet and a Slack channel, with email validation and a reply to the form. | Webhook, Google Sheets, Slack | [JSON](website-form-to-google-sheets-and-slack.json) | [Setup guide](https://serverserv.com/n8n-template-website-form-to-google-sheets-and-slack.html) |
| AI reply drafts for Gmail | Writes a reply draft for every new email in the same thread. Never sends on its own. | Gmail, OpenAI | [JSON](ai-email-reply-drafts-gmail.json) | [Setup guide](https://serverserv.com/n8n-template-ai-email-reply-drafts-gmail.html) |
| Private Telegram AI assistant | Telegram bot with conversation memory, locked to the user IDs you allow. | Telegram, OpenAI | [JSON](telegram-ai-assistant-bot.json) | [Setup guide](https://serverserv.com/n8n-template-telegram-ai-assistant-bot.html) |
| AI lead scoring with Slack alerts | Scores each lead 1 to 10 against your ideal customer, logs all of them and alerts Slack on hot ones. | Webhook, OpenAI, Google Sheets, Slack | [JSON](ai-lead-scoring-slack.json) | [Setup guide](https://serverserv.com/n8n-template-ai-lead-scoring-slack.html) |
| Website uptime monitor | Checks your URLs every 5 minutes and emails you when one is down or too slow. | HTTP Request, SMTP | [JSON](website-uptime-monitor-email-alerts.json) | [Setup guide](https://serverserv.com/n8n-template-website-uptime-monitor-email-alerts.html) |
| Error alerts on Telegram | An error workflow that messages you when any workflow fails, with a link to the execution. | Error Trigger, Telegram | [JSON](n8n-error-alerts-telegram.json) | [Setup guide](https://serverserv.com/n8n-template-n8n-error-alerts-telegram.html) |
| Back up n8n workflows to GitHub | Saves every workflow to a private GitHub repo each night, creating or updating files. | n8n API, GitHub | [JSON](n8n-workflow-backup-to-github.json) | [Setup guide](https://serverserv.com/n8n-template-n8n-workflow-backup-to-github.html) |
| Daily AI digest from RSS | Emails you a short AI briefing of the last 24 hours from an RSS feed. | RSS, OpenAI, SMTP | [JSON](rss-news-ai-daily-digest.json) | [Setup guide](https://serverserv.com/n8n-template-rss-news-ai-daily-digest.html) |
| Daily calendar agenda on Telegram | Sends today's Google Calendar events to Telegram on weekday mornings. | Google Calendar, Telegram | [JSON](google-calendar-daily-agenda-telegram.json) | [Setup guide](https://serverserv.com/n8n-template-google-calendar-daily-agenda-telegram.html) |
| Stripe payments to Google Sheets | Logs every successful Stripe charge to a sheet and announces it in Slack. | Stripe, Google Sheets, Slack | [JSON](stripe-payments-to-google-sheets.json) | [Setup guide](https://serverserv.com/n8n-template-stripe-payments-to-google-sheets.html) |

## How to import

1. Open the JSON file and copy it, or download it.
2. In n8n, create a new workflow and paste the JSON onto the canvas, or use the menu and choose **Import from file**.
3. Open each node with a warning and connect your own credentials. The sticky note on the canvas lists what to set.
4. Run it once by hand, check the output, then activate it.

## Security

Read any workflow before you run it, including these. Templates that take input from strangers (a form, an email, a chat message) validate that input and keep the AI model away from actions it should not take. Each guide has a short security section with anything else to lock down, such as turning on header auth for public webhooks.

## Where to run them

Webhook and schedule workflows need n8n online all the time and reachable over HTTPS. You can run n8n yourself with Docker, use n8n Cloud, or use [serverserv n8n Hosting](https://serverserv.com/n8n-hosting.html) (disclosure: that's us), where n8n comes pre-installed on your own server.

More detail on each template: [serverserv.com/n8n-templates.html](https://serverserv.com/n8n-templates.html)

## Licence

MIT. Use them for personal or business work, change them and share them.
