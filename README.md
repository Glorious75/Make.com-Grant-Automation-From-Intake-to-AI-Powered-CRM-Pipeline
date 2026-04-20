# Make.com Grant Automation: From Intake to AI-Powered CRM Pipeline

**Built for TechBridge Foundation | Prepared by Gloria Njorteah**

AI-powered grant intake &amp; eligibility automation system built for TechBridge Foundation using Make.com, Jotform, Airtable, OpenAI GPT-4o, Monday.com &amp; Gmail. Automates eligibility screening, AI summarisation and CRM pipeline management — saving nonprofits 80%+ admin time.

![Make.com](https://img.shields.io/badge/Make.com-6D00CC?style=for-the-badge&logo=make&logoColor=white)
![Jotform](https://img.shields.io/badge/Jotform-FF6100?style=for-the-badge&logo=jotform&logoColor=white)
![Airtable](https://img.shields.io/badge/Airtable-18BFFF?style=for-the-badge&logo=airtable&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI_GPT--4o-412991?style=for-the-badge&logo=openai&logoColor=white)
![Monday.com](https://img.shields.io/badge/Monday.com-FF3D57?style=for-the-badge&logo=monday&logoColor=white)
![Gmail](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)

---

## 📋 Table of Contents
- [Project Overview](#-project-overview)
- [Eligibility Criteria](#-eligibility-criteria)
- [Tech Stack](#-tech-stack)
- [Scenario 1 — Eligibility Checker](#-scenario-1--grant-eligibility-checker)
- [Scenario 2 — Full Application Collector](#-scenario-2--full-application-collector)
- [Airtable Database](#-airtable-database)
- [Monday.com CRM Pipeline](#-mondaycom-crm-pipeline)
- [Key Benefits for NGOs](#-key-benefits-for-ngos)
- [Author](#-author)
- [License](#-license)

---

## 🌍 Project Overview

Nonprofit organisations running grant programmes face a significant administrative burden — manually reviewing applications, checking eligibility, communicating with applicants, and tracking submissions across scattered spreadsheets and inboxes.

This project delivers a **fully automated, AI-powered grant management system** built in **Make.com** for the **TechBridge Foundation Community Innovation Grant** — handling everything from initial intake to CRM pipeline management.

| Challenge | Solution |
|-----------|----------|
| Manual eligibility screening | Automated router checks all 5 criteria instantly |
| Inconsistent decisions | Same rules applied to every applicant, every time |
| Delayed communication | Instant personalised emails sent automatically |
| Scattered data | Single Airtable database as source of truth |
| No pipeline visibility | Real-time Monday.com CRM board |
| Reviewers reading full applications | GPT-4o generates concise AI summaries |

---

## 🎯 Eligibility Criteria

An applicant must meet **all five criteria** to proceed:

| # | Criteria |
|---|----------|
| 1 | Organisation must be based in **CA, TX, NY, IL or GA** |
| 2 | Grant request must be **between $5,000 and $50,000** |
| 3 | Must be a **registered 501(c)(3) nonprofit** |
| 4 | Organisation must have been **operating for at least 2 years** |
| 5 | Must **not have received a TechBridge grant in the past 12 months** |

---

## 🛠 Tech Stack

| Tool | Purpose |
|------|---------|
| **Make.com** | Automation platform — runs both scenarios |
| **Jotform** | Intake form and full grant application form |
| **Airtable** | Central database for all submissions and statuses |
| **OpenAI GPT-4o** | AI-generated application summaries for reviewers |
| **Monday.com** | CRM pipeline for grant review and scoring |
| **Gmail** | Automated email communications to applicants |

---

## ✅ Scenario 1 — Grant Eligibility Checker

The first Make.com scenario runs the moment an applicant submits the intake form. It saves their details to Airtable, runs the eligibility check, and automatically routes them to either the eligible or ineligible path.

### 📝 Step 1 — Grant Intake Form (Jotform)
Applicants complete a short intake form providing contact details, organisation name, state, nonprofit status, years operating, and funding request amount.

![Intake Form 1](Form%20Intake%201.JPG)
![Intake Form 2](Form%20Intake%202.JPG)

---

### ⚙️ Step 2 — Scenario 1 Make.com Workflow Canvas
Once submitted, Make.com triggers instantly — saving the record to Airtable and routing the applicant through the eligibility check router.

![Scenario 1 Workflow](Grant%20Eligibilty%20Workflow.jpg)

---

### ✅ Step 3 — Eligible Path: Automated Email
Applicants who pass all 5 criteria instantly receive a personalised email confirming eligibility, with a unique full application link, key review dates, and submission reference ID.

![Eligible Email](Grant%20Eligibilty%20Email.jpg)

---

### ❌ Step 4 — Ineligible Path: Workflow & Decline Email
Applicants who do not meet the criteria are routed to the fallback path — a decline email is sent automatically listing all 5 eligibility criteria and their submission reference.

![Ineligibility Workflow](Grant%20Ineligibility%20workflow.jpg)

![Ineligible Email](Grant%20Ineligibility%20Email.jpg)

---

## 📁 Scenario 2 — Full Application Collector

Eligible applicants complete the full grant application form. This triggers the second Make.com scenario which captures all data, generates an AI summary, creates a CRM record, and sends a confirmation email.

### 📝 Step 1 — Full Grant Application Form (Jotform)
The full application collects project title, long description, expected outcomes, total budget, itemised budget breakdown, and supporting document uploads.

![Full Application 1](Full%20Application%201.jpg)
![Full Application 2](Full%20Application%202.jpg)

---

### ⚙️ Step 2 — Scenario 2 Make.com Workflow Canvas
Make.com watches for new full application submissions, finds the existing Airtable record, saves all data, generates an AI summary via GPT-4o, creates a Monday.com CRM item, and sends a confirmation email.

![Scenario 2 Workflow](S2_Full%20Grant%20Application_updated.jpg)

---

### 📧 Step 3 — Application Received Confirmation Email
Once the full application is submitted, the applicant immediately receives a professional confirmation email with key dates, application summary, and contact details.

![Confirmation Email](Full%20Grant%20Application%20Email.jpg)

---

## 🗃️ Airtable Database

Every submission — from intake through to full application and AI summary — is stored in a single Airtable database, giving the team a real-time view of all applications and their statuses.

![Airtable A](Airtable%20_A.jpg)
![Airtable B](Airtable%20B.jpg)

---

## 📊 Monday.com CRM Pipeline

Every full application automatically creates a record in the Monday.com Grant Program board with company name, status, contact email, region, submission date, Airtable Record ID, AI summary, and scoring columns.

![Monday CRM](Monday%20CRM_new.jpg)

---

## 🏆 Key Benefits for NGOs

| # | Benefit | Impact |
|---|---------|--------|
| 01 | **Save 80%+ of Staff Time** | Eligibility checks, emails, database entry and CRM updates all happen automatically |
| 02 | **Consistent, Bias-Free Screening** | Every applicant assessed against the same 5 criteria — no human error |
| 03 | **Applicant Experience Excellence** | Instant personalised responses build trust and professionalism |
| 04 | **Single Source of Truth** | All data in one Airtable database and one Monday.com board |
| 05 | **AI-Powered Review Efficiency** | GPT-4o briefs reduce reviewer reading time and speed up decisions |

---

## 👩‍💻 Author

**Gloria Njorteah**
AI & Automation Specialist

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/glorianjorteah)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Glorious75)

---

## 📄 License

This project is licensed under the **MIT License** — feel free to use and adapt for your own nonprofit automation projects.

---

> *"Automating grant management so nonprofits can focus on what matters most — their mission."*
>
> — Gloria Njorteah | TechBridge Foundation | 2026
