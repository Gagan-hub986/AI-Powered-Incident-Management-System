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

| UiPath Components   | External Services  |
| ------------------- | ------------------ |
| Maestro BPMN        | Zoho Desk REST API |
| Studio Web          | Microsoft Outlook  |
| Agent Builder       | OneDrive           |
| AI Agent            | Microsoft Excel    |
| Orchestrator        |                    |
| Integration Service |                    |
| Outlook Activities  |                    |
| HTTP Request        |                    |
| JSON Activities     |                    |
| Excel Activities    |                    |
| Assets              |                    |
| Event Trigger       |                    |

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
