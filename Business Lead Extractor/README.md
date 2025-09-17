
# 🕵️‍♂️ Business Lead Extractor

An automated workflow built in **n8n** that generates Google Maps search queries, scrapes business URLs, extracts emails from websites, and stores qualified leads in Airtable. Perfect for local lead generation, outreach, or market research.

---

## 📸 Workflow Overview  
<!-- Add your image below this line -->
![Workflow Diagram](../Assets/business_lead_scraper_main_workflow.png?raw=true "Business Lead Extractor Screenshot")

![Workflow Diagram](../Assets/business_lead_scraper_sub_workflow.png?raw=true "Business Lead Extractor Screenshot")

---

## 🔄 How It Works

1. **📌 Airtable Trigger**  
   The workflow starts when a new **business type** and **location** are added to Airtable.

2. **🧠 AI Query Generator**  
   An AI agent generates properly formatted **Google Maps search queries** by combining the business type with all subregions of the specified city.

3. **🌐 Google Maps Scraping**  
   Each query is looped through to make an HTTP request to Google Maps.  
   The workflow parses the HTML and **filters out unrelated links**, keeping only business-related URLs.

4. **🔍 Website Visit & Email Extraction**  
   The workflow visits each business website and extracts **email addresses** using regex and content parsing.

5. **📁 Airtable Storage**  
   All extracted emails and business info are stored back in Airtable for easy access and follow-up.

---

## 🛠️ Tech Stack

- **n8n** – Workflow orchestration  
- **OpenAI / Gemini** – Query generation  
- **Airtable** – Input and output database  
- **HTTP Request + HTML Parser** – Scraping logic  
- **Regex** – Email extraction

---

## 🎯 Use Cases

- Local business lead generation  
- Outreach campaigns for agencies or startups  
- Market research and competitor mapping  
- CRM enrichment workflows

---

## 📌 Notes

- Queries are formatted as `{Business}+in+{Subregion}` using `+` instead of spaces  
- Subregions are dynamically fetched based on the city input  
- Email extraction logic can be extended to include phone numbers or contact forms

---

> Built as part of my journey to become an AI automation specialist.  
> More workflows coming soon!

