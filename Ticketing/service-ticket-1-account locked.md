

# 🎫 Sample Ticket - User Account Locked After Multiple Failed Sign-In Attempts

[ Back to README] → [README](https://github.com/seemasm20-source/IT-Ticketing-System-AND-SLA-Management/blob/main/README.md)

---

> **Lab Note:** This is an illustrative ticket, written to show how an account lockout is handled from start to finish. The names, the contact details and the user's message are examples. The technical steps match the Active Directory labs in the Windows Server portfolio.

## 📋 Summary

A user cannot sign in to a company laptop because the account is locked after several wrong passwords. The technician verifies the user's identity, finds the cause, unlocks the account, and confirms that the user can work again.

---

## 🎫 1. Ticket Details

| Field | Value |
|-------|-------|
| **Ticket subject** | User account locked - unable to sign in |
| **Username** | Seema |
| **Contact number** | *(hidden)* |
| **Email address** | *(hidden)* |
| **Ticket type** | Incident |
| **Category** | Account and Access |
| **Priority** | 🟠 High |
| **SLA targets** | Response: 1 hour. Resolution: 8 hours |

> **Why High?** The user cannot sign in to Windows or Outlook, so there is no workaround and the user cannot work at all. One user is affected, so some organisations would set Medium. Follow your organisation's priority rule. 

---

## 💬 2. User-Reported Issue

> Hi IT Support,
>
> I am unable to sign in to my company laptop. I entered my password several times, and now I receive a message saying that my account is locked.
>
> I am unable to access my Windows account and Outlook. I need access to continue my work.
>
> Could you please help me resolve this issue?
>
> Thank you.

---

## 🔎 3. Investigation Notes

| Step | Action | Result |
|:----:|--------|--------|
| 1 | **Verified the user's identity** with the approved procedure, for example a callback to the registered number, before any change | Identity confirmed |
| 2 | **Confirmed the symptom** | The laptop shows "The referenced account is currently locked out and may not be logged on to" |
| 3 | **Checked the account status** in Active Directory Users and Computers (ADUC): user → **Properties → Account** tab | The account is locked out, and the **Unlock account** box is available |
| 4 | **Looked for the cause** in the Security log of the Domain Controller: Event ID **4740**, and the **Caller Computer Name** in it | The failed sign-ins came from the user's laptop |
| 5 | **Asked the user** what happened, and whether the password was changed recently | The password was typed wrongly several times |
| 6 | **Unlocked the account**: ticked **Unlock account** → **Apply → OK** | Account unlocked |
| 7 | **Reset the password only if the user had forgotten it.** A reset sets a temporary password and requires a change at the next sign-in | Not needed, because the user knows the password |
| 8 | **Asked the user to try again** and checked Windows and Outlook | The user signs in successfully |

> The details of steps 3, 4 and 6 are in [Unlock an Active Directory User Account](https://github.com/seemasm20-source/Windows-Server-Azure-AD/blob/main/Active%20Directory/unlock-account.md), [Event ID 4740 – Account Locked Out](https://github.com/seemasm20-source/Windows-Server-Azure-AD/blob/main/Event%20Viewer/event-id-4740-account-locked.md) and [Reset Active Directory User Password](https://github.com/seemasm20-source/Windows-Server-Azure-AD/blob/main/Active%20Directory/reset-password.md)

> **Finding the cause matters.** If the same account locks again soon after the unlock, something is still sending the old password, such as a phone, a mapped drive or a saved credential. The caller computer name in Event 4740 shows where to look.

---

## ✅ 4. Resolution and Closure Note

| Field | Entry |
|-------|-------|
| **Cause** | The account was locked out after several failed password attempts |
| **Action** | The identity was verified. The account was unlocked in ADUC. No password reset was needed |
| **Confirmation** | The user signed in to Windows and Outlook successfully |
| **Advice given** | Check saved passwords on other devices, such as a phone, if the lockout happens again |
| **Final status** | Resolved, then Closed after the user confirmed |

---

## 🛠️ If the Account Locks Again

| Check | What it shows |
|-------|---------------|
| **Event ID 4740 → Caller Computer Name** | Which device sends the wrong password |
| **A phone or tablet with the old password** | Mail or Wi-Fi settings that still use the old password |
| **Mapped drives and saved credentials** | Windows **Credential Manager** entries with an old password |
| **A service or scheduled task** | A task that runs under the user's account |
| **Escalate** | If the source is not found, pass the ticket to Tier 2 with the 4740 details |

---

## 🖼️ Screenshots

**Screenshot: account locked at sign-in:**

<img width="1920" height="1080" alt="Windows sign-in screen showing that the account is locked out" src="https://github.com/user-attachments/assets/7c1c8b8a-3847-4ec3-b3e6-19aefed09cef" />

**Screenshot: account status in ADUC:**

<img width="1920" height="1080" alt="ADUC Account tab showing the locked account and the Unlock account option" src="https://github.com/user-attachments/assets/c0d03698-fb73-459e-9e94-526be29ab2d7" />

**Screenshot: sign-in restored:**

<img width="1920" height="1080" alt="The user signed in after the account was unlocked" src="https://github.com/user-attachments/assets/cbd5b91a-bb64-4497-8028-085abf3f5e8d" />

---



