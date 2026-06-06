# client-onboarding-automation with Zapier
---

An automated client onboarding workflow built with **Zapier** and **Google Apps Script** 
that eliminates manual tasks, reduces onboarding time, and delivers a seamless experience 
for new clients.

## What This Automation Does
---

- Triggers when a new client fills out an intake form
- Automatically sends a personalised welcome email
- Create a client record in CRM, such as HubSpot, Airtable, Google Sheets, or AppScript.
- Schedules an onboarding call via Calendly.
- Send follow-up reminders at key intervals.
- Notifies the internal team via Slack or Email.
- Create a project folder in Google Drive.
- Runs custom Google Apps Script logic for data processing & dynamic actions.



  
 ## Tools & Integrations Used
 
---

  |TOOL                    |        ROLE                       |
  |--------------------    | ---------------------------       |
  |**Zapier**              | Automation backbone               |
  |**Google form**         | Client intake trigger             |
  |**Gmail**               | Automated email delivery          |
  |**Google sheet**        | Client database                   |
  |**Calendly**            | Onboarding call scheduling        |
  |**Slack**               | Internal team notiifications      |
  |**Google Drive**        | Client folder creation            |
  |**Google Apps Script**  | custom script for data processing |
  ---


   ## Demo
 >[Watch the full workflow demo](https://www.loom.com/share/6a3a23c2e426438fbdc439dc2e6518ea)

---
## Client Onboarding Automation Workflow
---
<img width="16384" height="6587" alt="AutopilotEmailSupport" src="https://github.com/user-attachments/assets/6093b3ac-9133-4e7f-9376-5a9cd6dad974" />

## Project Overview
---
A fully automated, multi-path client onboarding system built with 
**Zapier**, **Google Apps Script**, and **Google Workspace**. The workflow intelligently 
classifies incoming client requests and routes them through customized handling paths, 
all without manual work.

## Step-by-Step on How the Workflow Works
---

## Step 1 — Intake & Processing (Steps 1–4)

|  STEP                  |          PROCESS                                      |
|----------------------- |-----------------------------------------------------  |
| **Google Forms**       | Captures new client form submission (trigger)         |
| **Formatter by Zapier**| Cleans and formats the raw form text                  |
| **Code by Zapier**     | Runs custom logic to process and classify the data    |
| **Google Sheets**      | Creates a new spreadsheet row to log the submission   |

##  Step 2 — Request Classification (Step 5)

 ## PATH
 ## Request Type — Splits the workflow into 3 branches

|  PATH TYPE                |      PURPOSE                                         |  
|-------------------------- |----------------------------------------------------  |
| **Complaint**             | Handles client complaints with urgency detection     |
| **Feature Request**       | Logs and processes new feature requests              |
| **General Inquiry**       | Routes general questions to the right response       |

### Step 3 — Complaint Handling (Steps 6–14)

**Path conditions** — Confirms complaint type
**Path Urgency** — Detects urgency level and splits into three
1. High Urgency
2. Medium Urgency
3. Low Urgency

**High Urgency** 
- Checks routing schedule (Yes/No path)

**Yes** 
- Runs JavaScript
- Creates Google Calendar event
- Calls Sub-Zap
- Logs data in Google Sheets
       
**No**
- Calls Sub-Zap
- Logs data in Google Sheets      

