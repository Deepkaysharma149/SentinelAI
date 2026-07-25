# Business Context

## 1. Project Name
**SentinelAI** — AI-Powered Security Operations Automation Platform

## 2. Business Problem
Security Operations Centers (SOCs) are overwhelmed by alert volume and lack
automated intelligence to separate real threats from noise. This results in
slow response times, analyst burnout, and increased organizational risk
exposure.

## 3. Proposed Solution Overview
SentinelAI automates the full security incident lifecycle:

| Stage | Function |
|-------|----------|
| Collection | Ingests alerts from multiple security sources automatically |
| Classification | AI evaluates severity, context, and legitimacy of each alert |
| Assignment | Routes incidents to the right analyst/team automatically |
| Escalation | Enforces SLA-based escalation for unresolved critical incidents |
| Tracking | Maintains full incident lifecycle and audit trail |
| Reporting | Real-time dashboard and periodic security reports |

## 4. Business Value Proposition

| Value Driver | Benefit |
|---------------|---------|
| Speed | Reduces Mean Time to Respond (MTTR) via automation |
| Accuracy | AI-driven prioritization reduces false-positive handling |
| Cost Efficiency | Reduces analyst hours spent on manual triage |
| Visibility | Centralized dashboard for leadership & compliance |
| Scalability | Workflow-based architecture scales with alert volume |

## 5. Target Market / Users
- Small-to-mid-sized organizations without large dedicated SOC teams
- IT Security teams looking to automate Tier-1 triage
- Compliance-driven industries (finance, healthcare, SaaS) needing audit trails

## 6. Competitive Context
Enterprise SOAR (Security Orchestration, Automation & Response) platforms
(e.g., Splunk SOAR, Palo Alto XSOAR) exist but are expensive and complex.
SentinelAI targets a lightweight, workflow-automation-based (n8n) alternative
that is faster to deploy and more cost-effective for smaller teams.

## 7. Project Scope
**In Scope:**
- Alert ingestion workflow
- AI-based classification & prioritization
- Incident assignment/escalation logic
- PostgreSQL-based incident database
- Notification system (Email/Slack)
- Reporting dashboard

**Out of Scope (Phase 1):**
- Direct remediation/auto-blocking of threats
- Multi-tenant enterprise deployment
- Native SIEM tool development (SentinelAI integrates with existing tools)