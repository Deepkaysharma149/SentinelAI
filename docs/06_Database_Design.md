# Database Design

## 1. Database Engine
**PostgreSQL** — chosen for reliability, strong support for structured
relational data, JSON fields (for flexible alert payloads), and native
integration with n8n.

## 2. Core Tables (Overview)

| Table | Purpose |
|-------|---------|
| `alerts` | Stores raw/normalized incoming security alerts |
| `incidents` | Stores classified, trackable incidents derived from alerts |
| `users` | Stores analysts/team members for assignment |
| `notifications` | Logs all notifications sent (Email/Slack) |
| `audit_logs` | Immutable log of all system actions for traceability |

## 3. Table Relationships (High-Level)
- One `alert` → generates one `incident` (1:1 or 1:many if grouped)
- One `incident` → assigned to one `user`
- One `incident` → can trigger multiple `notifications`
- Every action across tables → recorded in `audit_logs`

## 4. Notes
Detailed column-level schema (data types, primary/foreign keys, constraints)
will be designed in the next phase, once workflow requirements are finalized
during n8n implementation.