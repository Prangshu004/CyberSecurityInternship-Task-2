# CyberSecurityInternship-Task-2

## 📌 Task Title:
**Phishing Email Analysis**

---

## 🧠 Objective:
The objective of this task is to analyze a suspicious email and identify phishing characteristics such as spoofed sender addresses, header discrepancies, malicious links, social engineering tactics, and language red flags. This activity is designed to develop real-world phishing detection skills.

---

## 🛠️ Tools & Resources Used:
- Sample phishing email (publicly available)
- [MxToolbox Email Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx)
- Web browser (to hover & inspect links)
- Email client (or raw .eml/.txt file)

---

## 🧪 Experiment Steps:

### 🧩 Step 1: Sample Phishing Email
A publicly available phishing email sample was selected for the analysis. The subject line read:


---

### 🧩 Step 2: Sender Email Analysis
**Displayed Sender:** `support@secure-update.com`  
**Actual Domain in Header:** `reply-to: hacker@phishingsite.ru`  
📌 **Observation:** Spoofed sender address – email domain mismatch

---

### 🧩 Step 3: Header Analysis
The full email header was analyzed using [MxToolbox Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx). Findings:

- SPF check: **Fail**
- DKIM: **Not Signed**
- Received Path: Shows suspicious foreign relay servers
- Return-Path: Not matching the sender

📌 **Observation:** Indicators of forged origin and poor domain authentication

---

### 🧩 Step 4: Suspicious Links
The email contained a button:  
**Text on Button:** "Verify Account Now"  
**Actual Link (hovered):** `http://malicious-site.ru/verify?uid=2947`

📌 **Observation:** Link redirects to a non-reputable domain unrelated to the supposed sender

---

### 🧩 Step 5: Language Red Flags
- Used phrases like:
  - "Act Now!"
  - "Your account will be permanently locked."
- Urgency + Fear tactics

📌 **Observation:** Classic social engineering strategy to trick users into reacting emotionally

---

### 🧩 Step 6: Spelling & Grammar
Examples from the email:
> "Your acount has been block due to supsicious activity."  
📌 **Observation:** Poor grammar and spelling is often a sign of phishing attempts

---

## 🔍 Phishing Indicators Summary:

| Indicator                      | Found? | Notes                                                 |
|-------------------------------|--------|--------------------------------------------------------|
| Spoofed sender address        | ✅     | Mismatch between "From" and "Reply-To" fields         |
| Failing SPF/DKIM              | ✅     | Failed sender authentication                          |
| Suspicious link               | ✅     | Redirects to unknown .ru domain                       |
| Urgency in language           | ✅     | "Act now or lose access"                              |
| Spelling/grammar errors       | ✅     | "acount block due to supsicious activity"             |
| Header discrepancies          | ✅     | Misaligned path and unusual relay                     |
| Email from unknown domain     | ✅     | Secure-looking sender, but fake domain used           |

---

## 📤 Files Included:
- `phishing_email.txt` – Raw text of the email
- `header_analysis_screenshot.png` – Header analysis proof
- `README.md` – This detailed report

---

## ✅ Conclusion:
This email clearly exhibits signs of a phishing attempt. It uses spoofed sender information, urgent and manipulative language, suspicious links, header inconsistencies, and grammatical errors to trick users. Recognizing these indicators helps prevent falling victim to such attacks.

---

## 🧠 Concepts Learned:

- Identifying spoofed sender emails
- Analyzing headers with SPF/DKIM
- Detecting social engineering in email content
- Verifying link safety and origin
- Enhancing email security awareness

---

## 🙋‍♂️ Author:

**Name:** Prangshu Das  
**Role:** Cybersecurity Intern @The ELevate Labs 

**Task Date:** 24rd June 2025


