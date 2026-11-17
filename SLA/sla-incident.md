
 
 # 📊 SLA Example with Incident

[ Back to Overview] → [README.md](./README.md)

---

> **Lab Note:** This is an illustrative scenario, written to show how an SLA applies to a ticket from start to finish. The ticket number, names and times are examples. The targets come from the example table in [SLA Key Components](./sla-key-components.md).

## 📋 Summary

A worked example of one critical incident, from the moment the ticket is raised to the moment it is closed, with the SLA targets checked at each step.

---

## 🎫 Incident

| Field | Value |
|-------|-------|
| **Ticket ID** | INC-00891 |
| **Requestor** | Tom Baker, Finance Manager |
| **Category** | Network |
| **Priority** | 🔴 Critical |
| **Description** | The whole Finance department cannot access the network. 12 users are affected, and they cannot process the end-of-month payments |
| **Raised at** | Monday 7 September 2026, 08:45 |
| **Assigned to** | Seema, IT Support Tier 1 |

> **Why Critical?** The impact is high (12 users, a whole department) and the urgency is high (month-end payments are due). Impact plus urgency gives the priority.

---

## ⏱️ SLA Targets for This Ticket

| Target | Time allowed | Must be done by |
|--------|--------------|-----------------|
| **Response** (acknowledge the ticket) | 15 minutes | 09:00 |
| **Resolution** (fully fixed) | 2 hours | 10:45 |

---

## 🕒 Incident Timeline

| Time | Elapsed | What happened |
|------|:-------:|---------------|
| 🔵 **08:45** | 0 min | Tom Baker raises the ticket. 12 users cannot access the network. The SLA clock starts |
| 🟠 **08:52** | 7 min | **Response target met ✅** Seema acknowledges the ticket and starts investigating |
| 🟠 **09:05** | 20 min | Seema checks the network switch in the Finance area. It has lost power, because its power cable is disconnected |
| 🟠 **09:10** | 25 min | The power cable is reconnected. The switch restarts, and network connectivity is restored |
| 🟣 **09:15** | 30 min | Seema contacts Tom to confirm that all users can reach the network |
| 🟢 **09:20** | 35 min | Tom confirms that all 12 users are back online. **Resolution target met ✅** The ticket is marked resolved |
| ⚫ **09:25** | 40 min | The ticket is closed with the resolution note: *switch power cable reconnected* |

> **When does the resolution clock stop?** This example stops it when the user confirms the fix (09:20). Some SLAs stop it when the service is restored (09:10), and others at closure (09:25). The result is the same here, because every time is well inside the 2-hour target. Always check how your own SLA defines it.

---

## ✅ SLA Outcome

| SLA target | Required | Actual | Share of the target used | Result |
|------------|----------|--------|:------------------------:|:------:|
| **Response time** | 15 minutes | 7 minutes | 47% | ✅ Met |
| **Resolution time** | 2 hours | 35 minutes | 29% | ✅ Met |

No escalation was needed, because Tier 1 fixed the problem within the target.

---

## 📝 Ticket Notes

A good ticket records what was done, so the next technician can follow it.

| Field | Entry |
|-------|-------|
| **Cause** | The power cable of the Finance area switch was disconnected |
| **Action** | Reconnected the power cable, and the switch restarted |
| **Confirmation** | The requestor confirmed that all 12 users are online |
| **Follow-up** | Find out why the cable was disconnected. Secure the cable, and consider a UPS and tidier cabling to prevent it from happening again |

---

## ⚠️ What If the SLA Was Missed?

If the resolution had taken longer than 2 hours, the SLA would be **breached**. Possible consequences:

| Consequence | Meaning |
|-------------|---------|
| **Report to management** | The breach is recorded and reported |
| **Review meeting** | The team finds out why the target was missed and how to prevent it |
| **Service credits** | Credits may apply if the service is provided by an **outside company**. An internal help desk normally reports the breach instead |

A technician should not wait for a breach. A ticket that is close to its target should be escalated to Tier 2 or a manager, and the user should be told about the delay.

---

## 💡 Next Step

→ [Ticket Priority Levels](./ticket-priority-levels.md)
 
 

