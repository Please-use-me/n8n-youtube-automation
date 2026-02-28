🤖 AutoTube-n8n: Autonomous AI Video Agent

AutoTube-n8n is a fully automated content pipeline built in n8n. It transforms raw ideas from a Google Sheet into fully rendered videos with AI-generated scripts and music, then uploads them directly to YouTube without any manual intervention.


🚀 Features
1.Scheduled Execution: The "Schedule" node checks for new content every hour.

2.AI Scriptwriting: Uses OpenAI to generate engaging video scripts based on sheet data.

3.Automated Soundtrack: A "Pick Random Music" function selects background tracks from a curated library.

4.Headless Rendering: Integrates with the json2video API to produce movie files via HTTP requests.

5.Smart Polling: A "Wait" node pauses for 30 seconds before checking if the render is complete.

6.Auto-Publishing: Downloads the finished video and uploads it directly to YouTube.

7.Error Handling: Failed renders are logged back to a "errors" sheet for easy debugging.



🛠️ Tech Stack
Workflow Engine: n8n

Brain: OpenAI (GPT-4/Turbo)

Database: Google Sheets

Video Engine: Json2Video API

Platform: YouTube Data API



📦 Quick Setup
Import: Load the AI_Video_Automation.json into your n8n instance.

Credentials: Set up your OpenAI, Google Sheets, and YouTube OAuth2 credentials in n8n.

Sheet IDs: Update the "Sheet ID" parameters in the Read, Update, and Error Log nodes with your specific Google Spreadsheet ID.

Activate: Set the workflow to "Active" to begin the hourly schedule.
