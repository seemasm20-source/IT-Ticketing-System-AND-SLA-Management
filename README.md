# 🎫 SLA Management and Ticketing Portfolio

**Portfolio:** IT Help Desk Tier 1 & Tier 2 - Service Management

**Tool:** Ticketing system concepts (ServiceNow, Jira Service Management, Freshservice, ManageEngine ServiceDesk Plus, Spiceworks Cloud Help Desk)

**Purpose:** Demonstrate how an IT Help Desk logs, prioritises, tracks and resolves tickets within agreed service levels, for IT Help Desk Tier 1 and Tier 2 roles

**Author:** Seema Soapanahalli Mallikarjunaiah

**Date:**  October 2026 
---

## 📌 Objective

This portfolio explains how a help desk works day to day, How a ticket is raised, categorised, prioritised and tracked, how Service Level Agreements (SLAs) set the response and resolution times, and how a technician records the work.

The objective of this portfolio is to demonstrate:

- Understanding of what an SLA is and what its components are
- Setting a ticket's category and priority from its impact and urgency
- Following a ticket through its statuses and measuring it against SLA targets
- Writing clear tickets, investigation notes and resolution notes
- Knowing when a Tier 1 technician escalates to Tier 2
- Working through realistic sample tickets, linked to the technical labs in my other portfolios

> **Lab Note:** The tickets, names, times and SLA targets in this portfolio are **illustrative examples**, written to show the method. They are not real company tickets. Every organisation sets its own priorities, times and status names.

---

## 💡 How a Ticket Flows

```text
User reports a problem
        ↓
Ticket logged  →  Category and priority set  →  SLA clock starts
        ↓
Tier 1: respond → investigate → fix → confirm with the user
        ↓                         ↘ cannot fix in time → escalate to Tier 2
Resolved  →  Closed, with a resolution note
```

| Concept | In one line |
|---------|-------------|
| **Ticket** | A record with a unique ID that follows an issue from start to finish |
| **Category** | The area of the issue, such as Network or Software |
| **Priority** | How urgent it is, from impact and urgency |
| **SLA** | The agreed response and resolution times for each priority |
| **Status** | Where the ticket stands, and who acts next |
| **Escalation** | Passing the ticket to a higher tier before it breaches |

---

## 📁 Portfolio Structure

| Section | Topic | Key Skills |
|---------|-------|------------|
| **Section 1** | SLA Fundamentals | What an SLA is, its components, a worked incident |
| **Section 2** | Ticketing System Fundamentals | Ticket types, fields, statuses, categories, priorities |
| **Section 3** | Sample Tickets | Account lockout, mailbox not found |

---

## 📜 Section 1 - SLA Fundamentals

| Topic | What it covers | File |
|-------|----------------|------|
| **What is a Service Level Agreement (SLA)?** | The definition, key terms, SLA vs OLA vs UC, and the Tier 1 and Tier 2 roles | [What is an SLA?](./what-is-sla.md) |
| **SLA Key Components** | Response time, resolution time, prioritisation, escalation, support hours, penalties | [SLA Key Components](./sla-key-components.md) |
| **SLA Example with Incident** | One critical ticket measured against its SLA targets, from raised to closed | [SLA Example with Incident](./sla-example-incident.md) |

---

## 🎫 Section 2 - Ticketing System Fundamentals

| Topic | What it covers | File |
|-------|----------------|------|
| **What is a Ticketing System?** | Why tickets are used, ticket types, the lifecycle, common tools | https://github.com/seemasm20-source/IT-Ticketing-System-AND-SLA-Management/blob/main/Ticketing/ticketing-system.md |
| **Key Components of a Ticket** | The ticket fields, a sample ticket, and how to write a good ticket | [Key Components](https://github.com/seemasm20-source/IT-Ticketing-System-AND-SLA-Management/blob/main/Ticketing/keycomponents.md) |
| **Ticket Status Flow** | The statuses, who acts next, the flow, and the SLA clock | [Ticket Status Flow](https://github.com/seemasm20-source/IT-Ticketing-System-AND-SLA-Management/blob/main/Ticketing/ticket-status-flow.md) |
| **Ticket Category List** | The categories, how to choose one, and subcategories | [Category List](https://github.com/seemasm20-source/IT-Ticketing-System-AND-SLA-Management/blob/main/Ticketing/categorylist.md) |
| **Ticket Priority Levels** | The priority levels, the impact and urgency matrix, worked examples | [Priority Levels](https://github.com/seemasm20-source/IT-Ticketing-System-AND-SLA-Management/blob/main/Ticketing/priority-levels.md)|

---

## 🧪 Section 3 - Sample Tickets

Each sample ticket follows the same layout: ticket details, the user's message, investigation notes, a resolution note and screenshots.

| Sample ticket | Category | Cause | Linked technical lab |
|---------------|----------|-------|----------------------|
| **User Account Locked After Failed Sign-In Attempts** | Account and Access | Too many wrong passwords | [Unlock a User Account](./unlock-user-account.md), [Event ID 4740](./event-id-4740.md) |
| **Outlook Desktop App: Mailbox Not Found** | Software (Outlook) | No Exchange Online licence | [Assign and Remove Licences](./assign-remove-licences.md), [Corrupted Outlook Profile](./outlook-corrupted-profile.md) |

| File | Description |
|------|-------------|
| [Sample Ticket - Account Locked](./sample-ticket-account-locked.md) | Verify the user, find the cause, unlock the account, prevent a repeat |
| [Sample Ticket - Mailbox Not Found](./sample-ticket-mailbox-not-found.md) | Test the web version, check the licence, assign it, confirm the mailbox |

---

## ⏱️ SLA Targets and Priority Levels (Example)

| Priority | Response time | Resolution time | Example |
|----------|---------------|-----------------|---------|
| 🔴 **Critical (P1)** | 15 minutes | 2 hours | A server is down. A full network outage |
| 🟠 **High (P2)** | 1 hour | 8 hours | A manager cannot reach email, and there is no workaround |
| 🟡 **Medium (P3)** | 4 hours | 24 hours | One user is affected, or a workaround exists |
| 🟢 **Low (P4)** | 24 hours | 72 hours | A minor issue or a simple request |

**Impact + Urgency = Priority.** These times are an example. Many SLAs count the time only during support hours.

---

## 🔄 Ticket Statuses

| Status | Meaning | Who acts next |
|--------|---------|---------------|
| 🔵 **New** | Just raised | The IT team assigns it |
| 🔵 **Assigned** | Given to a technician or team | The technician picks it up |
| 🟠 **In Progress** | Being worked on | The technician |
| 🟣 **Pending User Response** | Waiting for the user, often with the SLA clock paused | The user |
| 🟡 **On Hold** | Blocked, for example waiting for a part or approval | Whoever it waits for |
| 🔴 **Escalated** | Passed to Tier 2 or a senior technician | Tier 2 |
| 🟢 **Resolved** | Fixed, and the user was told | Closed by confirmation or automatically |
| ⚫ **Closed** | Complete | Nobody |
| 🔁 **Reopened** | The problem came back | The technician |

---

## 📂 Ticket Categories

| Category | Examples |
|----------|----------|
| **Hardware** | A broken screen, a printer that does not print |
| **Software** | Outlook will not open, Teams crashes |
| **Network** | VPN, Wi-Fi, no internet, shared drive not reachable |
| **Security** | Phishing, malware, unusual sign-in activity |
| **Account and Access** | Password reset, locked account, new user, permissions, licence |
| **Other** | An issue that fits no category |

---

## 🛠️ Tools and Concepts Used

| Tool or concept | Purpose |
|-----------------|---------|
| **Ticketing system** | Logging and tracking tickets (ServiceNow, Jira Service Management, Freshservice and others) |
| **SLA targets** | Measuring response and resolution times |
| **Impact and urgency matrix** | Setting priority |
| **Ticket notes and resolution notes** | Recording every action for the next technician |
| **Active Directory Users and Computers** | Account checks in the lockout ticket |
| **Microsoft 365 Admin Center** | Licence checks in the mailbox ticket |
| **Event Viewer** | Finding the cause of a lockout (Event ID 4740) |

---

## 📚 Skills Demonstrated

- Explaining an SLA, its components and the difference between response and resolution time
- Setting priority from impact and urgency, and not from the user's wording alone
- Choosing the right category, and updating it when the real cause is found
- Following a ticket through its statuses, and understanding the SLA clock
- Writing a clear ticket: the problem, the evidence, every action and the resolution
- Deciding when to escalate, and passing a ticket on with the details collected
- Verifying a user's identity before a password reset or an unlock
- Linking a ticket to the technical fix in the Active Directory and Microsoft 365 labs
- Technical documentation for a GitHub portfolio

---

## 🎯 Real-World Help Desk Tickets

| Caller Complaint | Category | Cause | Fix Applied |
|------------------|----------|-------|-------------|
| "My account is locked" | Account and Access | Too many wrong passwords | Verified identity, unlocked the account, checked for the source |
| "Outlook says the mailbox cannot be found" | Software | No Exchange Online licence | Tested the web version, assigned a licence, confirmed the mailbox |
| "The whole Finance department has no network" | Network | A switch lost power | Reconnected the cable, confirmed with the users (worked example) |
| "Outlook will not open" | Software | A faulty add-in | Started in safe mode, turned the add-in off (status flow example) |

---



## 🎓 Learning Outcome

This portfolio showed how service management works around the technical fixes. It built practical skills for the daily work of an IT Help Desk: setting the right priority, working to an SLA, writing notes that another technician can follow, and escalating in time. These skills are relevant to IT Help Desk Tier 1 and Tier 2 roles.

---

## ✅ Conclusion

SLA fundamentals, the ticketing system, its fields, statuses, categories and priorities were documented, and two sample tickets were worked from start to finish.

Together these show a systematic approach to support: log the ticket with the right priority, work to the SLA target, fix and confirm with the user, document what was done, and escalate when the target is at risk.

