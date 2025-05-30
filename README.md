# Leadership Digest Project

## Overview
Automate leadership email summaries using n8n and AI agents.

## Goals
- Fetch emails from Gmail.
- Summarize using GPT model.
- Post to Notion or Slack.

## Tools
- n8n
- OpenRouter.ai
- Notion API

## System Architecture (Mermaid Diagram)

```mermaid
flowchart TD
    A[Gmail API] --> B[n8n Workflow]
    B --> C[Filter by subject: Leadership tip of the week]
    C --> D[Send email body to OpenRouter GPT model]
    D --> E[Summarize the content]
    E --> F[Post the summarized tip to Notion or Slack]
