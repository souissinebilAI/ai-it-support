# Power Automate

## Flow

`AI_IT_Support_Analyze`

## Purpose

The flow connects Power Apps with Microsoft Foundry and returns the AI analysis to the application.

## Workflow

```text
Power Apps
    ↓
When Power Apps calls a flow (V2)
    ↓
Invoke an HTTP request
    ↓
Microsoft Foundry
    ↓
Compose
    ↓
Respond to a Power App or flow
    ↓
Power Apps
