# Intelligent Feedback Segregation Workflow (n8n + AI)

An advanced automation pipeline crafted with *n8n, **Google Gemini, **Slack, **Airtable, and **Gmail API, designed to **intelligently classify and route user feedback*. This system streamlines how organizations handle complaints, compliments, and feature requests — transforming raw user input into actionable insights, automatically.

---

## Problem Statement

Many organizations receive a high volume of user feedback through forms, emails, and surveys — yet *lack the infrastructure to categorize, respond, and route that feedback in real-time*.

This results in:
•⁠  ⁠Delays in resolving user complaints  
-  Feature requests getting lost  
-  Positive feedback not reaching the right teams  

---

## Solution Overview

This workflow solves that bottleneck by integrating *AI-based classification, **real-time database routing, **team collaboration, and **automated user communication* into a single seamless process.

### Key Capabilities

-  *AI Classification: Uses **Google Gemini 1.5 Flash* to detect whether feedback is a:
  - Complaint
  - Compliment
  - Feature Request

-  *Structured Storage in Airtable*:
  - Automatically logs feedback in *separate tables* based on category
  - Each record contains: name, email, feedback, classification

-  *Real-Time Slack Notifications*:
  - Sends categorized feedback to appropriate Slack channels/teams with all relevant user info

-  *Gmail API Auto-Responses*:
  - If a complaint is detected, the user receives an immediate, professional email acknowledging their concern

-  *Flexible Input Triggers*:
  - Starts from an *n8n form*, but can easily be adapted to Google Forms, Microsoft Forms, or any webhook-enabled frontend

---

## Workflow Lifecycle

1.⁠ ⁠*Form Submission* – User submits feedback (via n8n form or external webhook)
2.⁠ ⁠*AI Analysis* – Feedback content is interpreted using *Gemini 1.5 Flash*
3.⁠ ⁠*Conditional Routing*:
   - Stores in *Airtable* under the correct category table
   - Posts to *Slack* with metadata (name, email, message, type)
   - If complaint → triggers *Gmail auto-response*

---

## Visual Overview

![Workflow Screenshot](screenshot.png)

---

## Included Assets

| File | Description |
|------|-------------|
| ⁠ workflow.json ⁠ | Full export of the n8n feedback segregation logic |
| ⁠ screenshot.png ⁠ | Visual layout of the automation workflow |

---

## Tech Stack

•⁠  ⁠*n8n* (Self-hosted automation platform)
•⁠  ⁠*Google Gemini 1.5 Flash* (LLM for NLP classification)
•⁠  ⁠*Airtable* (Categorical data storage)
•⁠  ⁠*Slack* (Internal team alerts)
•⁠  ⁠*Gmail API* (Transactional responses)

---

## Ideal Use Cases

•⁠  ⁠SaaS startups automating user feedback intake  
•⁠  ⁠Product teams looking to streamline feature tracking  
•⁠  ⁠Customer support teams wanting immediate complaint acknowledgment  
•⁠  ⁠Businesses scaling up CX automation with AI tools  

---

## Author

*Sanskar Awasthi*  
Email: [sanskarawasthi93@gmail.com](mailto:sanskarawasthi93@gmail.com)  
GitHub: [@sanskar-94](https://github.com/sanskar-94)  

---

	⁠⭐ If this project helped you or inspired an idea, feel free to star the repo or connect with me for collaborations!\
