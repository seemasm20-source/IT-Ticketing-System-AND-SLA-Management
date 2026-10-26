# 🔄 Ticket Status Flow


Every ticket moves through these statuses from the moment it is raised until it is closed.


## Status Reference

| Status | Meaning | Who Acts Next |
|--------|---------|---------------|
| 🔵 New | Ticket just raised - not yet picked up | IT team assigns to a technician |
| 🟠 In Progress | Technician is actively working on the issue | Technician investigates and applies fix |
| 🟣 Pending User Response | Waiting for user to confirm fix worked | User must respond |
| 🔴 Escalated | Tier 1 cannot fix - passed to Tier 2 | Tier 2 or senior technician takes over |
| 🟢 Resolved | Issue fixed and confirmed by user | Technician closes the ticket |
| ⚫ Closed | Ticket complete - no further action | Ticket archived |

---

## Status Flow Example - Incident INC-00452

> 🔵 **09:15 — New** Sarah Jones raises ticket: "Outlook will not open"
>
> 🟠 **09:20 — In Progress** John picks up ticket, runs ScanPST on OST file
>
> 🟣 **09:45 — Pending User Response** Fix applied — John asks Sarah to confirm
>
> 🟢 **10:00 — Resolved** Sarah confirms Outlook is working
>
> ⚫ **10:05 — Closed** John closes ticket with resolution notes
