Intelligent Feedback Segregation Workflow (n8n + AI)
An advanced automation pipeline built with n8n, Google Gemini, Slack, Airtable, and Gmail API. This system is designed to intelligently classify and route user feedback, transforming raw user input into actionable insights automatically.

Problem Statement
Many organizations struggle with the high volume of user feedback received through forms, emails, and surveys. They often lack the infrastructure to categorize, respond to, and route this feedback in real-time.

This typically results in:

Delays in resolving user complaints

Feature requests getting lost

Positive feedback not reaching the right teams

Solution Overview
This workflow addresses these bottlenecks by integrating AI-based classification, real-time database routing, team collaboration, and automated user communication into a single, seamless process.

Key Capabilities
AI Classification: Leverages Google Gemini 1.5 Flash to categorize feedback as:

Complaint

Compliment

Feature Request

Structured Storage in Airtable: Automatically logs feedback in separate tables based on its category. Each record includes: name, email, feedback, and classification.

Real-Time Slack Notifications: Sends categorized feedback, along with all relevant user information, to the appropriate Slack channels or teams.

Gmail API Auto-Responses: If a complaint is detected, the user immediately receives a professional email acknowledging their concern.

Flexible Input Triggers: While it starts with an n8n form, the system can easily adapt to inputs from Google Forms, Microsoft Forms, or any webhook-enabled frontend.

Workflow Lifecycle
Form Submission: A user submits feedback via an n8n form or an external webhook.

AI Analysis: The feedback content is analyzed and interpreted using Gemini 1.5 Flash.

Conditional Routing:

Stored in Airtable under the correct category table.

Posted to Slack with metadata (name, email, message, type).

If a complaint, triggers a Gmail auto-response.

Visual Overview
Included Assets
File

Description

workflow.json

Full export of the n8n workflow logic

screenshot.png

Visual layout of the automation workflow


Export to Sheets
Tech Stack
n8n: Self-hosted automation platform

Google Gemini 1.5 Flash: LLM for NLP classification

Airtable: Categorical data storage

Slack: Internal team alerts

Gmail API: Transactional responses

Ideal Use Cases
SaaS startups automating user feedback intake

Product teams streamlining feature tracking

Customer support teams requiring immediate complaint acknowledgment

Businesses scaling up Customer Experience (CX) automation with AI tools

Author
Sanskar Awasthi

Email: sanskarawasthi93@gmail.com

GitHub: @sanskar-94

Upwork: https://www.upwork.com/freelancers/~015a6baf82356aebbe

⭐ If this project helped you or inspired an idea, feel free to star the repo or connect with me for collaborations!
