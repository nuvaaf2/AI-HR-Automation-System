<div align="center">

# 👥 AI-Powered HR Automation System

### End-to-End AI Hiring Pipeline — From Resume Screening to Interview Scheduling

[![n8n](https://img.shields.io/badge/Built%20with-n8n-FF6D00?style=for-the-badge&logo=n8n&logoColor=white)](https://n8n.io)
[![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4.1-412991?style=for-the-badge&logo=openai&logoColor=white)](https://openai.com)
[![Telegram](https://img.shields.io/badge/Telegram-Bot-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://telegram.org)
[![BeyondPresence](https://img.shields.io/badge/BeyondPresence.ai-AI%20Screening-6C3CE1?style=for-the-badge&logoColor=white)](https://beyondpresence.ai)

*Candidates apply via Telegram, AI screens their resume, shortlists the best fits, and automatically schedules interviews — no HR team needed.*

</div>

---

## 📌 Overview

This end-to-end HR automation pipeline replaces the manual, time-consuming parts of early-stage hiring. Candidates submit their resume through a **Telegram bot**, which triggers a fully automated AI workflow: GPT-4.1 parses and scores the resume, shortlists qualified candidates, and schedules interviews automatically — all without any manual HR effort.

---

## ✨ Features

- 🤖 **Telegram Bot Interface** — Candidates submit resumes directly via a conversational Telegram bot
- 📄 **Automatic PDF Extraction** — Parses resume content from uploaded PDF files
- 🧠 **AI Resume Screening** — GPT-4.1 scores candidates based on job requirements, skills, and experience
- ✅ **Smart Shortlisting** — Automatically filters and ranks qualified candidates
- 📅 **Interview Scheduling** — Sends interview invitations with time slots to shortlisted candidates
- 📧 **Offer Letter Generation** — Auto-generates and sends offer letters for selected candidates
- 🔄 **Full Onboarding Trigger** — Kicks off onboarding workflow upon acceptance

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| **n8n** | Workflow automation engine |
| **OpenAI GPT-4.1** | Resume analysis & candidate scoring |
| **Telegram Bot API** | Candidate-facing application interface |
| **Gmail API** | Sending interview & offer letter emails |
| **Webhook** | Triggering workflow stages |
| **PDF Parser** | Extracting text from resume PDFs |
| **Beyond Presence API** | Uses an AI interviewer to take interviews |

---

## 🔄 How It Works

```
Candidate sends resume PDF to Telegram Bot
        ↓
Webhook triggers n8n workflow
        ↓
PDF content extracted and parsed
        ↓
GPT-4.1 analyzes resume vs job requirements
        ↓
Candidate scored & shortlisted (or rejected)
        ↓
[If shortlisted] Interview invitation sent via Telegram/Email
        ↓
[If selected] Offer letter generated & sent
        ↓
Onboarding workflow triggered
```

---

## 🚀 How to Use

### Prerequisites
- [n8n](https://n8n.io) (self-hosted or cloud)
- OpenAI API key
- Telegram Bot Token (via [@BotFather](https://t.me/botfather))
- Gmail account
- Beyond Presence ([https://www.beyondpresence.ai](https://www.beyondpresence.ai/))

### Setup Steps

1. **Clone this repository**
   ```bash
   git clone https://github.com/nuvaaf2/ai-hr-automation.git
   cd ai-hr-automation
   ```

2. **Import the workflow**
   - Open your n8n instance
   - Go to **Workflows → Import from file**
   - Select `hr-automation-workflow.json`

3. **Configure credentials**
   - Add your **OpenAI API key** in n8n credentials
   - Add your **Telegram Bot Token**
   - Set up **Gmail** credentials for email delivery
   - Configure your **Webhook URL** in n8n

4. **Customize job requirements**
   - Open the workflow in n8n
   - Edit the AI prompt node to match your specific job description and screening criteria

5. **Activate the workflow**
   - Toggle to **Active**
   - Share your Telegram bot link with candidates

---

## 📂 Repository Structure

```
ai-hr-automation/
├── hr-automation-workflow.json   # n8n workflow export
```

---

## 📸 Workflow Preview

> <img width="1138" height="709" alt="image" src="https://github.com/user-attachments/assets/f1b62e7f-921f-4e9b-b236-6a110d88084a" />


---

## 🔮 Future Improvements

- [ ] Multi-role hiring support (different pipelines per job)
- [ ] ATS (Applicant Tracking System) integration
- [ ] Interview feedback collection via Telegram
- [ ] Analytics dashboard for hiring funnel

---

## 👤 Author

**Nuvaaf A N** — AI Automation Engineer | n8n Builder

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin)](https://www.linkedin.com/in/nuvaaf-a-n-0b53a5341/)
[![GitHub](https://img.shields.io/badge/GitHub-nuvaaf2-181717?style=flat&logo=github)](https://github.com/nuvaaf2)

---

<div align="center">
⭐ If you found this useful, please star the repo!
</div>
