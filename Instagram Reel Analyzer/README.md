
# 🎥 Instagram Reel Analyzer

An automated workflow built in **n8n** that fetches viral Instagram Reels, transcribes them, and uses an AI agent to analyze performance drivers. Designed for creators, marketers, and analysts who want to reverse-engineer virality and improve content strategy.

---

## 📸 Workflow Overview  
<!-- Add your image below this line -->
<img src="../Assets/ig_reel_analyzer.png?raw=true" alt="Instagram Reel Analyzer Screenshot" width="1000"/>


---

## 🔄 How It Works

1. **⏰ Scheduled Trigger**  
   The workflow runs on a schedule and pulls a list of Instagram accounts from Airtable.

2. **📈 Viral Reel Fetching**  
   For each account, it fetches their **top 10 most viral Reels** from the past few weeks.

3. **🎙️ Transcription**  
   Each video is transcribed to extract spoken content and captions.

4. **🧠 AI Agent Analysis**  
   The agent evaluates each Reel using a structured framework:
   - **Topic Fit**: Is it trending, solving a pain point, or sparking relatable reactions?  
   - **Hook Quality (0–2s)**: Does it grab attention instantly?  
   - **Retention Drivers (2–20s)**: Pacing, structure, captions—what keeps viewers watching?  
   - **Payoff & CTA**: Is there a strong finish and a clear call to action?

---

## 📊 Output Format

The analysis is delivered in three parts:
1. **Viral Diagnosis**: Highlights performance drivers and weak spots  
2. **Framework Table**: Maps key elements with evidence and improvement notes  
3. **Strategic Advice**: Written in a punchy, conversational style with strong verbs, vivid nouns, and emphasis on numbers

All results are stored back in Airtable for easy review and future strategy.

---

## 🛠️ Tech Stack

- **n8n** – Workflow orchestration  
- **Instagram API / Scraper** – Reel data fetching  
- **Transcription Tool** – Audio-to-text conversion  
- **Google Gemini / OpenAI** – AI analysis  
- **Airtable** – Input and output database

---

## 🎯 Use Cases

- Content creators looking to improve engagement  
- Social media managers analyzing performance trends  
- Agencies building data-backed content strategies  
- AI builders exploring media analysis workflows

---

## 📌 Notes

- The framework is modular—can be adapted to other platforms like TikTok or YouTube Shorts  
- Transcription can be enhanced with speaker detection or caption overlays  
- Strategic advice is optimized for clarity and actionability

---

> Built as part of my journey to become an AI automation specialist.  
> More workflows coming soon!

