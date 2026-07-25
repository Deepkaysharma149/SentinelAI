# Stakeholders

## 1. Stakeholder Overview
This document identifies all individuals/groups who impact, or are impacted
by, SentinelAI's design, development, and operation.

## 2. Primary Stakeholders

### Security Analysts (Tier 1/2)
- **Role:** Investigate and resolve assigned incidents
- **Needs:** Low noise, high-confidence prioritization, clear incident context
- **Pain Point Addressed:** Alert fatigue, manual triage overhead

### Security Operations Manager
- **Role:** Oversees SOC performance and resource allocation
- **Needs:** Dashboards, SLA compliance metrics, team workload visibility
- **Pain Point Addressed:** Lack of real-time operational visibility

### Incident Response Team
- **Role:** Handles escalated, high-severity incidents
- **Needs:** Immediate, accurate escalation with full context
- **Pain Point Addressed:** Delayed escalation of critical threats

### Compliance / Audit Team
- **Role:** Ensures regulatory and policy adherence
- **Needs:** Immutable audit logs, complete incident history
- **Pain Point Addressed:** Poor documentation, audit gaps

## 3. Secondary Stakeholders

### End Users / Employees
- Indirectly affected (e.g., phishing/compromise targets); benefit from
  faster containment and reduced business disruption

### Executive Leadership
- **Role:** Budget owners, risk decision-makers
- **Needs:** High-level security posture reports and trend analysis

### Project Owner / Developer (You)
- **Role:** Designs, builds, and maintains SentinelAI
- **Needs:** Clear requirements, feasible architecture, iterative delivery

## 4. RACI Summary

| Activity                     | Analyst | SOC Manager | IR Team | Compliance | Developer |
|-------------------------------|:-------:|:-----------:|:-------:|:----------:|:---------:|
| Alert triage                  | R       | A           | C       | I          | I         |
| Incident escalation           | I       | A           | R       | I          | I         |
| System design & development   | I       | C           | I       | I          | R/A       |
| Reporting & audits             | I       | C           | I       | R          | A         |

*(R = Responsible, A = Accountable, C = Consulted, I = Informed)*