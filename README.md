# Make-Core-Autiomation
"Collection of my intermediate Make.com automation workflows including OpenAI, Webhooks, and Google Sheets integrations."

<img width="1917" height="935" alt="Screenshot 2026-06-14 104656" src="https://github.com/user-attachments/assets/ca00d22b-f694-4932-9c51-ee7b1bae9f10" />


# 🤖 AI-Powered Amazon Affiliate Content Engine

An advanced Make.com workflow that automates product research, AI content generation, data logging, and social media publishing.

## 📊 Workflow Structure & Logic

1. **HTTP Module (RapidAPI):** Fetches real-time trending products from Amazon India (Query: `summer dress`) using custom API headers.
2. **OpenAI GPT (Module 42):** Generates high-converting, keyword-rich Pinterest descriptions optimized for SEO (< 500 chars).
3. **OpenAI GPT (Module 45):** Creates catchy, searchable Pinterest titles optimized for high click-through rates (< 100 chars).
4. **Tools (Set Variable):** Automatically appends custom affiliate tracking tags (`?tag=fashionhu013f-21`) to raw Amazon URLs to build tracking links.
5. **Google Sheets:** Logs all data into structured columns (Product Name, Price, AI Descriptions, and Generated Affiliate Links) for internal tracking.
6. **Pinterest Integration:** Automatically creates and posts a fresh Pin on the dedicated board with custom descriptions, target affiliate links, and product images.

## 🛠️ Tech Stack & Concepts Used
* **API Integration:** Custom HTTP handling with RapidAPI headers (`X-RapidAPI-Key`).
* **Sequential AI Chaining:** Multi-step prompt dependency inside Make.com.
* **Data Cleansing:** Variable lifetime mapping and text manipulation.
* **Database Management:** Auto-logging structures via Google Sheets API.
