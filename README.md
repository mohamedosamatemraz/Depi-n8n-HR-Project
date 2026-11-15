# OMNA People -- HR Automation

OMNA People is an HR automation project built with n8n to support
recruitment workflows, application screening, and candidate assistance.
It also includes an HR policy knowledge base that can answer questions
using the provided policy documents.

## Live Website

https://mohamedosamatemraz.github.io/Depi-n8n-HR-Project/

> This link will be available after GitHub Pages is enabled and the site
> configuration is completed.

## Workflows

  Workflow                         Trigger
  -------------------------------- ---------------------------------------------
  Recruitment 1 -- Intake          Form submission
  Recruitment 2 -- AI Screening    Schedule (every hour)
  Recruitment 3 -- Error Handler   Error trigger and scheduled triggers
  Job Application Coach            Form submission
  RAG + GPT                        Chat trigger
  Policy Loader                    Manual trigger and daily schedule (7:00 AM)

## Services and Tools

-   n8n -- workflow automation
-   Google Drive -- HR policy document storage
-   Google Sheets -- recruitment data
-   Google Gemini -- AI processing and embeddings
-   ngrok -- public access to the n8n instance and webhooks
-   GitHub Pages -- project website hosting

## Import Instructions

1.  Download the workflow JSON files from this repository.
2.  In n8n, import the required workflow files.
3.  Configure the credentials required by the nodes in each workflow.
4.  Update workflow-specific configuration values and resource
    references for your environment.
5.  Set the error-workflow relationship where applicable.
6.  Activate the workflows that use production triggers.
7.  Update the `CONFIG` object in `index.html` with your n8n base URL
    and the relevant webhook/form paths.

## Security

Do not add API keys, credentials, private IDs, or personal email
addresses to this repository. Configure credentials securely inside n8n.
