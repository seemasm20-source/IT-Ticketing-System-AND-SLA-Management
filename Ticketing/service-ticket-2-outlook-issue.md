
# 🎫 Sample Ticket - Outlook Desktop App: Mailbox Not Found Error

[ Back to Overview] → [README.md](./README.md)

---

> **Lab Note:** This is an illustrative ticket, written to show how a "mailbox not found" error is investigated from start to finish. The names, the contact details and the user's message are examples. The technical steps match the Microsoft 365 labs in this portfolio.

## 📋 Summary

A user opens Outlook and gets the error "We couldn't find the mailbox for this account". The technician verifies the user's identity, checks whether the mailbox works in Outlook on the web, finds that the user has no Exchange Online licence, assigns it, and confirms that the mailbox opens in Outlook.

---

## 🎫 1. Ticket Details

| Field | Value |
|-------|-------|
| **Ticket subject** | Unable to access Outlook desktop app - mailbox not found error |
| **Username** | Seema |
| **Contact number** | *(hidden)* |
| **Email address** | *(hidden)* |
| **Ticket type** | Incident |
| **Category** | Software (Outlook) |
| **Priority** | 🟠 High |
| **SLA targets** | Response: 1 hour. Resolution: 8 hours (example SLA, see [SLA Key Components](./sla-key-components.md)) |

> **Why High?** The user cannot read any email, and there is no workaround in the desktop app. Only one user is affected, so some organisations would set Medium. Follow your organisation's priority rule. See [Ticket Priority Levels](./ticket-priority-levels.md).
>
> **Category:** The ticket is logged by its symptom (Outlook). Once the cause is a missing licence, many help desks change the category to **Account and Access**, so the reports stay accurate. See [Ticket Category List](./ticket-category-list.md).

---

## 💬 2. User-Reported Issue

> Hi IT Support,
>
> I am unable to access my mailbox through the Outlook desktop app. When I open Outlook, I receive the following error message:
>
> *"Something went wrong. We couldn't find the mailbox for this account."*
>
> I am unable to access my emails through the Outlook desktop application and I need access to continue my work.
>
> Could you please investigate and help me resolve this issue?
>
> Thank you.

---

## 🔎 3. Investigation Notes

| Step | Action | Result |
|:----:|--------|--------|
| 1 | **Verified the user's identity** with the approved procedure before any change | Identity confirmed |
| 2 | **Confirmed the symptom:** the same error appears when Outlook opens | The error is confirmed |
| 3 | **Tested Outlook on the web** (`outlook.office.com`) with the same account | The mailbox does not open there either, so the fault is the mailbox or the licence, not the Outlook app |
| 4 | **Checked the account** in the Microsoft 365 Admin Center: **Users → Active users →** the user. Sign-in is not blocked, and the account is active | The account is fine |
| 5 | **Checked the licence:** **Licenses and apps** tab | No licence that includes **Exchange Online** is assigned |
| 6 | **Assigned a licence** that includes Exchange Online, with the user's **location** set, and clicked **Save changes** | The licence is assigned |
| 7 | **Waited for the mailbox to be created.** A new mailbox needs some time after the licence is assigned. Checked the mailbox in the Exchange admin center: **Recipients → Mailboxes** | The mailbox is listed |
| 8 | **Asked the user** to close and reopen Outlook, and to try again | The mailbox opens |

> The details of the licence steps are in [Assign and Remove Licences](./assign-remove-licences.md).

---

## ✅ 4. Resolution and Closure Note

| Field | Entry |
|-------|-------|
| **Cause** | The user had no Exchange Online licence, so no mailbox existed for the account |
| **Action** | The identity was verified. A licence that includes Exchange Online was assigned in the Admin Center. The mailbox was created |
| **Confirmation** | The user opened the mailbox in the Outlook desktop app and in Outlook on the web |
| **Final status** | Resolved, then Closed after the user confirmed |

---

## 🛠️ If the Error Continues

| Check | What to do |
|-------|-----------|
| **The mailbox is not there yet** | Wait a little longer, and check again. It can take time, and sometimes longer than expected. If it never appears, escalate to Tier 2 or the Exchange administrator |
| **Outlook still shows the error, but webmail works** | The Outlook profile is holding old information. Restart Outlook, then remove and add the account again, or create a new profile. See [Corrupted Outlook Profile](./outlook-corrupted-profile.md) |
| **Wrong account in Outlook** | Check **File → Office Account**. See [Outlook Sign-In and Profile Troubleshooting](./outlook-sign-in-profile.md) |
| **The licence does not include Exchange Online** | Some licences, such as Teams-only licences, have no mailbox. Assign one that includes Exchange Online |
| **A recently restored user** | A restored user returns without a licence. See [Delete and Restore a User](./delete-restore-user-m365.md) |
| **Hybrid or on-premises mailbox** | If the organisation has on-premises Exchange, the mailbox may live there, and an administrator must check it |

---

## 🖼️ Screenshots

**Screenshot: the mailbox error in Outlook:**

<img width="1920" height="1080" alt="Outlook showing the error that the mailbox for this account could not be found" src="https://github.com/user-attachments/assets/ef848193-3777-4af9-bd4f-a62e9ebb21d4" />

**Screenshot: licence assigned in the Admin Center:**

<img width="1920" height="1080" alt="Microsoft 365 Admin Center Licenses and apps tab with an Exchange Online licence assigned" src="https://github.com/user-attachments/assets/ccb66b70-23be-4394-b412-f2488b368ac1" />

**Screenshot: mailbox working in Outlook:**

<img width="1920" height="1080" alt="Outlook open with the mailbox loaded after the licence was assigned" src="https://github.com/user-attachments/assets/5d8d6eb1-aa4d-4681-b565-1441f7f4985a" />

---

## 💡 Next Step

→ [Sample Ticket: Account Locked](./sample-ticket-account-locked.md)





























# Outlook Desktop App - Mailbox Not Found Error

## 1. Ticket Details

- **Ticket Subject:** Unable to Access Outlook Desktop App - Mailbox Not Found Error
- **Username:** Seema
- **Contact Number:** *******
- **Email Address:** *******
- **Priority:** High
- **Category:** Software / Microsoft Outlook
- **Ticket Type:** Incident

## 2. User-Reported Issue

**Description:**

Hi IT Support,

I am unable to access my mailbox through the Outlook desktop app. When I open Outlook, I receive the following error message:

*“Something went wrong. We couldn't find the mailbox for this account.”*

I am unable to access my emails through the Outlook desktop application and I need access to continue my work.

Could you please investigate and help me resolve this issue?

Thank you.

## 3. Investigation Notes

1. Verified the user's identity according to the approved verification procedure.
2. Confirmed the Outlook desktop app error and checked whether the user could access their mailbox through Outlook on the web.
3. Checked the user's Microsoft 365 account status and verified that the appropriate Exchange Online licence was assigned.
4. Checked whether the user's mailbox existed and was provisioned correctly in Exchange Online.
5. Performed the appropriate troubleshooting steps based on the findings.
6. Asked the user to retry accessing Outlook and verified that the mailbox opened successfully.

## 4. Resolution / Closure Note

The Outlook mailbox access issue was investigated and the appropriate corrective action was taken based on the findings. The Exchange online license was assigned to the user and The user successfully accessed the mailbox through the Outlook desktop app. Troubleshooting actions and verification results were documented in the ticket.

- **Resolution:** Outlook mailbox access restored.
- **Final Status:** Resolved / Closed after successful verification.






<img width="1920" height="1080" alt="Screenshot (172)" src="https://github.com/user-attachments/assets/ef848193-3777-4af9-bd4f-a62e9ebb21d4" />



























<img width="1920" height="1080" alt="Screenshot (176)" src="https://github.com/user-attachments/assets/ccb66b70-23be-4394-b412-f2488b368ac1" />

















<img width="1920" height="1080" alt="Screenshot (177)" src="https://github.com/user-attachments/assets/5d8d6eb1-aa4d-4681-b565-1441f7f4985a" />

