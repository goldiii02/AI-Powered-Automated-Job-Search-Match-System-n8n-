# 🚀 AI-Powered Automated Job Search & Match System (n8n)

An end-to-end AI-driven job search automation workflow built using **n8n**.  
This system automatically fetches jobs, filters them based on user profile, removes duplicates, and emails personalized job opportunities daily.

---

## ✨ Features

- 🔍 Fetch jobs from multiple sources (Arbeitnow, Naukri-ready)
- 🧠 User profile–based filtering
- 🧹 Automatic duplicate removal
- 📊 Job data normalization
- 📧 Daily automated email alerts
- ⏰ Fully scheduled automation
- 🆓 Built using mostly free APIs

---

## 🏗️ Workflow Architecture

User Profile Form → Validation → Store Profile  
↓  
Daily Scheduler → Fetch Jobs → Combine Jobs  
↓  
Split → Normalize → Remove Duplicates  
↓  
Aggregate → Send Email Report

---

## ⚙️ Tech Stack

- **n8n** — workflow automation  
- **Groq / OpenAI compatible models** — AI matching  
- **Arbeitnow API** — job source  
- **Gmail API** — email notifications  
- **JavaScript (n8n expressions)**

---

## 📬 How It Works

1. User submits profile (skills, roles, resume)
2. Scheduler runs daily
3. System fetches latest jobs
4. Jobs are filtered and deduplicated
5. Top matches are emailed automatically

---

## 🧪 Demo Use Case

Ideal for:

- Job seekers  
- Automation engineers  
- AI workflow enthusiasts  
- n8n learners

---

## 🚀 How to Run Locally

1. Import the provided workflow JSON into n8n  
2. Configure credentials:
   - Gmail
   - Job APIs
3. Add your user profile
4. Activate the workflow

---

## 📌 Future Improvements

- LinkedIn job integration
- Advanced AI scoring
- Multi-user support
- Web dashboard

---

## 👨‍💻 Author

**Goldi Rathore**  
Automation Engineer | AI Workflow Builder

---

⭐ If you found this useful, give the repo a star!
