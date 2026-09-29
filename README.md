Windows Security Event Analysis

🎯 Objective

The objective of this project is to practice analyzing Windows Security Event Logs and understand how security events can be investigated in a SOC environment.

I performed controlled activities on my Windows 11 system and analyzed the resulting security events using Windows Event Viewer.

🛠️ Tools Used

- Windows 11
- Windows Event Viewer
- PowerShell
- GitHub

🔎 Events Investigated

Event ID| Event| Investigation
4625| Failed Logon| Investigated unsuccessful login attempts
4624| Successful Logon| Investigated successful authentication
4720| User Account Created| Investigated creation of a local account
4688| Process Created| Investigated creation of a new process

🧪 Lab 1 — Event ID 4625

What happened?

A controlled failed login attempt was performed on the Windows system.

What I investigated

- Timestamp
- Account name
- Logon Type
- Source information
- Failure reason
- Status/SubStatus

Security relevance

Event ID 4625 records a failed logon attempt. Repeated or unusual failed logons may require further investigation.

Evidence

"Event 4625" (screenshots/event-4625-failed-logon.png)

---

🧪 Lab 2 — Event ID 4624

What happened?

A successful login was performed and the corresponding security event was analyzed.

What I investigated

- Timestamp
- Account
- Logon Type
- Authentication information
- Source information

Security relevance

Event ID 4624 records a successful logon. Analysts can use it to understand when and how an account authenticated.

Evidence

"Event 4624" (screenshots/event-4624-successful-logon.png)

---

🧪 Lab 3 — Event ID 4720

What happened?

A controlled local user account was created and the resulting security event was investigated.

What I investigated

- Account created
- Creator account
- Timestamp
- Computer
- Account information

Security relevance

Event ID 4720 records the creation of a user account. Unexpected account creation can require investigation.

Evidence

"Event 4720" (screenshots/event-4720-account-created.png)

---

🧪 Lab 4 — Event ID 4688

What happened?

A harmless process was executed and the resulting process-creation event was investigated.

What I investigated

- New process
- Process ID
- Parent process
- Creator information
- Command line, when available

Security relevance

Event ID 4688 records the creation of a new process and can provide useful evidence during endpoint investigations.

Evidence

"Event 4688" (screenshots/event-4688-process-created.png)

---

🧠 Investigation Approach

For each event, I followed this basic investigation process:

Event → Timestamp → Account/Process → Source → Relevant fields → Determine what happened → Document findings

📚 Skills Practiced

- Windows Event Viewer
- Windows Security Logs
- Event ID analysis
- Authentication investigation
- Account activity investigation
- Process investigation
- Basic SOC alert investigation
- Security evidence documentation

⚠️ Disclaimer

This project was performed in a controlled personal lab environment for cybersecurity learning and defensive analysis.

👨‍💻 Author

Kaif Katike

Aspiring SOC Analyst | Cybersecurity Learner
