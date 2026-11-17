
# 🚦 Ticket Priority Levels

[ Back to README] → [README](https://github.com/seemasm20-source/IT-Ticketing-System-AND-SLA-Management/blob/main/README.md)

---

## 📋 Summary

**Priority** decides how quickly a ticket must be responded to and resolved. It is set from the ticket's **impact** and **urgency**, and it decides which SLA times apply. This file lists the priority levels, shows how to choose one, and gives examples.

---

## 🗂️ Priority Reference

| Priority | Meaning | Response time | Resolution time | Example |
|----------|---------|---------------|-----------------|---------|
| 🔴 **Critical (P1)** | The business is stopped, or a critical service is down. Many users are affected | 15 minutes | 2 hours | A server is down. A full network outage. All staff cannot work |
| 🟠 **High (P2)** | A major function is not working, or a team or an important user cannot do their job, and there is no workaround | 1 hour | 8 hours | A manager cannot reach email. A remote worker has no VPN and cannot work |
| 🟡 **Medium (P3)** | One user is affected, or users can still work in part. A workaround exists | 4 hours | 24 hours | Outlook syncs slowly but works. The printer is down, but the user can send the file by email |
| 🟢 **Low (P4)** | A minor issue or a simple request. No business impact, and it can wait | 24 hours | 72 hours | A desktop wallpaper change request. A mouse that double-clicks now and then |

> The times are an **example**, and they match [SLA Key Components](./sla-key-components.md). Every organisation sets its own, and many SLAs count the time only during support hours.

---

## 🔍 How Priority is Decided

| Factor | Question | Levels |
|--------|----------|--------|
| **Impact** | How many people are affected, and how badly? | High: many users, a whole department or a critical service. Medium: a team, or one important user. Low: one user |
| **Urgency** | How soon must it be fixed? | High: work has stopped, or a deadline is close, with no workaround. Medium: work is slowed. Low: it can wait |

**Impact + Urgency = Priority**

### Priority Matrix

| | **Urgency: High** | **Urgency: Medium** | **Urgency: Low** |
|---|:-----------------:|:-------------------:|:----------------:|
| **Impact: High** | 🔴 Critical | 🟠 High | 🟡 Medium |
| **Impact: Medium** | 🟠 High | 🟡 Medium | 🟢 Low |
| **Impact: Low** | 🟡 Medium | 🟢 Low | 🟢 Low |

> This matrix is an example. Organisations adjust it. Check the one your help desk uses.

---

## 🎫 Worked Examples

| Situation | Impact | Urgency | Priority |
|-----------|--------|---------|----------|
| The whole Finance department has no network, and month-end payments are due | High | High | 🔴 Critical |
| A manager cannot read email before an important meeting | Medium | High | 🟠 High |
| One user cannot print, but can email the file | Low | Medium | 🟢 Low |
| One user's Outlook is slow, but works | Low | Low | 🟢 Low |
| A user asks for a new wallpaper | Low | Low | 🟢 Low |

The first example is the one in [SLA Example with Incident](./sla-example-incident.md).

---

## ⚠️ Setting the Priority Correctly

- **Do not take the user's word alone.** Every user thinks their issue is urgent. Ask who is affected and what cannot be done.
- **Ask about a workaround.** If the user can still work, the priority is lower.
- **Change it when you learn more.** A ticket that looked like one user can turn out to affect a whole team, and the priority should go up. Record why you changed it.
- **Security overrides.** A suspected phishing attack, malware or a possible account compromise goes to the security team at once, whatever the matrix says. See [Ticket Category List](./ticket-category-list.md).
- **Special cases are set by policy.** Some organisations raise the priority for certain users or systems, such as executives or payroll at month end. Follow your organisation's rule, and do not decide it on your own.
- **Do not lower a priority to avoid a breach.** The SLA time follows the real priority.

---

## 💡 Next Step

→ [Escalation Process](./escalation-process.md)

















