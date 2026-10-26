
 📊 SLA Example with Incident


A real-world example showing how SLA applies to a complete incident from ticket raised to ticket closed.


## Incident

| Field | Value |
|-------|-------|
| Ticket ID | INC-00891 |
| Requestor | Tom Baker - Finance Manager |
| Category | Network |
| Priority | 🔴 Critical |
| Description | Entire Finance department cannot access network - 12 users affected. Cannot process end-of-month payments. |
| Raised At | Monday 07/09/2026 - 08:45 |
| Assigned To | Seema - IT Support Tier 1 |

---

## SLA Targets for This Ticket

| Target | Required By |
|--------|------------|
| Response (acknowledge) | 09:00 - within 15 minutes |
| Resolution (fully fixed) | 10:45 - within 2 hours |

---

## Incident Timeline

> 🔵 **08:45** — Tom Baker raises ticket. 12 users cannot access network.
>
> 🟠 **08:52** — **SLA Response met ✅** Seema acknowledges ticket. Begins investigation.
>
> 🟠 **09:05** — Seema checks switch in Finance area. Finds switch has lost power — cable disconnected.
>
> 🟠 **09:10** — Power cable reconnected. Switch reboots. Network connectivity restored.
>
> 🟣 **09:15** — Seema contacts Tom to confirm all users can access network.
>
> 🟢 **09:20** — Tom confirms all 12 users back online.
>
> ⚫ **09:25** — **SLA Resolution met ✅** Ticket closed. Resolution: switch power cable reconnected.

---

## SLA Outcome

| SLA Target | Required | Actual | Result |
|------------|---------|--------|--------|
| Response Time | 15 minutes | 7 minutes | ✅ Met |
| Resolution Time | 2 hours | 35 minutes | ✅ Met |

---

## What if SLA was Missed?

If the resolution had taken longer than 2 hours the SLA would be breached.
Consequences could include a service credit issued to the Finance department, a report generated for management and a review meeting to understand why the target was missed and how to prevent it.
