# CRM Automation Architecture

## Overview

This project is a production-style CRM automation system built using n8n.

The system automates lead collection, validation, processing, routing, and storage while implementing reliability features such as error handling and retry recovery.

---

# System Flow

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
Country Based Routing
|
|
Team Assignment
|
|
Google Sheets CRM Storage


---

# Reliability Architecture

To improve workflow reliability, separate failure handling workflows are implemented.


Main Workflow

Lead Processing
|
|
Failure Occurs
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

# Components

## Main CRM Workflow

Responsible for:

- Receiving lead data
- Validating input
- Processing lead information
- Assigning teams
- Storing CRM records


## Error Handler Workflow

Responsible for:

- Capturing failed executions
- Recording error information
- Sending failure notifications


## Retry Handler Workflow

Responsible for:

- Detecting failed operations
- Retrying temporary failures
- Preventing unlimited retry loops


---

# Current Version

## Version 1.1 - Reliability Upgrade

Added:

- Centralized error handling
- Retry recovery mechanism
- Improved workflow monitoring


---

# Future Improvements

- PostgreSQL database integration
- Advanced analytics
- AI-based lead qualification
- Production deployment
