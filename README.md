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


---

# 🔀 Project 2: Router-Based Conditional Data Pipeline

A logic-driven Make.com scenario that demonstrates conditional routing, data filtering, and multi-branch segregation based on source criteria.

## 📊 Workflow Structure & Logic

1. **Google Sheets (Watch Rows):** Acts as the automated trigger, instantly capturing new incoming rows of unorganized data.
2. **Router Module:** Evaluates the incoming data attributes against specific pre-defined filter criteria (e.g., separating leads by departments like Marketing, Software, or Ecommerce).
3. **Tools (Set Variable Branches):** Dynamically processes and re-assigns localized variables based on the successful route, isolating data streams for precise backend operations.

## 🛠️ Tech Stack & Concepts Used
* **Advanced Routing:** Implementing multi-route logical forks inside Make.com.
* **Data Filtering:** Setting up exact matching conditions to control scenario paths.
* **State Management:** Using the Tools module to handle runtime variables dynamically.

## 🖼️ Workflow Diagram
<img width="1920" height="1080" alt="Screenshot 2026-06-15 162710" src="https://github.com/user-attachments/assets/bce0fe95-ba9c-4dbb-b235-a3cf0c78a949" />
<img width="1920" height="1080" alt="Screenshot 2026-06-15 162634" src="https://github.com/user-attachments/assets/6e7a96bd-844d-44a6-92fc-541a9198794a" />
