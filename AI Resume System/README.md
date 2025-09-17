# 🧠 AI Resume Screening System

An automated resume screening workflow built in **n8n**, designed to evaluate candidates using AI agents and structured logic. This system helps recruiters and hiring teams save time while maintaining consistent, explainable evaluation standards.

---

## 📸 Workflow Overview  
<!-- Add your image below this line -->
![AI Resume System Workflow Image](../Assets/resume_screening_system.png?raw=true "AI Resume System Screenshot")

---

## 🔄 How It Works

1. **📥 Form Submission Trigger**  
   Candidates submit their **name**, **email**, and **resume file** (PDF or DOCX) via a form.

2. **📄 Resume Text Extraction**  
   The uploaded file is parsed to extract clean, structured text.

3. **🧠 AI Agent Analysis**  
   The resume is evaluated against a job description using an AI agent.  
   The agent performs a structured review:
   - Strengths  
   - Weaknesses  
   - Risk Factor (e.g. gaps, mismatches)  
   - Reward Factor (e.g. standout traits)  
   - Overall Fit Rating

4. **✅ Decision Logic**  
   - If the candidate **passes**, their data is saved to Airtable, they receive a **“You passed!”** email, and the recruiter gets a **Telegram alert**.  
   - If the candidate **doesn’t pass**, they receive a polite rejection email.

---

## 🛠️ Tech Stack

- **n8n** – Workflow orchestration  
- **Google Gemini / OpenAI** – Resume analysis  
- **Airtable** – Candidate data storage  
- **Gmail** – Email notifications  
- **Telegram Bot** – Recruiter alerts

---

## 🎯 Use Cases

- Automate initial resume screening  
- Maintain consistent evaluation criteria  
- Save time for recruiters and HR teams  
- Build scalable, explainable hiring logic

---

## 📌 Notes

- The AI agent uses structured prompts to ensure consistent analysis.  
- The system is modular—easily extendable to include interview scheduling, CRM syncing, or multi-role screening.

---

> Built as part of my journey to become an AI automation specialist.  
> More workflows coming soon!


