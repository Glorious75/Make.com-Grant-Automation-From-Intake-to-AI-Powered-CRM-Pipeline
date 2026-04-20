# Make.com Grant Automation: From Intake to AI-Powered CRM Pipeline
AI-powered grant intake &amp; eligibility automation system built for TechBridge Foundation using Make.com, Jotform, Airtable, OpenAI GPT-4o, Monday.com &amp; Gmail. Automates eligibility screening, AI summarisation and CRM pipeline management — saving nonprofits 80%+ admin time.

> **Built for TechBridge Foundation | Prepared by Gloria Njorteah**

![Make.com](https://img.shields.io/badge/Make.com-6D00CC?style=for-the-badge&logo=make&logoColor=white)
![Jotform](https://img.shields.io/badge/Jotform-FF6100?style=for-the-badge&logo=jotform&logoColor=white)
![Airtable](https://img.shields.io/badge/Airtable-18BFFF?style=for-the-badge&logo=airtable&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI_GPT--4o-412991?style=for-the-badge&logo=openai&logoColor=white)
![Monday.com](https://img.shields.io/badge/Monday.com-FF3D57?style=for-the-badge&logo=monday&logoColor=white)
![Gmail](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)

---

## 📋 Table of Contents

- [Project Overview](#-project-overview)
- [System Architecture](#-system-architecture)
- [Scenario 1 — Eligibility Checker](#-scenario-1--grant-eligibility-checker)
- [Scenario 2 — Full Application Collector](#-scenario-2--full-application-collector)
- [Eligibility Criteria](#-eligibility-criteria)
- [Tech Stack](#-tech-stack)
- [Key Results](#-key-results)
- [Screenshots](#-screenshots)
- [Author](#-author)
- [License](#-license)

---

## 🌍 Project Overview

Nonprofit organisations running grant programmes face a significant administrative burden — manually reviewing applications, checking eligibility, communicating with applicants, and tracking submissions across scattered spreadsheets and inboxes.

This project delivers a **fully automated, AI-powered grant management system** built in **Make.com** for the **TechBridge Foundation Community Innovation Grant**.

### The Problem
| Challenge | Impact |
|-----------|--------|
| Manual eligibility screening | Hours wasted per application |
| Inconsistent decisions | Human error and bias |
| Delayed applicant communication | Damaged trust and reputation |
| Scattered data | No single source of truth |
| No pipeline visibility | Difficult reporting and decisions |
| Zero AI assistance | Reviewers read every page from scratch |

### The Solution
A two-scenario Make.com automation that handles everything from initial intake to CRM pipeline — **saving 80%+ of staff admin time** and delivering a professional applicant experience.

---

## 🏗 System Architecture

The system is built across **two Make.com scenarios** that work together seamlessly:

```
SCENARIO 1 — Grant Eligibility Checker
Jotform Intake → Airtable Database → Eligibility Router → Email + Status Update

SCENARIO 2 — Full Application Collector
Jotform Full App → Airtable Search → Save Data → GPT-4o Summary → Monday.com CRM → Gmail Confirmation
```

![System Workflow](./screenshots/combined_workflows.jpg)

---

## ✅ Scenario 1 — Grant Eligibility Checker

This scenario runs automatically the moment an applicant submits the intake form.

```
Step 1 → Intake Form Received (Jotform Webhook)
          Watches for new form submissions in real time

Step 2 → Save to Database (Airtable)
          Creates a new record with all applicant details

Step 3 → Eligibility Check (Router)
          Checks all 5 eligibility criteria automatically

         ┌─────────────────────────────────┐
         │                                 │
    ELIGIBLE PATH                   INELIGIBLE PATH
         │                                 │
Step 4a → Send Eligible Email        Step 4b → Send Decline Email
          (Personalised with                    (Lists all 5 criteria
           full application link)               and submission reference)
         │                                 │
Step 5a → Update Airtable Status     Step 5b → Update Airtable Status
          → "Eligible"                          → "Ineligible"
```

### 📧 Eligible Email includes:
- Personalised greeting
- Confirmation of eligibility
- Unique full application link
- Key dates (review deadline, decision date)
- Submission reference ID

### ❌ Ineligible Email includes:
- Respectful decline message
- All 5 eligibility criteria listed
- Applicant's submission reference
- Organisation and amount requested

---

## 📁 Scenario 2 — Full Application Collector

Triggered when an eligible applicant completes the full grant application form.

```
Step 1 → Watch for Submissions (Jotform)
          Monitors full application form for new submissions

Step 2 → Find Applicant Record (Airtable Search)
          Locates the existing intake record by organisation name

Step 3 → Save Full Application (Airtable Update)
          Updates the record with full project details, budget,
          outcomes, and supporting documents

Step 4 → Generate AI Summary (OpenAI GPT-4o)
          Generates a structured brief: applicant name,
          organisation, project title, funding request,
          and concise project description

Step 5 → Store AI Summary (Airtable Update)
          Saves the GPT-4o summary back to the Airtable record

Step 6 → Create CRM Item (Monday.com)
          Creates a new item in the Grant Program board with
          status "Under Review", region, contact email,
          Airtable Record ID, and scoring columns

Step 7 → Send Confirmation Email (Gmail)
          Sends "Application Received!" email with key dates,
          application summary, and contact information
```

---

## 🎯 Eligibility Criteria

An applicant must meet **all five criteria** to proceed to the full application:

| # | Criteria |
|---|----------|
| 1 | Organisation must be based in **CA, TX, NY, IL or GA** |
| 2 | Grant request must be **between $5,000 and $50,000** |
| 3 | Must be a **registered 501(c)(3) nonprofit** |
| 4 | Organisation must have been **operating for at least 2 years** |
| 5 | Must **not have received a TechBridge grant in the past 12 months** |

---

## 🛠 Tech Stack

| Tool | Purpose | Link |
|------|---------|------|
| **Make.com** | Automation platform — runs both scenarios | [make.com](https://make.com) |
| **Jotform** | Intake form and full application form | [jotform.com](https://jotform.com) |
| **Airtable** | Central database for all submissions | [airtable.com](https://airtable.com) |
| **OpenAI GPT-4o** | AI-generated application summaries | [openai.com](https://openai.com) |
| **Monday.com** | CRM pipeline for grant review | [monday.com](https://monday.com) |
| **Gmail** | Automated email communications | [gmail.com](https://gmail.com) |

---

## 🏆 Key Results

| # | Benefit | Impact |
|---|---------|--------|
| 01 | **Save 80%+ of Staff Time** | Eligibility checks, emails, database entry and CRM updates all happen automatically |
| 02 | **Consistent, Bias-Free Screening** | Every applicant assessed against the same 5 criteria — no human error |
| 03 | **Applicant Experience Excellence** | Instant personalised responses build trust and professionalism |
| 04 | **Single Source of Truth** | All data in one Airtable database and one Monday.com board |
| 05 | **AI-Powered Review Efficiency** | GPT-4o briefs reduce reviewer reading time and speed up decisions |

---

## 📸 Screenshots

### Scenario 1 & 2 — Make.com Workflow Canvas
![Combined Workflows](./screenshots/combined_workflows.jpg)

### Grant Intake Form (Jotform)
![Intake Form](./screenshots/intake_form.jpg)

### Eligible Email
![Eligible Email](./screenshots/eligible_email.jpg)

### Ineligible Email
![Ineligible Email](./screenshots/ineligible_email.jpg)

### Airtable Database
![Airtable](./screenshots/airtable_database.jpg)

### Monday.com CRM Pipeline
![Monday CRM](./screenshots/monday_crm.jpg)

### Application Received Confirmation Email
![Confirmation Email](./screenshots/confirmation_email.jpg)

> 📁 Add your screenshots to a `/screenshots` folder in this repository and update the paths above.

---

## 👩‍💻 Author

**Gloria Njorteah**
AI & Automation Specialist

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/glorianjorteah)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/glorianjorteah)

---

## 📄 License

This project is licensed under the **MIT License** — feel free to use and adapt for your own nonprofit automation projects.

---

> *"Automating grant management so nonprofits can focus on what matters most — their mission."*
>
> — Gloria Njorteah | TechBridge Foundation | 2026
