# Free Interactive Security Training Library

**70+ free hands-on SCORM exercises** covering security awareness, GDPR, AI security, and more. Built for people who want to retain what they learn and share with others.

🔗 **[Browse the full library →](https://learning.ransomleak.com/)** &nbsp;|&nbsp; 🎮 **[Try a live demo →](https://ransomleak.com/exercises/phishing/)**


![demo](/Assets/demo.gif)


---

## Why this exists

Most security awareness training is forgettable: boring slide decks, soulless videos, and lately, AI-generated materials that turn people off. The problem isn't the content itself — it's the format, because passive learning doesn't build habits. People sit through a 10-minute video, click "Complete," and remember nothing when it matters.

**This library takes a different approach.**

Every exercise drops you into an interactive 3D office environment where you face realistic incidents in first-person. You interact with real objects — a phone, a PC running a live OS (browser, terminal, Zoom), a flipchart — and make decisions under pressure, just like you would at your desk.

Scenarios include things like:

- Spotting phishing indicators in a suspicious email
- Handling a scam phone call (vishing) in real time
- Downloading a malicious file and watching the consequences unfold

The goal is to build muscle memory so that when something bad is about to happen at work, people remember having faced it before — and respond accordingly. Every exercise ends with a quiz at a 100% pass threshold to confirm the knowledge is stuck.

---

## Format

Every exercise is a **SCORM .zip file** — ready to import into any LMS, embed into your existing training pipeline, or test on [SCORM Cloud](https://cloud.scorm.com/) before rollout.

The repo root contains full course packages. The `Individual Exercises` folder contains standalone exercises if you want to build a custom curriculum.

---

## Usage & License

You're free to use, embed, and teach with this content — personally, professionally, or commercially in workshops. Redistributing or reselling the content as a standalone product is prohibited.

[![CC BY-NC 4.0][cc-by-nc-shield]][cc-by-nc]

This library is licensed under [CC BY-NC 4.0][cc-by-nc]. Free to use and share with attribution. Commercial resale of the content is prohibited.

[cc-by-nc]: https://creativecommons.org/licenses/by-nc/4.0/
[cc-by-nc-shield]: https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg

---

# Courses
### AI Security
Artificial intelligence is transforming how organizations operate – but it's also introducing new attack vectors that traditional security training doesn't cover. This course equips you with the knowledge to recognize and respond to AI-specific threats in your daily work.

#### Exercises

1. **Clawdbot (Moltbot) Prompt Injection**
   Prompt injection is an attack technique where malicious instructions are hidden inside documents, emails, or web pages that an AI assistant processes, causing it to perform unintended actions like leaking confidential data. This exercise puts you in a realistic scenario involving Clawdbot, a viral AI assistant with document analysis capabilities. An attacker has embedded hidden instructions inside a file that Clawdbot is asked to summarize. When the AI reads the document, the injected prompt overrides its original instructions and tricks it into extracting sensitive information from the conversation, then encoding that data into a URL that gets sent to an attacker-controlled server. You will observe the attack unfold in real time, identify the moment the AI's behavior changes, and trace how the exfiltration occurs through what appears to be a normal link.

---

### Web & Browser Safety
Navigate the web safely by understanding browser-based threats and how to avoid them. This course covers HTTPS and website security, safe browsing and download practices, typosquatting awareness, browser autofill risks, extension safety, and file extension awareness. You'll also learn about emerging threats like SEO poisoning and browser notification abuse that exploit trust in everyday browsing.

#### Exercises

1. **HTTPS & Website Security**
   HTTPS means the connection between your browser and a website is encrypted, but it does not guarantee the site itself is legitimate. This exercise puts you in front of several websites where you need to evaluate whether the connection is truly secure. One site displays a padlock icon but uses an expired certificate. Another has a valid certificate issued to a completely different organization. A third triggers your browser's warning page, and you have to decide whether to click through or walk away. The simulation breaks down what a TLS certificate actually proves, who issues them, and why free certificates from services like Let's Encrypt mean that even phishing sites can show a padlock.

2. **Safe Browsing & Downloads**
   Malicious downloads are one of the most common ways malware reaches corporate devices, and they rarely look suspicious at first glance. In this exercise, you search for a legitimate software update and land on a convincing clone of the vendor's official website. The download button triggers a file that looks right, with the correct name and icon, but it carries an embedded payload. You then navigate a scenario where a pop-up claims your browser is outdated and urges an immediate update. The simulation reveals how drive-by downloads work: pages that exploit browser vulnerabilities to install software without your consent.

3. **Typosquatting Awareness**
   Typosquatting is the practice of registering domain names that are slight misspellings or visual lookalikes of legitimate websites, and it catches more people than you would expect. This exercise presents you with a series of URLs and login pages where the differences are measured in single characters. You will encounter domains that swap letters, add extra characters, and use international characters that look identical to Latin letters but point to entirely different servers. That last technique, called a homograph attack, can make a fake domain appear pixel-perfect in your browser's address bar.

4. **Browser Autofill Risks**
   Browser autofill is designed for convenience, but attackers weaponize it to steal data you never intended to share. In 2023, researchers at Princeton found that over 1,100 websites contained hidden form fields specifically designed to capture autofilled data. In this simulation, you follow Alice, a senior consultant who clicks a conference registration link from a colleague. What Alice cannot see are additional fields buried in the page code that her browser quietly fills with her credit card number, phone number, and home address. The exercise finishes with a practical walkthrough of browser autofill settings and verification habits.

5. **Browser Extension Safety**
   Browser extensions operate with deep access to everything you do online. A 2024 Stanford study found that over 280 million users had installed malicious Chrome extensions over a three-year period. In this exercise, you follow Alice at Delvara Analytics as she installs "TabMaster Pro," a productivity extension with a 4.6-star rating. Three weeks later, IT Security traces a data exfiltration incident directly to this extension. You walk through the forensic timeline and then conduct a full extension audit, learning to apply the principle of least privilege to extensions.

6. **Browser Notification Abuse**
   Push notification abuse has become one of the fastest-growing social engineering vectors. Malicious sites trick users into granting notification permissions through deceptive prompts, most commonly fake CAPTCHA challenges. In this simulation, you follow Alice at Brightwave Analytics as she visits an infographic tool that tricks her into granting push notification permission. You experience the attack escalation firsthand, then walk through the full remediation process and learn to identify differences between real CAPTCHA challenges and fake notification prompts.

---

### Passwords & Account Security
This course covers the basics that actually matter: setting up a password manager so you stop reusing passwords, configuring MFA so a stolen password isn't game over, and spotting fake password reset emails before you hand over your credentials on a phishing page.

#### Exercises

1. **Password Manager Habits**
   Most people know they should use unique passwords for every account. Almost nobody actually does it without a password manager. This exercise is a hands-on walkthrough of using an enterprise password manager in daily work. You start by migrating a set of reused and weak passwords from a spreadsheet into a password vault, generating unique replacements for each one. The simulation covers practical friction points and features — including how the manager's URL-binding refuses to autofill on a spoofed login page, tipping you off that something is wrong.

2. **Least Privilege Awareness**
   The principle of least privilege means every person and system gets only the minimum access required to do their job, nothing more. This exercise drops you into a realistic access review where you audit the permissions assigned to members of a cross-functional project team. Some users have admin rights to systems they accessed once, six months ago. Others share a service account because "it was easier than requesting individual access." One contractor still has VPN credentials three weeks after their project ended. You work through each case, deciding what to keep, what to revoke, and what to flag.

3. **Joiner-Mover-Leaver Awareness**
   Every time someone joins your company, changes roles, or leaves, their access permissions need to change with them. This simulation places you in three distinct scenarios: onboarding a new hire, managing a lateral role change, and processing a departure with next-day credential revocation. Each scenario includes realistic complications such as a manager requesting exceptions, a departing employee who forwarded files to a personal email, and a new hire who needs emergency access on day one.

4. **MFA Setup & Best Practices**
   Multi-factor authentication blocks over 99% of automated account compromise attempts, according to Microsoft's security research. This exercise walks you through setting up MFA on a corporate account, comparing the security tradeoffs between SMS codes, authenticator apps, and hardware security keys. You will see a live demonstration of how attackers intercept SMS-based one-time passwords, and experience a push notification you did not initiate — the telltale sign of an MFA fatigue attack — with training on the correct response.

5. **Credential Stuffing Awareness**
   Credential stuffing is the automated use of stolen username-password pairs to break into unrelated accounts. This exercise puts you in the middle of a credential stuffing incident targeting your organization. You review alerts flagging thousands of failed login attempts, trace the attack pattern, determine which accounts were compromised, and take the right containment steps. The simulation walks you through checking whether your own credentials appear in known breach databases and building habits that break the password reuse cycle.

6. **Account Recovery Security**
   Account recovery is one of the weakest links in organizational security, and attackers know it. In this simulation, you play the role of a help desk analyst fielding an urgent account recovery request from someone who claims to be a locked-out employee. The caller has done their homework — knowing the employee's full name, department, and manager. Your job is to follow proper identity verification procedures under pressure, and the exercise covers self-service recovery flows and how poorly configured security questions create openings for attackers.

7. **Privileged Access Basics**
   Privileged accounts — the admin and root credentials that control your organization's critical systems — are the number one target for attackers. This exercise puts you in two contrasting scenarios to show why. First, you walk through a just-in-time access workflow for a routine server update. Second, you investigate the aftermath of an incident where an admin used their privileged account for everyday tasks like checking email and browsing, and an attacker phished that account, gaining immediate access to the entire infrastructure.

---

### Device Security
Keep your devices safe from malware, ransomware, and unauthorized access. This course covers essential device security practices including endpoint patching, encryption, backup strategies, and EDR alert management. You'll learn about USB drop attacks, IoT security risks, mobile device security, safe Bluetooth practices, and how to manage mobile app permissions to minimize your attack surface.

#### Exercises

1. **Ransomware**
   Ransomware attacks cost organizations an average of $4.54 million per incident. This simulation places you at the exact moment a ransomware attack begins, starting with a suspicious email attachment. You observe unusual system behavior — files renaming themselves, programs becoming unresponsive, a ransom note appearing — and must make rapid decisions under pressure. Each choice reveals how ransomware propagates through shared drives, exploits open network connections, and encrypts data both locally and across mapped resources.

2. **USB Drop Attack**
   A USB drop attack is a social engineering technique where attackers leave infected USB drives in locations where target employees are likely to find and plug them in. In this simulation, you find a USB drive labeled with something tempting and experience what happens when that drive is plugged in — from autorun scripts and fake documents to USB Rubber Ducky devices that compromise a system in under 10 seconds. You learn the correct response and organizational policies for removable media.

3. **Backup Best Practices**
   A proper backup strategy is your last line of defense when ransomware strikes or hardware fails. The 3-2-1 backup rule is the industry standard: keep at least 3 copies of your data, on 2 different types of storage media, with 1 copy stored offsite or in the cloud. This simulation walks you through the real consequences of common backup failures, covers ransomware resilience through offline and immutable backups, and teaches what individual employees are expected to do within an organization-wide backup strategy.

4. **Encryption & Lock Discipline**
   Device encryption converts your data into unreadable code that can only be unlocked with the correct credentials. This simulation begins with a common situation: you step away from your desk for coffee, leaving your laptop open and unlocked. The exercise fast-forwards through what an attacker can accomplish in 90 seconds — reading email, copying files, installing a keylogger. You practice configuring automatic screen lock timers, setting strong device passwords, and verifying that full disk encryption is actually enabled on your machine.

5. **OS Updates & Patching Basics**
   Operating system and software updates frequently contain patches for vulnerabilities that attackers are already exploiting. This simulation puts you in a situation where a system update notification pops up during a busy workday and you click "Remind me later." The exercise walks you through what that specific update was patching, known exploits targeting the vulnerability, and how quickly attackers weaponize public vulnerability disclosures — on average within 15 days of a CVE being published.

6. **Endpoint Patching & EDR Alerts**
   An EDR alert pops up on your screen mid-morning. Is this a false positive or the start of a real incident? This exercise puts you in front of a live EDR dashboard where you see specific alert types — process anomalies, unauthorized registry changes, unusual network connections — and decide whether to ignore, investigate, or escalate. The simulation also covers why endpoint patching matters from your perspective, connecting individual patch decisions to the organization's broader defense posture.

7. **Safe Bluetooth Practices**
   Your Bluetooth headphones connect automatically every morning — but that invisible radio signal could expose confidential calls. This simulation starts with sensitive data intercepted through a Bluetooth vulnerability and works backwards through the incident. You conduct a full paired-device audit, remove unrecognized connections, and configure non-discoverable mode. The exercise covers the BlueBorne, KNOB, and BLUFFS vulnerability families and why leaving Bluetooth discoverable in public spaces creates a measurable attack surface.

8. **File Extension Awareness**
   A file named Invoice_Final.pdf.exe sits among legitimate documents — the PDF icon looks normal, and Windows hides the .exe extension by default. This simulation walks you through a file-based attack from start to finish, highlighting warning signs most people miss. You learn which file extensions can execute code on your system, including less obvious ones like .scr, .cmd, .vbs, .js, and .ps1, and how to reveal true file types and verify legitimacy before opening anything.

---

### Protecting Sensitive Information
Understand how to identify, handle, and safeguard sensitive data throughout its lifecycle. From data classification and secure sharing practices to preventing data leakage and identity theft, this course equips you with practical skills for protecting confidential information. You'll also learn about metadata risks, log sensitivity, secure document disposal, and how to use generative AI tools safely without exposing sensitive data.

#### Exercises

1. **Data Leakage**
   Data leakage occurs when sensitive information leaves your organization's control through accidental or negligent means. This exercise walks you through the most common data leakage scenarios: accidentally sending a confidential financial report to the wrong email recipient, discovering hidden metadata in a Word document that reveals internal discussions, and finding an unsecured file share with default permissions. The simulation also covers less obvious leakage channels such as personal cloud storage, video calls with active screen sharing, and AI tools without data processing agreements.

2. **Data Classification Basics**
   Data classification is the practice of labeling information by sensitivity level so your organization can apply the right protections to the right data. This exercise drops you into a classification workflow where you sort real-world documents and datasets into categories like Public, Internal, Confidential, and Restricted. The simulation shows what proper handling looks like at each classification level, covering storage requirements, sharing restrictions, encryption obligations, and disposal procedures.

3. **Identity Theft Prevention**
   Identity theft costs individuals an average of 200 hours and significant financial loss to resolve. This simulation places you in scenarios where identity theft risk is high but easy to miss — a convincing HR email requesting you to "verify" your Social Security number, a colleague's personnel file open on an unattended workstation, a phone call from someone who already knows your name and department. Each scenario teaches you to spot warning signs and learn specific verification steps, reporting procedures, and daily habits that reduce your exposure.

4. **Secure Sharing Practices**
   Sharing files and data is something you do dozens of times per day, and each instance is a decision point. This exercise walks you through common sharing scenarios — sending a contract to an external law firm, sharing customer data with a colleague, collaborating with a vendor on a different platform, and transferring large files that exceed email attachment limits. You learn why emailing an unencrypted attachment differs from using a password-protected link with an expiration date, and build a practical checklist for sharing decisions.

---

### Phishing & Impersonation Attacks
How to recognize phishing attacks, avoid data leakage and find out when you've been targeted by an AI voice cloning.

#### Exercises

1. **Vishing**
   Vishing, or voice phishing, uses phone calls to manipulate employees into revealing sensitive information, transferring funds, or granting system access. In this simulation, your phone rings with a caller ID appearing to belong to your company's IT department or a trusted vendor. The person on the other end is calm, professional, and uses industry-specific terminology. They explain a security incident that requires your immediate cooperation. You will practice pausing the conversation, asking verification questions, and using callback procedures through official phone numbers.

2. **Phishing**
   Phishing is the single most common cyberattack vector, responsible for over 80% of reported security incidents. In this interactive 3D simulation, you receive a suspicious email that closely mirrors real-world phishing campaigns. You examine sender addresses for subtle misspellings, hover over links to reveal mismatched URLs, and evaluate the emotional pressure tactics attackers rely on. Beyond identification, this exercise trains you in proper response protocols including forwarding suspicious messages to your security team and understanding how stolen credentials escalate into full account takeovers.

3. **Double Barrel Phishing**
   Double barrel phishing is a two-stage attack where the first message is completely harmless and the second message carries the malicious payload. The initial email establishes legitimacy and builds trust — a simple introduction, a meeting confirmation, or a routine document share. The follow-up arrives hours or days later referencing the first message. In this simulation, you receive a friendly introductory email with no links or attachments, and then a follow-up referencing your interaction that includes a credential-harvesting document.

4. **Whaling With A Deepfake**
   Deepfake-enabled whaling combines executive impersonation with AI-generated audio and video to create attacks that are nearly impossible to detect by sight and sound alone. In February 2024, a finance worker transferred $25 million after a video call with what appeared to be the company's CFO and several colleagues — every person was a deepfake. In this simulation, you join a video conference where a senior executive makes an urgent financial request and must figure out what is wrong before authorizing a transfer that cannot be reversed.

5. **Social Engineering**
   Social engineering bypasses every technical security control by targeting the human layer directly. In this simulation, you receive a phone call from someone who sounds credible and is prepared with details about your company, your department, your manager's name, and recent projects — all harvested from public sources. You will practice holding your ground when the caller escalates pressure using authority, reciprocity, and artificial urgency, and learn how to redirect verification through official channels without creating an adversarial interaction.

6. **Business Email Compromise**
   Business email compromise (BEC) is the most financially damaging form of cybercrime, with the FBI reporting $2.9 billion in adjusted losses in 2023 alone. In this simulation, you receive an urgent email appearing to come from your CEO or CFO requesting an immediate wire transfer or change to vendor payment details. The email tone matches the executive's communication style and includes a plausible business justification. You practice the verification workflow that stops these attacks despite the urgency.

7. **Smishing**
   Smishing is phishing delivered through SMS text messages, with click rates on malicious SMS links running 6 to 10 times higher than email phishing. In this simulation, you receive a text message that looks like a package delivery notification, a banking security alert, or an IT department password reset request. The message is short, urgent, and contains a shortened URL that obscures the real destination. You learn to slow down, verify through official channels, and recognize how attackers time their messages to coincide with real events to increase credibility.

8. **Callback Phishing**
   Callback phishing (also called TOAD, or Telephone-Oriented Attack Delivery) is a hybrid attack that begins with an email and ends with a phone call. There is no malicious link in the message — instead, the email poses as an invoice or subscription renewal and includes a phone number for "customer support." In this simulation, you receive a realistic callback phishing email claiming a charge of $499.99 has been applied to your account. You practice evaluating callback phishing indicators and learn the manipulation tactics used during the phone conversation.

9. **Spear Phishing**
   A conference talk. A flattering follow-up email from an admiring attendee. A link to a collaboration portal with your session recordings. Everything checks out — but every detail was harvested from a single LinkedIn post. In this simulation, you step into the role of a Senior Product Analyst who recently spoke at an industry conference. Spear phishing accounts for only 0.1% of all email attacks but is responsible for 66% of all breaches. You trace exactly how an attacker moves from a social media post to a fully personalized phishing email.

10. **QR Code Phishing (Quishing)**
    A company-branded email arrives: Mandatory Security Upgrade. It includes a QR code for quick mobile setup. You scan the code with your phone — and that's exactly what attackers are counting on. QR codes convert URLs into images, which email security filters that scan text-based links never see. Hoxhunt reported a 587% surge in QR code phishing attacks in 2023. In this exercise, you'll receive a realistic quishing email, walk through the full attack chain, and learn to preview QR code destinations before scanning.

11. **Tech Support Scams**
    You're browsing a legitimate news site when your screen is suddenly taken over by a full-screen alert claiming your computer is infected with a trojan. A siren blares from your speakers. None of it is real — the "alert" is a webpage using JavaScript to fake a system warning. But in the moment, with adrenaline pumping, it feels completely real. The FBI received over 37,500 tech support scam complaints in 2023, with reported losses exceeding $924 million. You'll walk through the attacker's full playbook and learn why the correct first response is Ctrl+Alt+Delete and force-closing the browser.

12. **WhatsApp Social Engineering**
    A WhatsApp message from your CEO. New number, they explain, because their usual phone is being repaired. They need a quick favor — can you pick up some gift cards for a client appreciation event? This is one of the most common and costly social engineering attacks in the world. In this simulation, you'll experience a real-time WhatsApp conversation with someone impersonating your manager, with messages that escalate in urgency and emotional pressure. You'll learn why attackers choose gift cards, why they create time pressure, and why they pick messaging apps over email.

13. **SEO Poisoning Awareness**
    You need to download a PDF reader for a work task. You search for it and click the first result — the page looks like the vendor's official site, same logo, same layout, same download button. But the URL is subtly wrong, and the installer contains malware bundled alongside the legitimate application. SEO poisoning places malicious websites at the top of search results for common software searches. In this simulation, you'll encounter a poisoned result and learn to verify software by checking publisher signatures, comparing file hashes, and navigating directly to vendor sites.

---

### GDPR Compliance
Equip your team with practical knowledge to handle personal data responsibly and stay compliant with the EU's General Data Protection Regulation.

#### Exercises

1. **Marketing Consent Management**
   GDPR marketing consent management is the process of collecting, recording, and honoring user preferences for receiving marketing communications under GDPR Article 7. This interactive exercise drops you into a scenario where your marketing team needs to launch a new email campaign while staying compliant. You design opt-in flows that meet the "clear affirmative action" standard, build a consent record system, and handle a live consent withdrawal request. Regulators have issued fines exceeding €400 million for consent violations since 2018.

2. **Fraudulent DSAR Detection**
   Fraudulent DSARs are data subject access requests submitted by attackers impersonating legitimate individuals to extract personal data. This exercise presents you with multiple incoming DSARs — some genuine and some fraudulent — and you evaluate each for red flags: inconsistencies in claimed identity, urgency language, requests targeting specific high-value individuals, and contact details that don't match existing records. You practice the escalation process when a request looks suspicious, including how to delay response without violating the 30-day deadline.

3. **Data Breach Response**
   GDPR data breach response is the mandatory process of detecting, assessing, and reporting personal data breaches within the 72-hour notification window set by Article 33. Failure to notify on time can result in fines up to €10 million or 2% of global annual turnover. This exercise places you inside the first hours after your organization discovers a potential compromise. You triage the incident, draft the notification to your supervisory authority, and practice making difficult judgment calls about whether an incident qualifies as notifiable.

4. **Third-Party Data Processor Vetting**
   GDPR Article 28 mandates that controllers only use processors providing "sufficient guarantees" of appropriate data protection measures. You are directly liable for compliance failures by your processors. This exercise simulates evaluating a SaaS vendor your organization wants to engage for customer data processing, reviewing their security certifications, handling practices, sub-processor arrangements, and breach notification procedures. The scenario includes a realistic Data Processing Agreement with clauses that fall short of GDPR requirements.

5. **Security Incident Response**
   Security incident response under GDPR requires organizations to determine whether a security event involves personal data and, if so, follow specific assessment and notification procedures within tight regulatory deadlines. You are placed in command of an active incident where network monitoring detects suspicious data exfiltration patterns. You must coordinate between IT security, who want to contain and investigate, and the privacy team, who need to assess personal data implications — priorities that sometimes conflict.

6. **Privacy by Design Review**
   Privacy by Design is a GDPR requirement under Article 25 that obligates organizations to integrate data protection into the development of products from the earliest stage. This exercise puts you in the role of a privacy reviewer evaluating a new product feature before it goes to production. You examine the feature's data collection scope, identify where it gathers more personal data than necessary, and navigate realistic tradeoffs between product functionality and privacy across behavioral tracking and user profiling requests.

7. **Legitimate DSAR Processing**
   A data subject access request (DSAR) is the right under GDPR Article 15 for any individual to obtain a copy of their personal data. Organizations must respond within one calendar month. This exercise simulates a realistic DSAR from a customer who wants all personal data your organization holds. You verify the requester's identity, search across multiple systems including CRM, email archives, support tickets, analytics platforms, and backup databases, then compile the response package and handle redaction of third-party personal data.

8. **Cross-Border Data Transfers**
   Cross-border data transfers under GDPR restrict the movement of personal data from the EEA to countries without an adequacy decision. This exercise places you in a scenario where your organization needs to transfer customer data to a provider outside the EEA. You evaluate whether the destination country has an adequacy decision, select Standard Contractual Clauses as the transfer mechanism, and conduct a Transfer Impact Assessment following the Schrems II ruling — examining government surveillance powers, judicial remedy, and independent oversight.

9. **PII Document Redaction**
   PII document redaction is the process of permanently removing personally identifiable information from documents before they are shared. This exercise gives you a set of realistic business documents — contracts, customer records, internal reports, email threads — that must be sanitized before release. The exercise teaches you why common redaction methods fail: drawing black boxes over text in a PDF does not always remove the underlying data, and metadata in Word files can contain tracked changes that expose what you thought you removed.

10. **Data Protection Impact Assessment**
    A Data Protection Impact Assessment (DPIA) is a structured risk analysis required by GDPR Article 35 before any processing operation likely to result in high risk to individuals' rights. This exercise gives you a processing activity that triggers multiple DPIA criteria, and you work through the assessment from start to finish: describing processing operations, assessing necessity and proportionality, mapping risks like unauthorized access and discriminatory profiling, documenting mitigation measures, and producing a DPIA document that meets Article 35(7) content requirements.

11. **Data Mapping and Records of Processing**
    Records of Processing Activities (RoPA) are mandatory documentation required by GDPR Article 30. This exercise tasks you with building a processing register from scratch for a mid-sized organization. You conduct data mapping interviews with department heads to discover what personal data each team collects, why they collect it, where it is stored, who it is shared with, and how long it is retained. You then connect these fragmented data flows into a coherent register covering all fields required under Article 30(1).

---

### Safe Communication & Sharing
Communicate and collaborate securely across platforms without exposing sensitive information. This course covers cloud sharing controls, collaboration tool hygiene, guest access management, secure messaging practices, and the risks of social media oversharing. You'll learn to manage third-party app OAuth permissions and follow social media policies that protect both you and your organization.

#### Exercises

1. **Social Media Oversharing**
   Social media oversharing is a primary reconnaissance tool for targeted cyberattacks. Attackers routinely scan platforms like LinkedIn, Instagram, Facebook, and X to collect personal and professional details that make phishing and vishing attacks far more convincing. This exercise demonstrates the attacker's perspective — showing how a single vacation photo, birthday post, new job announcement, and conference check-in can be pieced together to build a complete profile enabling highly personalized attacks. You learn to audit your own digital footprint and configure privacy settings that reduce exposure.

2. **Cloud Sharing Controls**
   Cloud storage platforms make sharing easy — too easy, in many cases. In this exercise, you manage a project folder where files have accumulated a tangle of permissions over time. One document is shared with "anyone with the link." Another was shared with a contractor who left six months ago. A third has edit permissions granted to an entire department. You audit these permissions, tighten access to the minimum required level, set expiration dates, and then face a time-pressured scenario where the fastest option is a public link.

3. **Guest Access Management**
   Guest access lets external collaborators, vendors, and clients into your corporate tools — but those accounts often outlive the relationship that created them. This exercise drops you into a Teams workspace where several guest accounts are still active months after their projects ended. One former vendor still has access to internal channels containing product roadmaps. You review each guest account, determine whether access is still justified, revoke or restrict permissions where needed, and create a structured offboarding checklist for guest accounts.

4. **Secure Messaging Practices**
   Workplace messaging tools like Slack and Teams feel casual and private, which is exactly why employees share things there they would never put in an email. This exercise begins with a chat thread where a colleague pastes a database password to "save time," another thread containing customer personal data, and a photo of a whiteboard posted to a public channel. You assess each situation and practice the correct way to share sensitive information. The simulation also introduces an attacker who compromises a colleague's messaging account to request files that seem routine.

5. **Social Media Policy**
   Your company's social media policy exists because a single careless post can leak proprietary information, damage a brand, or give attackers the reconnaissance they need for a targeted attack. This exercise starts with real-world scenarios: an employee's LinkedIn post about "a big deal closing next week" tips off a competitor; a photo inside the office captures a monitor displaying a client list. You evaluate each post, determine the specific risk, and rewrite the content to remove the exposure without losing the message.

6. **Third-Party App OAuth Risks**
   OAuth lets you connect third-party apps to your work accounts with a single click — and malicious apps use the same authorization flow as legitimate ones. A 2023 Microsoft Digital Defense Report found that OAuth-based attacks on enterprise tenants increased by 65% year-over-year. This exercise starts when you receive a link to a new scheduling tool that requests access to your email, contacts, calendar, and files. You evaluate whether those permissions match what the app actually needs, audit apps currently connected to your corporate account, and recognize consent phishing campaigns.

---

### Workplace Security
Protect your physical and digital work environment from insider threats, unauthorized access, and unconventional attack vectors. This course covers both accidental and intentional insider threats, shadow IT risks, visitor and badge management, clean desk policies, and emerging threats like image-based attacks (stegosploit). You'll learn to maintain a security-conscious workplace culture.

#### Exercises

1. **Insider Threat (Intentional)**
   A malicious insider is an employee, contractor, or business partner who deliberately abuses their authorized access. According to the 2024 Ponemon Institute report, intentional insider incidents take an average of 86 days to contain and cost approximately $701,500 per incident. This simulation places you in a workplace scenario where a colleague's behavior starts raising quiet red flags — after-hours access to file shares they don't normally use, large downloads to a personal USB device. The challenge is recognizing the pattern before the damage is done.

2. **Shadow IT Awareness**
   Shadow IT refers to any software, cloud service, or hardware that employees use for work without IT or security team approval. Gartner estimates that 30–40% of IT spending in large enterprises goes toward shadow IT. In this simulation, your team is under deadline pressure and someone suggests using a free online tool to convert a confidential spreadsheet. The exercise walks you through what actually happened behind the scenes: your company data was uploaded to a third-party server with no data processing agreement, no encryption guarantees, and no way to request deletion.

3. **Image-Based Attacks (Stegosploit)**
   Steganography is the practice of hiding data inside ordinary-looking files, and images are the most common carrier. An attacker can embed executable code within the pixel values of a JPEG or PNG file — the image opens normally, looks normal, and passes most email filters. This exercise begins with a realistic scenario: a contractor sends a portfolio of sample work, one of which contains a hidden JavaScript payload exploiting a browser rendering vulnerability. You examine file metadata, compare file sizes, and learn three distinct attack methods and their corresponding detection approaches.

4. **Insider Threat (Accidental)**
   It starts with two browser tabs and a Monday morning rush. In this simulation, you step into the role of a project manager who accidentally attaches a confidential HR salary spreadsheet to an email meant for an external client. Forty-seven employees' compensation data lands in the wrong inbox. You experience the moment the Data Loss Prevention system flags the outbound email, then work through filing an incident report. Accidental insiders account for more than half of all data breach incidents, according to the 2024 Ponemon report.

5. **Collaboration Tool Hygiene**
   A deadline is closing in, and copying database credentials into a team channel feels like the fastest path forward. In this simulation, you experience what happens three days later when IT Security reveals those credentials were used for unauthorized access through two vectors you never considered: a stale webhook integration silently forwarding channel messages to an external endpoint, and an ex-contractor who still has full channel access six weeks after leaving. You conduct a full channel audit and practice the correct workflow for sharing credentials.

---

### Remote & Home Office Security
Secure your remote work setup against the unique threats that come with working outside the office. This course covers home office security fundamentals, VPN usage, home router hardening, secure online meeting practices, and the specific risks of working from shared or public spaces.

#### Exercises

1. **VPN Usage & Safety**
   A VPN encrypts your internet traffic between your device and your company's network, but only when it is configured and used correctly. In this exercise, you connect to a coffee shop Wi-Fi and attempt to access corporate resources while your VPN silently disconnects mid-session. You work through the real consequences of that dropped connection: exposed login credentials, unencrypted file transfers, and session data leaking across a public network. The simulation also covers split tunneling and a fake VPN app on a third-party download site.

2. **Home Router Security**
   Your home router handles every packet of data between your devices and the internet. A 2023 Broadband Genie survey found that 86% of users had never changed their router's admin password. This exercise starts with a scenario where you log into your router's admin panel and find devices you don't recognize on your network. You identify connected devices, remove unauthorized ones, change the default admin password, disable WPS, enable WPA3 encryption, and update the firmware. The exercise also covers DNS hijacking and how to recognize signs of router tampering.

---

### Real-World Incidents
Learn from documented cybersecurity breaches that actually happened. Each module walks you through how the incident unfolded, what went wrong, and the key lessons organizations can apply to prevent similar attacks.

#### Exercises

1. **MGM Resorts Breach**
   The September 2023 MGM Resorts breach is one of the most expensive social engineering attacks in corporate history, costing an estimated $100 million. This exercise walks you through the actual attack chain used by the Scattered Spider threat group: open-source reconnaissance on LinkedIn, a 10-minute vishing call to the IT helpdesk to request a password reset, and deployment of ALPHV/BlackCat ransomware that took down hotel reservation systems, digital room keys, slot machines, and ATMs for approximately 10 days. You evaluate your own organization's identity verification procedures.

2. **OneNote Email Attack**
   This exercise reconstructs a real business email compromise incident where attackers gained access to a client's email account, monitored invoice-related conversations for weeks without sending a single message, and struck at the exact moment a legitimate payment was due. You receive an invoice redirect request appearing to come from a known business contact — with real project details, the right tone, and the right invoice amount — where the only clue is a one-character difference in the sender's domain name.

---

### Security Policies & Your Role
Learn how your organization's security policies protect both the business and its people. This course covers the fundamentals of information security management systems (ISMS), your responsibilities under security policies, audit readiness, and acceptable use of internet and email resources.

#### Exercises

1. **Audit Mindset Basics**
   Compliance audits examine whether your organization actually follows the security policies it claims to follow. In this simulation, you step into the shoes of an internal auditor reviewing a department's access controls and documentation practices. You check whether password policies match real behavior, verify that access reviews happened on schedule, and identify gaps between written procedures and daily operations. The exercise builds your ability to spot compliance gaps before external auditors do and teaches you how to maintain the documentation trail that keeps your t