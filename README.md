# 🤖 AI IT Support

> AI-powered IT service desk built with Microsoft Power Apps, Microsoft Dataverse, Power Automate, and Microsoft Foundry.

## 📌 Project Overview

**AI IT Support** is a portfolio project that demonstrates how modern Microsoft cloud technologies and generative AI can be combined to improve an internal IT service desk workflow.

Employees can submit IT support requests through a Power Apps Canvas App. An AI support agent analyzes the reported problem, classifies the issue, recommends a priority, summarizes the problem, and provides troubleshooting guidance.

The AI recommendation is then returned to the application and can influence the ticket priority while keeping the final decision with the user or IT technician.

---

## ✨ Key Features

### 🎫 IT Ticket Management

- Create IT support tickets
- Validate employees against Dataverse
- Store tickets in Microsoft Dataverse
- Search and filter tickets
- Manage ticket status
- Assign tickets to IT employees
- View detailed ticket information

### 🤖 AI-Powered Support Analysis

The Microsoft Foundry agent analyzes incoming support requests and provides:

- **Issue category**
  - Hardware
  - Software
  - Network
  - Account & Access
  - Security
  - Other

- **Recommended priority**
  - Low
  - Medium
  - High
  - Critical

- Problem summary
- Troubleshooting steps
- Recommended next action
- Follow-up questions when required

### 🔄 AI → Application Integration

The AI recommendation is integrated directly into the Power Apps workflow.

For example:

User reports a company-wide network outage
              ↓
Microsoft Foundry analyzes the request
              ↓
Recommended priority: Critical
              ↓
Power Automate returns the AI response
              ↓
Power Apps selects "Critical"
              ↓
User can review or change the priority
              ↓
Ticket is submitted to Dataverse IT Ticket

                         ┌─────────────────────┐
                         │      Employee       │
                         └──────────┬──────────┘
                                    │
                                    ▼
                         ┌─────────────────────┐
                         │   Power Apps        │
                         │   Canvas App        │
                         └──────┬───────┬──────┘
                                │       │
                    Submit      │       │ Analyze
                    Ticket      │       │ with AI
                                │       ▼
                                │  ┌─────────────────┐
                                │  │ Power Automate  │
                                │  └────────┬────────┘
                                │           │
                                │           ▼
                                │  ┌─────────────────┐
                                │  │ Microsoft       │
                                │  │ Foundry         │
                                │  │ AI Agent        │
                                │  └────────┬────────┘
                                │           │
                                │           ▼
                                │  ┌─────────────────┐
                                │  │ AI Analysis     │
                                │  └────────┬────────┘
                                │           │
                                │           ▼
                                │  ┌─────────────────┐
                                │  │ Power Automate  │
                                │  └────────┬────────┘
                                │           │
                                └───────────┼──────────────┐
                                            ▼              │
                                  ┌─────────────────┐      │
                                  │ Microsoft       │◄─────┘
                                  │ Dataverse       │
                                  └─────────────────┘
## Technology Stack

| Technology               | Purpose                                   |

| Microsoft Power Apps     | Canvas App and user interface             |
| Microsoft Dataverse      | IT ticket and employee data               |
| Microsoft Power Automate | Workflow orchestration and AI integration |
| Microsoft Foundry        | AI agent and model integration            |     
| GitHub                   | Source control and documentation          |

## Key Features

- IT ticket creation
- Employee validation
- Ticket search and filtering
- Ticket status management
- Ticket assignment
- AI-powered IT issue analysis
- AI issue categorization
- AI priority recommendation
- AI-generated troubleshooting guidance
- AI recommendation integrated into the Power Apps workflow
- Human override of AI recommendations

## AI Workflow

The Microsoft Foundry agent analyzes an IT support request and provides:

1. Issue category
2. Recommended priority
3. Problem summary
4. Troubleshooting steps
5. Recommended next action
6. Follow-up questions when required

The recommended priority is returned to Power Apps and automatically selected in the priority field. The user can still change the recommendation before submitting the ticket.

## Project Status

Core application completed.

Implemented:

- [x] Power Apps Canvas App
- [x] Microsoft Dataverse backend
- [x] Power Automate integration
- [x] Microsoft Foundry AI agent
- [x] AI issue classification
- [x] AI priority recommendation
- [x] AI → Power Apps priority integration
- [x] Ticket management
- [x] Ticket assignment
- [x] GitHub documentation

## Security

This repository does not contain passwords, API keys, access tokens, connection credentials, employee records, or production ticket data.

                                  
