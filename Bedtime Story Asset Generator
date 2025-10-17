# 🌙 Bedtime Story Asset Generator

A modular, multi-agent storytelling pipeline built in **n8n** that generates **titles, subjects, images, narratives, sound effects, and lullabies** for children’s stories. Designed for scalability, creativity, and real-world production of multimedia storytelling assets.

---

## 📸 Workflow Overview  
<!-- Add your image below this line -->
Watch the demo (Click the image below)!  
[![Watch the demo](../Assets/story_generator_main_workflow.png)](https://drive.google.com/drive/u/1/folders/your-demo-folder-link)

Screenshots of the Workflow:  

![Workflow Diagram](../Assets/story_generator_main_workflow.png?raw=true "Story Generator Main Workflow")

![Workflow Diagram](../Assets/story_generator_titles.png?raw=true "Generate Titles Workflow")

![Workflow Diagram](../Assets/story_generator_subjects.png?raw=true "Generate Subjects Workflow")

![Workflow Diagram](../Assets/story_generator_images.png?raw=true "Generate Images Workflow")

![Workflow Diagram](../Assets/story_generator_sfx.png?raw=true "Generate SFX Workflow")

![Workflow Diagram](../Assets/story_generator_lullaby.png?raw=true "Generate Lullaby Workflow")

![Workflow Diagram](../Assets/story_generator_save_assets.png?raw=true "Save Assets Workflow")

---

## 🧠 Core Architecture

The system is composed of two main layers:

### 1. **Parent Orchestrator**
- Listens for incoming webhook triggers  
- Routes requests to the correct generation workflow (titles, subjects, images, audio, etc.)  
- Ensures structured flow and consistency across all assets  

### 2. **Child Workflows (Modular Generators)**
Each child workflow is a standalone generator for a specific asset type. The orchestrator invokes one or more of these based on the request.

---

## 🧩 Workflow Breakdown

### 🎨 Generate Titles Webhook
- Generates story titles inspired by trending and beloved children’s themes  
- Produces multiple titles based on the requested number  

---

### 🧸 Generate Subjects Webhook
- Generates subjects derived from the chosen title  
- Supports multiple subjects depending on the requested count  

---

### 🖼️ Generate Images Webhook
- Creates themed illustrations for each subject  
- Generates both **awake** and **asleep** versions  

---

### 🔄 Regenerate Image Webhook
- Re-generates a specific subject’s image if needed  
- Maintains consistent art style and prompts  

---

### 📖 Generate Story Narratives Webhook
- Produces a complete story (opening → subject narratives → closing)  
- References photo descriptions for both awake and asleep versions  

---

### 🎶 Generate SFX Webhook
- Generates sound effects for each subject or scene  
- Logs outputs in Google Sheets for tracking  

---

### 🎼 Generate Lullaby Webhook
- Creates custom lullabies based on story themes  
- Saves audio and links it to the correct story  

---

### 💾 Save Assets Webhook
- Collects and organizes all generated outputs  
- Saves to Google Drive with structured naming  

---

## 📊 Status Check Workflows

Each generation step has a paired status check to monitor progress and confirm completion:

- 🖼️ Multiple Image Status Check  
- 🔄 Regenerate Image Status Check  
- 🎶 SFX Status Check  
- 🎼 Lullaby Status Check  
- 💾 Save Assets Status Check  

---

## 🛠️ Tech Stack

- **n8n** – Workflow orchestration  
- **Lovable** – Frontend integration  
- **OpenAI / Gemini / Claude** – Text generation and orchestration  
- **Seedream / Suno / ElevenLabs** – Audio generation (SFX + lullabies)  
- **Google Drive / Google Sheets / Google Docs** – Asset storage and logging  
- **Custom APIs** – Image generation and pipeline integration  

---

## 🎯 Use Cases

- Automated children’s story production  
- Scalable multimedia content creation  
- Educational storytelling pipelines  
- Creative asset generation for apps, games, or media  

---

## 📌 Notes

- Each webhook is **modular**—can be triggered independently  
- Status checks ensure transparency and reliability  
- Assets are consistently linked and stored for easy retrieval  

---

> Built as part of my journey to become an AI automation specialist.  
> More workflows coming soon!  
> Inspired by modular agent design principles.
