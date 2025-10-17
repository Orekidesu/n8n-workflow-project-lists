
---

# 🌙 Bedtime Story Generator

An automated storytelling pipeline built in **n8n** that generates **titles, subjects, illustrations, narratives, sound effects, and lullabies** for children’s bedtime stories. Designed for scalability, creativity, and real-world multimedia production.

---
## [📑 (Click To) View Website Screenshots](https://www.dropbox.com/scl/fi/0ncw2ab8kwx9osm39jd9m/BedTime-Story-Asset-Generator.pdf?rlkey=gc9r6sw6139wugubrodufn2nh&st=2wkszq4d&dl=0)

## 📸 Workflow Overview  
<!-- Add your image below this line -->

### Generate Titles and Subjects Webhooks
![Workflow Diagram](../Assets/Bedtime%20Stories%20Assets/Workflow%20Images/bedtime_story_titles_subjects.png?raw=true "Generate Subjects Workflow")
### Generate Multiple Images Webhook
![Workflow Diagram](../Assets/Bedtime%20Stories%20Assets/Workflow%20Images/bedtime_story_generate_images.png?raw=true "Generate Subjects Workflow")
### Regenerate Image Webhook
![Workflow Diagram](../Assets/Bedtime%20Stories%20Assets/Workflow%20Images/bedtime_story_regenerate_image.png?raw=true "Generate Subjects Workflow")
### Generate Story Narative Webhook
![Workflow Diagram](../Assets/Bedtime%20Stories%20Assets/Workflow%20Images/bedtime_story_story.png?raw=true "Generate Subjects Workflow")
### Generate Sound Effects Webhook
![Workflow Diagram](../Assets/Bedtime%20Stories%20Assets/Workflow%20Images/bedtime_story_sfx.png?raw=true "Generate Subjects Workflow")
### Generate Audio Lullaby Webhook
![Workflow Diagram](../Assets/Bedtime%20Stories%20Assets/Workflow%20Images/bedtime_story_lullaby.png?raw=true "Generate Subjects Workflow")
### Save All Assets to Google Drive Webhook
![Workflow Diagram](../Assets/Bedtime%20Stories%20Assets/Workflow%20Images/bedtime_story_save_assets.png?raw=true "Generate Subjects Workflow")

### Generate/Regenerate Status Check Webhook
![Workflow Diagram](../Assets/Bedtime%20Stories%20Assets/Workflow%20Images/bedtime_story_generate_regenerate_images_status_check.png?raw=true "Generate Subjects Workflow")

### Sound Effects and Lullaby Images Status Check Webhook
![Workflow Diagram](../Assets/Bedtime%20Stories%20Assets/Workflow%20Images/bedtime_story_sfx_lullaby_status_check.png?raw=true "Generate Subjects Workflow")

### Save Assets Status Check Webhook
![Workflow Diagram](../Assets/Bedtime%20Stories%20Assets/Workflow%20Images/bedtime_save_assets_status_check.png?raw=true "Generate Subjects Workflow")




---

## 🔄 How It Works

1. **🎨 Title Generation**  
   AI generates story titles inspired by trending and beloved children’s themes. Multiple titles can be created at once.

2. **🧸 Subject Creation**  
   Subjects are generated based on the chosen title, with support for multiple characters or objects.

3. **🖼️ Image Generation**  
   Each subject is illustrated in both **awake** and **asleep** versions, maintaining a consistent art style.

4. **📖 Narrative Writing**  
   A full story is composed with an opening, subject-based narratives, and a closing.

5. **🎶 Sound Effects**  
   AI generates child‑friendly sound effects to match subjects or scenes, logged in Google Sheets.

6. **🎼 Lullaby Creation**  
   A custom lullaby is composed to accompany the story, saved and linked to the correct narrative.

7. **💾 Asset Saving**  
   All outputs (titles, subjects, images, audio, story text) are organized and stored in Google Drive.

8. **📊 Status Checks**  
   Each generation step has a paired status check workflow to confirm progress and completion.

---

## 🛠️ Tech Stack

- **n8n** – Workflow orchestration  
- **OpenAI / Gemini / Claude** – Text generation and orchestration  
- ** Suno / ElevenLabs** – Audio generation (SFX + lullabies)  
- **Seedream** – Illustration/Image generation  
- **Google Drive / Google Sheets / Google Docs** – Asset storage and logging  

---
---

## 🎯 Use Cases

### 🎬 Content Creation & Media
- **YouTube Story Videos** – Generate illustrated short stories (fairy tales, myths, sci‑fi, etc.) with narration and background audio.  
- **Animated Explainers** – Use the same pipeline to create educational explainers with visuals + voiceover.  
- **Podcast + Visuals** – Pair generated audio with simple images for YouTube “podcast with visuals” style uploads.  

---

### 📚 Education & Learning
- **Language Learning Stories** – Create bilingual storybooks with text, narration, and images for learners.  
- **History or Science Stories** – Generate illustrated “mini‑documentaries” for classrooms or e‑learning platforms.  
- **Interactive Quizzes** – Add branching narratives where each subject leads to a different outcome.  

---

### 🎮 Games & Apps
- **Visual Novels / Interactive Stories** – Generate characters, scenes, and dialogue for lightweight story‑driven games.  
- **Children’s Apps** – Daily “new story” content with images, narration, and lullabies.  
- **Gamified Learning** – Turn lessons into illustrated adventures with sound effects.  

---

### 🎨 Marketing & Engagement
- **Brand Storytelling** – Companies can generate fun illustrated stories featuring their mascots or products.  
- **Social Media Content** – Quick illustrated reels or shorts with narration and music.  
- **Personalized Gifts** – Parents or teachers could generate custom stories with a child’s name and likeness.  

---

## 🛠️ Why It’s Flexible
Because each step is modular (title → subject → image → audio → save), you can swap out:
- **The theme** (bedtime → horror → comedy → educational)  
- **The output channel** (storybook → YouTube → podcast → app)  
- **The asset type** (illustrations → stock photos → 3D renders → background music)  

--- 

---

## 📌 Notes

- Each webhook is modular and can be triggered independently  
- Status checks ensure transparency and reliability  
- Assets are consistently linked and stored for easy retrieval  
- The system is extensible — new asset types (e.g., background music, translations) can be added without disrupting the core flow  

---

