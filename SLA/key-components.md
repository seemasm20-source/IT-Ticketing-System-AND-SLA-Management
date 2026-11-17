





# 📋 SLA Key Components

[ Back to Overview] → [README.md](./README.md)

---

## 📋 Summary

An SLA is built from a few key components: how fast a ticket gets a response, how fast it is resolved, how its priority is decided, when it is escalated, when support is available, and what happens when a target is missed. This file explains each component with an example. For the definition of an SLA, see [What is a Service Level Agreement](./what-is-sla.md).

---

## 🧩 Components

| Component | Definition | Example |
|-----------|------------|---------|
| **Response time** | How quickly IT must acknowledge the ticket and start work | Critical: 15 minutes. High: 1 hour |
| **Resolution time** | How quickly the problem must be fully fixed | Critical: 2 hours. High: 8 hours |
| **Ticket prioritisation** | The rules for giving a ticket the correct priority, based on **impact** (how many are affected) and **urgency** (how fast it must be fixed) | A server down for all users = Critical. One user who cannot work = Medium, or High if the user or the function is business-critical |
| **Escalation process** | When and how a ticket is passed to a higher tier or a manager | Tier 1 cannot resolve the ticket within its agreed time, or the ticket is close to breaching → escalate to Tier 2 |
| **Support hours (service availability)** | The hours IT support is available, and the cover for critical issues | Monday to Friday, 08:00 to 18:00. Critical tickets 24/7 |
| **Penalties and consequences** | What happens when a target is missed | A report to management and a review. With an outside provider, service credits may also apply |

---

## ⏱️ SLA Response and Resolution Times

| Priority | Response time | Resolution time |
|----------|---------------|-----------------|
| 🔴 **Critical** | 15 minutes | 2 hours |
| 🟠 **High** | 1 hour | 8 hours |
| 🟡 **Medium** | 4 hours | 24 hours |
| 🟢 **Low** | 24 hours | 72 hours |

> These times are an **example**. Every organisation sets its own. Many SLAs count the time only during **support hours**, so a Medium ticket logged at 17:00 on Friday does not breach on Saturday. Critical tickets are often counted around the clock.

---

## 🔍 How the Components Work Together

| Step | What happens | Component |
|:----:|--------------|-----------|
| 1 | The user reports a problem, and a ticket is logged | |
| 2 | The technician gives the ticket a priority from its impact and urgency | Ticket prioritisation |
| 3 | The response clock starts, and the technician acknowledges the ticket in time | Response time |
| 4 | The technician works on the fix, and updates the ticket | Resolution time |
| 5 | If the fix cannot be made in time, the ticket is escalated | Escalation process |
| 6 | If a target is missed, it is recorded and reported | Penalties and consequences |

---

## 💡 Next Step

→ [Ticket Priority Levels](./ticket-priority-levels.md)






















# 📋 SLA Key Components



## Components

| Component | Definition | Example |
|-----------|------------|--------|
| **Response Time** | How quickly IT must acknowledge the ticket | Critical: 15 mins. High: 1 hour. |
| **Resolution Time** | How quickly the issue must be fully fixed | Critical: 2 hours. High: 8 hours. |
| **Ticket Prioritisation** | Rules for assigning correct priority | Server down = Critical. One user = High. |
| **Escalation Process** | When and how to pass ticket to higher tier | Tier 1 cannot resolve in 1 hour → escalate to Tier 2 |
| **Service Availability** | Hours IT support is available | Mon–Fri 08:00–18:00. Critical 24/7. |
| **Penalties and Consequences** | What happens if SLA targets are missed | Service credits issued. Management report generated. |

---

## SLA Response and Resolution Times

| Priority | Response Time | Resolution Time |
|----------|--------------|----------------|
| 🔴 Critical | 15 minutes | 2 hours |
| 🟠 High | 1 hour | 8 hours |
| 🟡 Medium | 4 hours | 24 hours |
| 🟢 Low | 24 hours | 72 hours |
