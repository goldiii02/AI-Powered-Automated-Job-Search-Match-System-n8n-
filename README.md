# AI-Powered Automated Job Search & Match System (n8n)

An end-to-end job automation workflow built with n8n that collects user preferences, fetches relevant job postings from public APIs, processes and deduplicates the data, and delivers personalized job reports via email.

The system is designed to reduce manual job searching by providing users with a structured daily digest of relevant opportunities.

---

## Overview

This project demonstrates how workflow automation and API integrations can be combined to build a production-style job aggregation pipeline.

The workflow:

- Captures user preferences through a form  
- Retrieves job listings from external APIs  
- Normalizes and cleans raw job data  
- Removes duplicate postings  
- Aggregates the most relevant opportunities  
- Sends a formatted email report to the user  

The architecture is modular and can be extended to support additional job sources or AI-based ranking.

---

## Key Features

### Automated Job Aggregation

The system automatically fetches job listings from external job APIs (currently Arbeitnow, extensible to others). This removes the need for manual job searching across multiple platforms.

---

### Data Normalization and Deduplication

Raw job data often contains inconsistencies and duplicates. The workflow includes a preprocessing layer that:

- Standardizes job fields  
- Cleans incomplete records  
- Removes duplicate listings  
- Prepares structured output for downstream steps  

This improves the quality of results delivered to users.

---

### Personalized Email Delivery

Each user receives a structured HTML email containing relevant job opportunities based on their submitted preferences.

The email includes:

- Job title  
- Company name  
- Location  
- Direct job link  

Email delivery is handled through the Gmail API integration within n8n.

---

### Scheduled Execution

The workflow supports automated execution using the n8n scheduler, enabling periodic job scans and continuous delivery of opportunities without manual intervention.

---

## Workflow Architecture

Main pipeline components:

1. User Profile Form  
2. Input Validation  
3. Profile Storage  
4. Job Fetch (Arbeitnow API)  
5. Job Combination Layer  
6. Split and Normalize  
7. Duplicate Removal  
8. Aggregation  
9. Email Notification  

![Workflow](./workflow.png)

---

## Tech Stack

- n8n (workflow automation)  
- REST APIs  
- Arbeitnow Jobs API  
- Gmail API  
- JavaScript expressions (n8n)  
- Render (optional self-hosting)  
- n8n Cloud (form endpoint)

---

## Live Demo

Public Form  
https://goldiii.app.n8n.cloud/form/9265bf1f-9bba-44f4-95b1-2251fc2ed105

Repository  
https://github.com/goldiii02/AI-Powered-Automated-Job-Search-Match-System-n8n-

---

## How It Works

### Step 1: User Submission

The user submits:

- Name  
- Email  
- Desired role  
- Preferred locations  
- Skills  

---

### Step 2: Job Retrieval

The system fetches the latest job postings from supported APIs.

---

### Step 3: Processing Pipeline

The workflow performs:

- Data normalization  
- Deduplication  
- Aggregation  

---

### Step 4: Email Delivery

A formatted job report is automatically sent to the user's email.

---

## Local Setup (Self-Hosted n8n)

### Prerequisites

- Running n8n instance  
- Gmail credentials configured  
- Internet access for job APIs  

---

### Setup Steps

1. Import the workflow JSON into n8n  
2. Configure Gmail credentials  
3. Update API nodes if needed  
4. Activate the workflow  
5. Share the form URL with users  

---

## Possible Enhancements

- Semantic job matching using LLMs  
- Multi-source job aggregation  
- LinkedIn integration  
- Vector similarity ranking  
- Auto-apply functionality  
- User dashboard and analytics  

---

## Author

Goldi Rathore  
Software Engineer / Automation Engineer  
Email: goldirathore2003@gmail.com
