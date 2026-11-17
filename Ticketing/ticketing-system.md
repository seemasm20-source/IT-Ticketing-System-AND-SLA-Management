
# 🎫 What is a Ticketing System?

[ Back to README] → [README](https://github.com/seemasm20-source/IT-Ticketing-System-AND-SLA-Management/blob/main/README.md)

---

## 📋 Summary

A **ticketing system** is software that turns every user complaint, request or incident into a **ticket**: a unique record with an ID number that follows the issue through its whole life, until it is resolved and closed. It is the main tool of an IT Help Desk Tier 1 and Tier 2 technician, and the place where SLA times are measured.

---

## 💡 Why a Ticketing System is Used

| Reason | Explanation |
|--------|-------------|
| **Tracks every issue** | Nothing gets lost, because every request has a record |
| **Prioritises work** | Critical issues are handled before low-priority ones |
| **Accountability** | Every ticket is assigned to a specific technician or team |
| **Communication** | The user is kept up to date on the status of their issue |
| **Reporting** | Management can see how many tickets were resolved and how fast |
| **Measures the SLA** | The ticket records the times the SLA targets are checked against |
| **Builds knowledge** | Past tickets and their solutions help solve the same problem faster next time |

---

## 🗂️ Types of Tickets

| Type | Meaning | Example |
|------|---------|---------|
| **Incident** | Something is broken or not working as it should | "I cannot sign in to Outlook" |
| **Service request** | A user asks for something standard | "I need a new user account" or "I need access to a shared folder" |
| **Problem** | The root cause of one or more repeated incidents | Many users lose the VPN every morning, and the cause is found and fixed |
| **Change** | A planned change to a system | Upgrading a server or changing a firewall rule |

> A technician works mostly with **incidents** and **service requests**. **Problems** and **changes** are usually handled by Tier 2 or other teams, with an approval step for changes.

---

## 📝 What a Ticket Contains

| Field | What it holds |
|-------|---------------|
| **Ticket ID** | A unique number, for example `INC-00891` |
| **Requestor** | The user who reported the issue, and their contact details |
| **Category** | The type of issue, for example Network, Email or Hardware |
| **Priority** | How urgent the ticket is (impact and urgency) |
| **Status** | Where the ticket stands, for example New, In Progress, Resolved |
| **Description** | What the problem is, and what the user sees |
| **Assigned to** | The technician or team working on it |
| **Timestamps** | When the ticket was raised, responded to and resolved, for the SLA |
| **Notes and updates** | Every action taken, and every message to the user |
| **Resolution** | How the problem was fixed |

---

## 🔄 Ticket Lifecycle (Overview)

```text
New → Assigned → In Progress → (Waiting for user) → Resolved → Closed
```

| Stage | What happens |
|-------|--------------|
| **New** | The ticket is logged, by the user, by email, by phone or by a monitoring tool |
| **Assigned** | The ticket gets a priority and goes to a technician or team |
| **In progress** | The technician investigates and works on the fix |
| **Waiting for user** | The technician needs information from the user. In many systems, the SLA clock pauses |
| **Resolved** | The fix is done and the user is told |
| **Closed** | The user confirms the fix, or the ticket closes automatically after a set time |

---

## 🛠️ Common Ticketing Tools

| Tool | Notes |
|------|-------|
| **ServiceNow** | Widely used in large enterprises |
| **Jira Service Management** | Common in technical and software teams |
| **Zendesk** | Popular for customer support, also used for IT |
| **Freshdesk** (Freshservice for IT) | Cloud help desk for small and medium teams |
| **ManageEngine ServiceDesk Plus** | Common in IT departments of all sizes |
| **Spiceworks Cloud Help Desk** | A free option for small IT teams |

> The tools look different, but they all work the same way: a ticket with an ID, a priority, a status and a history. If you learn one, you can quickly learn another.

---

## 💡 Next Step

→ [Ticket Lifecycle](./ticket-lifecycle.md)



