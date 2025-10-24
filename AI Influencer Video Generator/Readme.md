# 🎥 AI Influencer Video Generator  

An automated content pipeline built in **n8n** that transforms a single Telegram message into a full week of influencer‑style short videos. From script generation to MP4 creation, captioning, and storage, this workflow is designed for scalability, reliability, and hands‑off social media production.  


## 📸 Workflow Overview  
<!-- Add your images below this line -->

### Telegram Trigger & Script Preparation  
![Workflow Diagram](../Assets/AI%20Influencer%20Assets/Workflow%20Images/telegram_trigger.png?raw=true "Telegram Trigger Workflow")  

### Script Selection & Validation  
![Workflow Diagram](../Assets/AI%20Influencer%20Assets/Workflow%20Images/script_selection.png?raw=true "Script Selection Workflow")  

### Image Fetching & Base64 Conversion  
![Workflow Diagram](../Assets/AI%20Influencer%20Assets/Workflow%20Images/image_fetching.png?raw=true "Image Fetching Workflow")  

### Video Generation Sub‑Workflow  
![Workflow Diagram](../Assets/AI%20Influencer%20Assets/Workflow%20Images/video_generation.png?raw=true "Video Generation Workflow")  

### Save Videos to Google Drive & Update Sheet  
![Workflow Diagram](../Assets/AI%20Influencer%20Assets/Workflow%20Images/save_assets.png?raw=true "Save Assets Workflow")  

### Error Handling & Spam Protection  
![Workflow Diagram](../Assets/AI%20Influencer%20Assets/Workflow%20Images/error_spam_protection.png?raw=true "Error Handling Workflow")  

---

## 🔄 How It Works  

1. **💬 Telegram Trigger**  
   User sends a weekly summary message to the Telegram bot, which kicks off the workflow.  

2. **✍️ Script Generation**  
   AI generates 7 short, handheld selfie‑style scripts (one per day) in the influencer’s voice.  

3. **📨 Script Selection**  
   The bot sends scripts back to the user for review. The user can select, cancel, or retry. Invalid inputs are caught gracefully.  

4. **🖼️ Image Preparation**  
   The system fetches background images from a fixed library, downloads them from Google Drive, and converts them to Base64.  

5. **🎬 Video Generation**  
   Scripts + images are combined and sent to the **VEO 3.1 API** for 8‑second video generation.  

6. **📁 Asset Storage**  
   Generated MP4s are saved into a dated weekly folder in Google Drive.  

7. **📝 Logging**  
   Scripts, captions, hashtags, and status updates are logged in Google Sheets for transparency.  

8. **🚫 Spam Protection**  
   If a user tries to send new prompts while a process is running, the bot replies with a polite “⏳ Please wait, generation is still in progress.”  

9. **✅ Completion Notice**  
   Once all videos are ready, the bot notifies the user that assets are complete and ready for review.  

---

## 🛠️ Tech Stack  
- **n8n** – Workflow orchestration and automation logic  
- **OpenAI / ChatGPT** – Script generation in influencer voice  
- **VEO 3.1** – Video generation from scripts and images  
- **Google Drive** – Stores all generated MP4s in weekly folders  
- **Google Sheets** – Logs scripts, captions, hashtags, and status  
- **Telegram Bot API** – User input, notifications, and anti‑spam safeguards  

---

## 🎯 Use Cases  

### 📱 Social Media Automation  
- Weekly influencer content generation with zero manual editing  
- Batch‑produced short‑form videos for TikTok, Instagram, or YouTube Shorts  

### 🏢 Agencies & Teams  
- Manage multiple influencer accounts with scalable automation  
- Provide clients with consistent, ready‑to‑publish content  

### 🎨 Brand & Marketing  
- AI‑driven brand mascots or personalities posting weekly updates  
- Campaigns with automated video storytelling  

### 👤 Creators & Entrepreneurs  
- Solo creators who want to focus on ideas, not editing  
- Automated pipelines for niche content (fitness tips, comedy skits, product demos)  

---

## 🛠️ Why It’s Flexible  
Because each step is modular (trigger → script → image → video → save), you can swap out:  
- **The input channel** (Telegram → Slack → Web form)  
- **The video engine** (VEO → Runway → Pika)  
- **The storage/logging** (Google Drive/Sheets → Notion → Airtable)  

---

## 📌 Notes  
- Each step is modular and can be triggered independently  
- Error handling and spam protection ensure reliability  
- Assets are consistently linked and stored for easy retrieval  
- The system is extensible — new environments, prompts, or video services can be added without disrupting the core flow  

---

