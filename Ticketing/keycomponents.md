# 📋 Key Components of a Ticket

[ Back to README] → [README](https://github.com/seemasm20-source/IT-Ticketing-System-AND-SLA-Management/blob/main/README.md)

---

## 📋 Summary

Every ticket holds the same core fields, whichever ticketing tool is used. The fields tell the next technician what the problem is, who is affected, how urgent it is, what has been done and where it stands. A ticket with complete, clear fields is solved faster, and the SLA times in it are accurate.

---

## 🗂️ Ticket Fields

| Field | Description | Example |
|-------|-------------|---------|
| **Ticket ID** | A unique reference number, assigned automatically | INC-00452 |
| **Requestor** | The user who raised the ticket, with contact details | Sarah Jones, HR |
| **Ticket type** | Incident, service request, problem or change | Incident |
| **Category** | The area the issue is in. See [Ticket Category List](./ticket-category-list.md) | Software |
| **Priority** | How urgent the ticket is, set from its impact and urgency. The priority decides the SLA response and resolution times | High |
| **Assigned to** | The technician or team responsible for the ticket | John Smith, IT Support |
| **Status** | The current stage of the ticket. See [Ticket Status Flow](./ticket-status-flow.md) | In Progress |
| **Description** | The details of the issue | "Outlook will not open since this morning" |
| **Created date** | When the ticket was raised | 2026-09-07 09:15 |
| **Resolution** | What was done to fix the issue | A faulty add-in was turned off, and Outlook opens normally |

### Other Fields You Often See

| Field | What it holds |
|-------|---------------|
| **Impact and urgency** | The two values that set the priority |
| **Affected asset or location** | The computer, the application or the office involved |
| **Contact details** | How to reach the user, such as a phone number |
| **Assignment group** | The team that owns the ticket, such as the Tier 2 queue |
| **Notes or work log** | Every action taken and every message to the user, with times |
| **Attachments** | Screenshots or error messages |
| **SLA target and due time** | When the response and resolution are due |
| **Resolved and closed dates** | When the ticket was fixed and closed |

---

## 🎫 Sample Ticket

| Field | Value |
|-------|-------|
| **Ticket ID** | INC-00452 |
| **Requestor** | Sarah Jones, HR |
| **Ticket type** | Incident |
| **Category** | Software |
| **Priority** | 🟠 High |
| **Assigned to** | John Smith, IT Support Tier 1 |
| **Status** | 🟠 In Progress |
| **Created** | 2026-09-07 09:15 |
| **Description** | Outlook will not open since this morning. It closes at startup, with no error message |

> The same ticket is followed from start to finish in [Ticket Status Flow](./ticket-status-flow.md), and the resolution is recorded there.




---







