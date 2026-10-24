# AI-Assisted EU Data Update Automation with n8n

An **n8n-based automation project** that helps maintain a structured information database by processing incoming updates, using AI to assess relevant changes, and coordinating records across connected services.

## Overview

The workflow reduces repetitive review and data-entry tasks while allowing human oversight when the system cannot confidently determine the next action. It combines scheduled automation, webhooks, AI-assisted analysis, and spreadsheet updates in a single process.

## What the Automation Does

- **Detects new information:** Monitors incoming changes and prepares them for processing.
- **Assesses records with AI:** Uses language models to help identify relevant records and draft suitable updates.
- **Routes exceptions for review:** Sends uncertain cases through an approval process instead of applying changes blindly.
- **Synchronizes information:** Updates corresponding records in connected spreadsheets and data stores.
- **Tracks outcomes:** Maintains an update history and supports notifications for completed or exceptional actions.

## Workflow Preview

![Sanitized n8n workflow overview](screenshots/workflow-overview-public.png)

*Redacted overview of the n8n workflow. Node-level labels and client-specific routing details are intentionally obscured.*

## Technology Stack

| Tool | Role |
| --- | --- |
| **n8n** | Workflow orchestration, triggers, conditional paths, and integrations |
| **OpenAI API** | AI-assisted record analysis and update suggestions |
| **Google Sheets** | Structured record management and update tracking |
| **Webhooks** | Approval and event-driven actions |
| **JavaScript** | Lightweight data transformation and validation |

## Implementation Notes

The workflow is designed around separating routine updates from cases requiring review. It uses conditional processing, structured responses, and change tracking to support more consistent data maintenance. Configuration and operational behavior depend on the connected environment.

## Confidentiality

This repository is a **portfolio overview**, not a deployable copy of the client system. Private data, access links, prompts, business-specific rules, credentials, workflow exports, and identifying labels are intentionally excluded. The screenshot has been sanitized for public display.
