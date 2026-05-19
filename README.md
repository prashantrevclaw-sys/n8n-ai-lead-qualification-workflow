# n8n AI Lead Qualification Workflow

This project is an AI-powered lead qualification and routing workflow built with n8n.

It takes a new lead, validates the data, sends the lead details to an AI model, returns a structured score and summary, routes the lead based on urgency, updates the CRM, logs the result, and alerts the team.

## What This Workflow Does

1. Receives a new lead through webhook/form input
2. Cleans and validates lead data
3. Uses AI to score and summarize the lead
4. Routes hot, warm, cold, or invalid leads
5. Updates CRM/pipeline status
6. Logs the result in Google Sheets
7. Sends team alerts for high-priority leads
8. Includes error logging and manual review path

## Workflow Screenshot
<img width="587" height="134" alt="n8n workflow" src="https://github.com/user-attachments/assets/ccf88285-a0a7-40a2-ba09-ce315359d9f7" />


## Tools Used

- n8n
- OpenAI / Claude API
- Webhooks
- Google Sheets
- CRM workflow logic
- Slack / team alerts
- JSON-based AI output

## Example Use Case

A marketing agency or service business receives leads from forms, ads, landing pages or CRM sources.

Instead of manually checking every lead, this workflow automatically checks the lead quality, gives a score, recommends the next action, and alerts the right person.

## Sample AI Output

```json
{
  "lead_score": 85,
  "lead_status": "Hot Lead",
  "summary": "The lead is asking for urgent service and has provided complete contact details.",
  "next_action": "Send booking link and alert sales team",
  "priority": "High"
}
