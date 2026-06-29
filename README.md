<div align="center">

# 🤖 AI-Powered Incident Management System

### Intelligent Incident Detection • Root Cause Analysis • Automated Ticketing • Agentic AI

![UiPath](https://img.shields.io/badge/UiPath-Agentic%20AI-orange)
![Maestro](https://img.shields.io/badge/Maestro-BPMN-blue)
![Studio Web](https://img.shields.io/badge/Studio-Web-success)
![Zoho Desk](https://img.shields.io/badge/Zoho-Desk-red)
![Outlook](https://img.shields.io/badge/Outlook-365-blue)

---

### 🚀 Built using UiPath Maestro • AI Agent • Studio Web • Orchestrator APIs • Zoho Desk APIs

</div>

---
# Project Description

The AI-Powered Incident Management System is an intelligent automation solution developed using UiPath Maestro, UiPath Studio Web, UiPath Agent Builder, Low-Code AI Agent, UiPath Orchestrator REST APIs, and Zoho Desk APIs. The solution automates the complete incident management lifecycle for unattended UiPath automations by continuously monitoring the latest completed Orchestrator jobs, analyzing execution logs using AI, identifying failures and their root causes, creating incident tickets, notifying the responsible developer, and maintaining a centralized execution history.

Unlike traditional incident management processes that require manual investigation of robot logs and ticket creation, this solution leverages an AI Agent to perform intelligent failure analysis and automate decision-making. The result is faster incident resolution, reduced manual effort, improved operational visibility, and increased reliability of enterprise automation processes.

---

# Problem Statement

Organizations often operate hundreds of unattended automation processes that execute critical business operations. When an automation fails, support teams must manually monitor UiPath Orchestrator, review execution logs, identify the root cause, determine the responsible developer, create an incident ticket, and notify stakeholders. This manual process is repetitive, time-consuming, and prone to human error, leading to increased Mean Time to Resolution (MTTR), operational delays, and reduced business productivity.

---

# 📌 Overview

Organizations often run hundreds of unattended automations every day.

When one automation fails, support teams typically need to:

- Review Orchestrator logs
- Identify the failure reason
- Find the responsible developer
- Create an incident ticket
- Notify stakeholders
- Maintain execution history

All of these activities are manual and time-consuming.

This solution automates the **entire Incident Management Lifecycle** using **UiPath Agentic AI**.

---

# 🎯 Key Features

✅ Automatic monitoring of latest completed Orchestrator Job

✅ Reads complete Robot Execution Logs

✅ AI-based Root Cause Analysis

✅ Failure Classification

✅ Responsible Developer Identification

✅ Priority Prediction

✅ Expected Resolution Time Prediction

✅ Automatic Zoho Desk Ticket Creation

✅ Automatic Email Notification

✅ Centralized Execution History

✅ Fully Low-Code Architecture

---

# 🏗 Solution Architecture

```text
Outlook Event Trigger
          │
          ▼
 Read Configuration
          │
          ▼
 Fetch Latest Job
          │
          ▼
 Fetch Robot Logs
          │
          ▼
      AI Agent
          │
   ┌──────┴──────┐
   │             │
Success       Failure
   │             │
   ▼             ▼
Update      Create Ticket
Records         │
                ▼
        Notify Developer
                │
                ▼
          Update Records
                │
                ▼
               End
````

---

## Agent Type

This solution utilizes a **Low-Code AI Agent** developed using **UiPath Agent Builder**.

The AI Agent analyzes UiPath Orchestrator job details, execution logs, and bot knowledge base information to perform root cause analysis, identify the responsible developer, determine ticket priority, estimate the expected resolution time, and recommend possible resolutions.

**Coded Agents:** Not Used

**Low-Code AI Agents:** Used

---

# 🧠 AI Agent Responsibilities

The Low-Code AI Agent analyzes:

* Job Details
* Robot Logs
* Bot Knowledge Base

Then predicts:

| AI Decision     | Description         |
| --------------- | ------------------- |
| Job Status      | Pass / Fail         |
| Root Cause      | Failure Reason      |
| Priority        | High / Medium / Low |
| Resolution Time | Estimated Time      |
| Developer       | Responsible Owner   |
| Resolution      | Suggested Fix       |

---

# 🛠 Technologies Used

| UiPath Components                        | External Services  |
| -------------------                      | ------------------ |
| Maestro BPMN                             | Zoho Desk REST API |
| UiPath Studio Web                        | Microsoft Outlook  |
| Agent Builder                            | OneDrive           |
| AI Agent                                 | Microsoft Excel    |
| Orchestrator                             |                    |
| UiPath Integration Service               |                    |
| Outlook Activities                       |                    |
| UiPath HTTP Request Activities           |                    |
| JSON Activities                          |                    |
| Excel Activities                         |                    |
| UiPath Assets                            |                    |
| UiPath OneDrive & SharePoint Activities  |                    |
| UiPath Low-Code AI Agent                 |                    |
| UiPath Orchestrator REST APIs            |                    |
| UiPath Outlook 365 Activities            |                    |
| UiPath OneDrive & SharePoint Activities  |                    |
| UiPath Event Trigger                     |                    |
| UiPath JSON Activities                   |                    |
| UiPath Variables & Arguments             |                    |
| API Workflows                            |                    |

---

# 📂 Project Structure

```
Incident Management
│
├── Incident Management Bot Data and Config.uis
├── Incident Management Orchestrator Data.uis
├── Incident Management Orchestrator Agent.uis
├── Incident Management Zoho Desk.uis
├── Incident Management Records.uis
├── Incident Management Flow.bpmn
│
├── Config.xlsx
├── Bot Data.xlsx
│
└── README.md
```

---
# 🚀 Setup Instructions

Follow the steps below to configure and run the **AI-Powered Incident Management System**.

---

## 📋 Prerequisites

Before starting, ensure you have access to:

* ✅ UiPath Automation Cloud Account
* ✅ UiPath Studio Web
* ✅ UiPath Maestro
* ✅ UiPath Orchestrator
* ✅ Microsoft Outlook 365 Account
* ✅ Microsoft OneDrive Account
* ✅ Zoho Desk Account
* ✅ Required permissions to create Orchestrator Assets and API Tokens

---

## Step 1: Download the Project

1. Download or clone this GitHub repository.
2. Extract the ZIP file to your local machine.

---

## Step 2: Upload the Excel Files

Upload the following files to your **Microsoft OneDrive**:

* `Config.xlsx`
* `Bot Data.xlsx`

> **Note:** These files are used by the workflows during execution.

---

## Step 3: Import the UiPath Workflows

1. Open **UiPath Studio Web**.
2. Click **Create New**.
3. Click the **▼** arrow next to **Create New**.
4. Select **Import**.
5. Import all the `.uis` workflow files included in the project.

---

## Step 4: Configure OneDrive Connection

1. Open the **Incident Management Bot Data and Config** workflow.
2. Replace the existing **OneDrive connection** with your own connection.
3. Save the workflow.

---

## Step 5: Update the Configuration File

Open **Config.xlsx** and update the following values:

* Cloud Name
* Organization Name
* Tenant Name
* Folder ID
* Bot Data Path
* Bot Data Sheet Name
* Notification Settings (if required)

Save the file after updating the configuration.

---

## Step 6: Configure the Bot Data Path

1. Copy the sharing link of **Bot Data.xlsx** from OneDrive.
2. Open **Config.xlsx**.
3. Paste the copied link into the **Bot Data Path** field.
4. Save the file.

---

## Step 7: Create Required Connections

Create and authorize the following connections in UiPath:

* Microsoft Outlook 365
* Microsoft OneDrive
* Zoho Desk

Replace all existing project connections with your own authenticated connections.

---

## Step 8: Generate an Orchestrator Personal Access Token

1. Open **UiPath Automation Cloud**.
2. Navigate to **Orchestrator**.
3. Click your **Profile** icon.
4. Select **Preferences**.
5. Open **Personal Access Tokens**.
6. Click **Create Token**.
7. Copy the generated token.

---

## Step 9: Create the Orchestrator Asset

In the same Orchestrator folder where the project is deployed:

1. Create a new **Text Asset**.
2. Name the Asset:

```text
Orchestrator_token
```

3. Paste the generated Personal Access Token as the Asset value.
4. Save the Asset.

---

## Step 10: Verify Asset Configuration

Open the **Incident Management Orchestrator Data** workflow and ensure the **Get Asset** activity is configured to retrieve:

```text
Orchestrator_token
```

from the correct Orchestrator folder.

---

## Step 11: Import the Maestro Workflow

Import the provided **Incident Management Maestro BPMN** file into UiPath Maestro.

---

## Step 12: Configure the Outlook Event Trigger

If you want to monitor a different mailbox or Outlook folder:

1. Open the Maestro BPMN.
2. Select the **Email Received** Event.
3. Open the **Tools** panel.
4. Select your Outlook account.
5. Choose the mailbox and folder to monitor.
6. Save and publish the workflow.

---

## Step 13: Publish the Solution

After completing all configurations:

1. Publish all UiPath workflows.
2. Publish the Maestro BPMN.
3. Ensure all connections and Assets are correctly configured.

---

## Step 14: Execute the Solution

1. Send a new email to the configured Outlook mailbox.
2. The Outlook Event Trigger will automatically start the Maestro workflow.
3. The solution will:

   * Read the configuration
   * Fetch the latest completed Orchestrator job
   * Retrieve execution logs
   * Analyze the execution using the AI Agent
   * Create a Zoho Desk ticket (if the job fails)
   * Notify the responsible developer
   * Update the centralized execution history

---

# ✅ Verification Checklist

Before running the solution, verify the following:

* [ ] All `.uis` workflows are imported.
* [ ] Maestro BPMN is imported and published.
* [ ] `Config.xlsx` and `Bot Data.xlsx` are uploaded to OneDrive.
* [ ] OneDrive, Outlook, and Zoho Desk connections are configured.
* [ ] `Orchestrator_token` Asset is created.
* [ ] Folder ID is correctly configured.
* [ ] All required permissions are granted.
* [ ] The Outlook Event Trigger is enabled.

---

# ⚠️ Important Notes

* Always publish the latest version of the Maestro workflow after making any changes.
* Ensure all external connections are replaced with your own authenticated connections before execution.
* Store the Personal Access Token securely and avoid sharing it publicly.
* Create a dedicated Orchestrator folder for this solution to prevent accidental execution loops with production automations.
* Every execution (successful or failed) is automatically recorded in the centralized execution history for auditing and reporting purposes.


---
# ⚙ Workflow Details

## 1️⃣ Incident Management Bot Data and Config

Responsible for:

* Reading Config.xlsx
* Reading Bot Data.xlsx
* Loading AI Knowledge Base
* Passing Configuration

---

## 2️⃣ Incident Management Orchestrator Data

Responsible for:

* Reading Personal Access Token
* Calling Orchestrator REST APIs
* Fetching Latest Completed Job
* Fetching Robot Logs
* Passing JSON to AI Agent

---

## 3️⃣ Incident Management Orchestrator Agent

The Intelligence Layer.

Performs:

* Root Cause Analysis
* Failure Detection
* Developer Identification
* Priority Prediction
* Suggested Resolution
* Resolution Time Estimation

---

## 4️⃣ Incident Management Zoho Desk

Executed only for failed jobs.

Creates:

* Zoho Ticket
* Returns Ticket ID
* Returns Ticket Status

---

## 5️⃣ Incident Management Records

Maintains execution history.

Stores:

* Process Name
* Job Status
* Failure Reason
* Ticket Number
* Ticket Status
* Owner
* Timestamp

---

## 6️⃣ Maestro BPMN

Main Orchestration Layer.

```
Email Trigger

↓

Read Configuration

↓

Fetch Job

↓

Fetch Logs

↓

AI Analysis

↓

Decision

↓

Success → Update Records

Failure → Ticket → Email → Update Records
```

---

# 📊 Excel Files

## Config.xlsx

Contains:

* Cloud Name
* Organization Name
* Tenant Name
* Folder ID
* Bot Data Path
* Notification Settings
* Knowledge Base Path

---

## Bot Data.xlsx

Contains:

* Bot Name
* Developer
* Manager
* Business Priority
* Contact Details
* Business Description
* Additional Metadata

---

# 🚀 Initial Setup

## Step 1

Extract the ZIP Folder.

---

## Step 2

Upload both Excel files to your OneDrive.

---

## Step 3

Import every `.uis` file into UiPath Studio Web.

---

## Step 4

Replace OneDrive Connections.

---

## Step 5

Update Config.xlsx.

---

## Step 6

Replace:

* Outlook Connection
* Zoho Desk Connection
* OneDrive Connection

---

## Step 7

Import Maestro BPMN.

---

# ☁ Orchestrator Configuration

## Generate Personal Access Token

```
Cloud Portal

↓

Orchestrator

↓

Profile

↓

Preferences

↓

Personal Access Token

↓

Create Token
```

---

## Create Asset

Create a **Text Asset**

```
Orchestrator_token
```

Paste the generated Personal Access Token.

---

## Verify Asset

Inside

```
Incident Management Orchestrator Data
```

Verify Get Asset uses

```
Orchestrator_token
```

---

# 📁 Config File

Update:

* Cloud Name
* Organization
* Tenant
* Folder ID
* Bot Data Path
* Sheet Name

---

# 📌 Finding Folder ID

Open the desired Orchestrator Folder.

Browser URL:

```
fid=123456789
```

Copy the value after **fid=**

---

# 📧 Event Trigger Configuration

The Maestro BPMN starts automatically whenever an email is received.

To change the monitored mailbox:

1. Open Maestro BPMN
2. Select Email Received
3. Open Tools Panel
4. Select Outlook Account
5. Choose Folder
6. Publish Again

---

# 🔄 Complete Execution Flow

```text
Email Received
      │
      ▼
Read Configuration
      │
      ▼
Fetch Latest Job
      │
      ▼
Fetch Execution Logs
      │
      ▼
AI Analysis
      │
      ▼
Pass?
│
├─────────────── Yes ───────────────┐
│                                   │
▼                                   ▼
Update Records                    End

No
│
▼
Create Zoho Ticket
│
▼
Notify Developer
│
▼
Notify Manager (Business Critical)
│
▼
Update Records
│
▼
End
```

---

# 📝 Notes

> **Important**

* Publish the latest Maestro BPMN after changes.
* Replace every external connection.
* Verify Folder ID.
* Upload both Excel files.
* Ensure `Orchestrator_token` Asset exists.
* Every execution is logged.
* Set Agent Priority to **Highest**.
* Create a dedicated Orchestrator Folder for this project.
* **Do not deploy these workflows inside your production automation folder**, as doing so may create recursive execution loops.

---

# 👨‍💻 Author

**Gagan Grover**

Associate Consultant | UiPath RPA Developer

Specializing in:

* Agentic AI
* UiPath Maestro
* Studio Web
* AI Agents
* API Integrations
* Intelligent Automation

---

⭐ If you found this project useful, don't forget to Star the repository.

```
```
