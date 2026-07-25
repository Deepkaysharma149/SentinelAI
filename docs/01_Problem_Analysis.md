# Problem Analysis

## 1. Background
Modern organizations deploy dozens of security tools — firewalls, SIEM
platforms, endpoint detection (EDR), intrusion detection systems (IDS), cloud
security monitors — each generating a continuous stream of alerts. Industry
research shows a mid-sized SOC (Security Operations Center) can receive
10,000+ alerts per day, of which up to 45% are false positives. Analysts
cannot manually triage this volume, resulting in "alert fatigue" — a state
where genuine threats get buried under noise.

## 2. Problem Statement
> Security teams lack an automated, intelligent system to collect, classify,
> prioritize, and track security alerts end-to-end — leading to delayed
> incident response, missed critical threats, and inefficient use of analyst
> time.

## 3. Root Cause Analysis

| Root Cause                          | Consequence                                      |
|--------------------------------------|---------------------------------------------------|
| No unified alert intake pipeline     | Alerts scattered across disconnected tools         |
| No automated severity classification | Analysts manually read every alert                |
| No rule-based/AI-based prioritization| Critical threats treated same as low-risk noise    |
| No SLA-based escalation              | Unresolved critical incidents go unnoticed         |
| No centralized incident history      | Poor audit trail, repeated investigation effort    |

## 4. Quantifiable Impact
- **Mean Time to Detect (MTTD)** and **Mean Time to Respond (MTTR)** increase
  significantly when triage is manual.
- Analyst productivity drops due to time spent on false positives.
- Increased breach risk: delayed response windows are directly correlated
  with higher breach cost (per industry breach-cost reports, e.g. IBM's
  annual Cost of a Data Breach studies).
- Compliance risk from inconsistent incident documentation.

## 5. Why Automation + AI Is the Right Approach
Rule-based systems alone cannot adapt to evolving attack patterns and produce
high false-positive rates. An AI/LLM-based classification layer, combined with
workflow automation (n8n), can:
- Understand alert context/content, not just static rules
- Continuously prioritize based on severity and business impact
- Free analysts to focus only on real, high-priority threats

## 6. Conclusion
This project (SentinelAI) addresses the above gaps by building an end-to-end
automated pipeline: **Alert Collection → AI Classification → Incident
Assignment → Escalation → Resolution Tracking → Reporting.**  
