

# CRM Automation with n8n

A production-style CRM automation system built using **n8n** that automates lead processing, validation, routing, and storage while implementing reliability features like error handling and retry recovery.

---

# Project Evolution

## Version 1.0 — CRM Automation Foundation

Initial CRM automation system using Google Sheets as the data storage layer.

Implemented:

- Lead capture automation
- Webhook-based triggers
- Data validation
- Lead scoring
- Country-based routing
- Team assignment
- Google Sheets CRM storage


---

## Version 1.1 — Reliability Upgrade

Added production reliability features to improve workflow stability.

New features:

- Centralized error handling workflow
- Failure monitoring
- Retry recovery workflow
- Improved workflow debugging


---

# Architecture

## Main Workflow


Lead Source
|
|
Webhook Trigger
|
|
Data Validation
|
|
Lead Processing
|
|
Lead Scoring
|
|
Country Routing
|
|
Team Assignment
|
|
Google Sheets CRM Storage



## Failure Handling Architecture


Main Workflow

  |
  |

Workflow Failure

  |
  |

Error Handler Workflow

  |
  |

Capture Error Details

  |
  |

Retry Handler Workflow


---

# Features

## CRM Automation

✅ Webhook trigger  
✅ Lead validation  
✅ Lead scoring  
✅ Country-based routing  
✅ Team assignment  
✅ Google Sheets CRM storage  


## Reliability System

✅ Centralized error handling  
✅ Failure tracking  
✅ Retry mechanism  
✅ Workflow recovery process  


---

# Repository Structure


crm-automation-n8n/

├── README.md

├── workflows/
│ ├── CRM LEAD AUTOMATION.json
│ ├── error_handler_workflow.json
│ └── retry_failure_handler_workflow.json

├── documentation/
│ ├── architecture.md
│ ├── error_handling.md
│ └── retry_mechanism.md

└── screenshots/
├── main_workflow.png
├── error_handler_workflow.png
└── retry_handler_workflow.png


---

# Technology Stack

- n8n
- Webhooks
- REST APIs
- JSON
- Google Sheets API


---

# Documentation

Detailed documentation:

- [System Architecture](documentation/architecture.md)
- [Error Handling](documentation/error_handling.md)
- [Retry Mechanism](documentation/retry_mechanism.md)


---

# Future Improvements

## Version 2.0 — PostgreSQL Migration

Planned improvements:

- Replace Google Sheets with PostgreSQL database
- Design relational database schema
- Add SQL-based lead management
- Implement database indexing
- Improve scalability and performance


## Future Features

- Email notifications
- AI-based lead qualification
- Analytics dashboard
- Production deployment


---

# Project Status

Current Version:

**v1.1 — Reliability Upgrade**

Completed:

✅ CRM automation workflow  
✅ Error handling system  
✅ Retry recovery system  

Next:

🚀 PostgreSQL database integration
