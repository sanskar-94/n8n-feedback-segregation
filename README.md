# Intelligent Feedback Segregation Workflow (n8n + AI)

An advanced AI-powered automation pipeline built using n8n, Google Gemini, Slack, Airtable, and the Gmail API. This workflow is designed to intelligently categorize and route incoming user feedback, transforming raw inputs into actionable insights in real time.

---

## Problem Statement

Many organizations face challenges in managing the high volume of user feedback received through forms, emails, and surveys. Often, there is no streamlined system in place to categorize, respond to, and route this feedback efficiently.

Common issues include:

- Delays in responding to user complaints  
- Feature requests being overlooked  
- Positive feedback not reaching the relevant teams  

---

## Solution Overview

This workflow solves these challenges by integrating AI-driven classification, real-time database storage, internal team collaboration, and automated user communication—all within a single automated system.

---

## Key Capabilities

### AI-Based Classification  
Uses Google Gemini 1.5 Flash to classify feedback into the following categories:

- Complaint  
- Compliment  
- Feature Request  

### Airtable-Based Structured Storage  
Automatically logs each feedback entry into Airtable with the following fields:
- Name  
- Email  
- Feedback message  
- Category  

Each feedback type is stored in its corresponding table for better organization and tracking.

### Real-Time Slack Notifications  
Routes categorized feedback to the appropriate Slack channels along with associated metadata such as name, email, feedback message, and type.

### Automated Gmail Responses  
For complaints, the system sends an immediate and professional acknowledgment email via the Gmail API to the user.

### Flexible Input Triggers  
Though designed with an n8n form as the primary input source, this workflow can be extended to support:
- Google Forms  
- Microsoft Forms  
- Any webhook-enabled frontend  

---

## Workflow Lifecycle

1. **Form Submission**  
   A user submits feedback through an n8n form or any external webhook-integrated form.

2. **AI Analysis**  
   Google Gemini 1.5 Flash processes the feedback to determine its category.

3. **Conditional Routing**  
   - Feedback is stored in the corresponding Airtable table  
   - A Slack notification is sent to the appropriate team or channel  
   - If the category is "Complaint", a Gmail auto-response is triggered to acknowledge the user  

---

## Visual Overview

| File             | Description                                 |
|------------------|---------------------------------------------|
| `workflow.json`  | Full export of the n8n workflow logic       |
| `screenshot.png` | Visual layout of the entire workflow        |

---

## Tech Stack

- **n8n** – Workflow automation platform (self-hosted)
- **Google Gemini 1.5 Flash** – Large Language Model (LLM) for natural language classification
- **Airtable** – Structured, category-based feedback storage
- **Slack** – Internal communication and notifications
- **Gmail API** – Automated responses for complaint submissions

---

## Ideal Use Cases

- SaaS startups automating feedback processing at scale  
- Product teams managing and prioritizing feature requests  
- Customer support teams ensuring immediate complaint acknowledgment  
- Organizations scaling Customer Experience (CX) using AI and automation  

---

## Author

**Sanskar Awasthi**  
Email: [sanskarawasthi93@gmail.com](mailto:sanskarawasthi93@gmail.com)  
GitHub: [@sanskar-94](https://github.com/sanskar-94)  
Upwork: [https://www.upwork.com/freelancers/~015a6baf82356aebbe](https://www.upwork.com/freelancers/~015a6baf82356aebbe)

---

## Support

If you found this project valuable or would like to collaborate, feel free to star the repository or reach out directly.
