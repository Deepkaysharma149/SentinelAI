# Workflow Architecture

## Overview
SentinelAI's automation is built as 5 modular n8n workflows, each responsible
for a distinct stage of the security incident lifecycle. This separation
ensures maintainability, easier debugging, and independent scalability.

## Workflow 1 — Security Alert Collection
**Purpose:** Ingest and normalize alerts from multiple security sources
(webhooks, APIs, email) into a consistent format stored in the `alerts` table.

## Workflow 2 — AI Threat Classification & Prioritization
**Purpose:** Send alert data to an AI/LLM model to determine severity
(Critical/High/Medium/Low), detect false positives, and enrich the alert
before incident creation.

## Workflow 3 — Incident Assignment & Escalation
**Purpose:** Convert classified alerts into incidents, auto-assign to the
appropriate analyst/team, and escalate unresolved critical incidents based
on SLA rules.

## Workflow 4 — Resolution Tracking & Notifications
**Purpose:** Track incident status changes (open → in-progress → resolved)
and trigger notifications (Email/Slack) to relevant stakeholders at each
stage.

## Workflow 5 — Security Dashboard & Incident Reports
**Purpose:** Aggregate data across all workflows to power a real-time
dashboard and generate periodic security reports (e.g., daily/weekly
summaries, SLA compliance, trend analysis).

## Workflow Interaction Summary