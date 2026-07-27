# SentinelAI

An intelligent Security Operations Automation platform built with **n8n**, **PostgreSQL**, **Google Gemini AI**, and **Gmail** to automate the end-to-end cybersecurity incident response lifecycle.

The project demonstrates how workflow automation and AI can streamline SOC (Security Operations Center) activities by reducing manual effort, improving incident prioritization, accelerating response time, and generating actionable security reports.

---

## Overview

Modern organizations receive thousands of security alerts every day from firewalls, endpoint protection platforms, IDS/IPS systems, cloud monitoring services, and security appliances. Security analysts often spend significant time reviewing alerts, identifying false positives, assigning incidents, notifying stakeholders, and preparing reports.

SentinelAI addresses these challenges by automating the incident management lifecycle through modular n8n workflows enhanced with AI-powered threat analysis.

---

## Key Features

- Automated Security Alert Collection
- AI-Based Threat Classification
- Dynamic Incident Prioritization
- Automated Incident Assignment
- Daily Security Dashboard Generation
- HTML Email Reporting
- Scheduled Workflow Automation
- PostgreSQL-based Incident Repository
- Modular Workflow Architecture
- Scalable Automation Design

---

## Technology Stack

| Category | Technology |
|----------|------------|
| Workflow Automation | n8n |
| Database | PostgreSQL |
| Artificial Intelligence | Google Gemini |
| Reporting | HTML + Gmail |
| Version Control | Git & GitHub |

---

## Workflow Architecture

The platform is designed as a collection of independent automation workflows that communicate through a centralized PostgreSQL database.

```
Security Alerts
        │
        ▼
Workflow 1
Alert Collection
        │
        ▼
PostgreSQL
        │
        ▼
Workflow 2
AI Classification
        │
        ▼
Workflow 3
Assignment & Escalation
        │
        ▼
Workflow 4
Dashboard Generation
        │
        ▼
Workflow 5
Scheduled Reporting
        │
        ▼
Email Notifications
```

---

# Implemented Workflows

## Workflow 1 — Security Alert Collection

Collects security alerts from external sources and stores them in a centralized PostgreSQL database for further processing.

---

## Workflow 2 — AI Threat Classification & Prioritization

Uses Google Gemini AI to analyze incoming incidents and determine:

- Threat Category
- Severity
- Priority
- Risk Score

---

## Workflow 3 — Incident Assignment & Escalation

Automatically assigns incidents to the appropriate response team based on severity and predefined business rules. Critical incidents can be escalated immediately.

---

## Workflow 4 — Security Dashboard & Reporting

Generates operational security metrics and prepares a structured dashboard summarizing the current security posture.

---

## Workflow 5 — Final Automation & Scheduling

Runs automatically on a scheduled basis, compiles the latest dashboard, and delivers an HTML email report to stakeholders.

---

# Repository Structure

```
SentinelAI/
│
├── assets/
├── config/
├── docs/
├── logs/
├── presentation/
├── scripts/
├── workflows/
└── README.md
```

---

## Highlights

- 5 Independent n8n Workflows
- 25+ Workflow Nodes
- AI-Powered Decision Making
- Scheduled Automation
- Database Logging
- Conditional Routing
- Automated HTML Reporting
- Production-Style Workflow Design

---

## Future Enhancements

- SIEM Platform Integration
- Microsoft Teams & Slack Notifications
- Interactive Web Dashboard
- Threat Intelligence Integration
- Automatic Ticket Creation (Jira/ServiceNow)
- Response Time Analytics

---

## Author

**Deepak Sharma**

Summer School 2026 – n8n Capstone Project

**Project Theme:** AI Cyber Security Incident Response Platform 