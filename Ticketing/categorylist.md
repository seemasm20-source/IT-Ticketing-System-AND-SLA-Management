
# 📂 Ticket Category List

[ Back to README] → [README](https://github.com/seemasm20-source/IT-Ticketing-System-AND-SLA-Management/blob/main/README.md)

---

## 📋 Summary

A **category** describes what kind of issue a ticket is about. Categories help route a ticket to the right team, and they show which types of issues are most common, so IT can spot trends and fix the causes.

---



## 🗂️ Categories

| Category | Description | Example | Usually handled by |
|----------|-------------|---------|--------------------|
| **Hardware** | Physical device faults: PC, laptop, printer, monitor | A laptop screen is broken. A printer does not print. A PC will not power on | Tier 1, then a hardware or desktop team |
| **Software** | Application errors, crashes, installation and licence problems | Outlook will not open. Teams crashes. Software cannot be installed | Tier 1, then Tier 2 or the application owner |
| **Network** | Connectivity problems: no internet, VPN, Wi-Fi, shared drives | VPN will not connect. No internet access. A shared drive cannot be reached | Tier 1, then the network team |
| **Security** | Compromised accounts, suspicious activity, malware and phishing | A phishing email was received. Ransomware was detected. Unusual sign-in activity | The security team, immediately |
| **Account and Access** | Passwords, lockouts, new accounts, and requests to grant or remove access | A forgotten password. A locked account. A new user needs access to the HR shared drive. A Microsoft 365 licence is needed | Tier 1, with approval from the data or system owner when access is requested |
| **Other** | An issue that fits no category | A question about a process | The help desk, which finds the right team |

> **Security tickets are different.** A suspected phishing email, malware or a possible account compromise goes to the security team **at once**, whatever the SLA says. The user should not click anything, and a computer with malware should be disconnected from the network, following your organisation's procedure.

---

## 🔍 Choosing the Right Category

Some issues could fit two categories. Use the **cause** when you know it, and the **symptom** when you do not.

| Issue | Category | Why |
|-------|----------|-----|
| **"I can't open the shared drive"** | **Network** if the drive is unreachable. **Account and Access** if the drive opens for others but this user gets "Access denied" | The first is a connection fault, and the second is a permission fault |
| **"I can't sign in to Outlook"** | **Account and Access** if the password or the account is the cause. **Software** if the app itself fails | Check the account first |
| **"I need a licence for a program"** | **Account and Access** (a request) | It is a request for access, and not a fault |
| **"My laptop is slow"** | **Hardware** or **Software**, depending on the cause | Start with the symptom, then update the category when you find the cause |
| **"The VPN connects but I can't reach the server"** | **Network** | The fault is in the connection or the routes |
| **"I received a strange email asking for my password"** | **Security** | A possible phishing attack |

> Update the category if the cause turns out to be different. A ticket logged as Network that ends up being a permission problem should be changed to Account and Access, so the reports stay accurate.

---

## 🧩 Subcategories

Many tools add a second level under each category. This is an example.

| Category | Subcategories |
|----------|---------------|
| **Hardware** | Laptop, desktop, printer, monitor, peripheral |
| **Software** | Microsoft 365, operating system, line-of-business application, installation |
| **Network** | Wi-Fi, VPN, internet, shared drive, DNS or DHCP |
| **Security** | Phishing, malware, suspicious sign-in, lost or stolen device |
| **Account and Access** | Password reset, account lockout, new account, permissions, licence |

---

## 💡 Next Step

→ [Ticket Priority Levels](./ticket-priority-levels.md)


