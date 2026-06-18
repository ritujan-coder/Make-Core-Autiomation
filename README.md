# Make-Core-Auoomation
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

---

# ⚡ Project 3: Webhook-Triggered AI Email & Logging Pipeline

An instant, event-driven Make.com workflow designed to process real-time incoming webhooks, leveraging AI for content generation, automating Gmail draft creations, and maintaining centralized logging.

## 📊 Workflow Structure & Logic

1. **Custom Webhooks:** Acts as an instant, real-time trigger that catches data immediately when an external event occurs.
2. **OpenAI GPT (Module 3):** Dynamically processes the incoming webhook payload to structure or generate customized content based on prompt instructions.
3. **Gmail (Create a Draft):** Automatically crafts and structures a professional email draft using the AI-generated response.
4. **Google Sheets (Add a Row):** Logs the operational metadata, webhook details, and system responses into a tracking spreadsheet for audits.

## 🛠️ Tech Stack & Concepts Used
* **Instant Triggers:** Working with custom webhooks for zero-latency automation.
* **AI Content Generation:** Transforming raw payload data into contextual email copy.
* **Cross-Platform Synchronization:** Chaining communication channels (Gmail) with databases (Google Sheets) smoothly.

## 🖼️ Workflow Diagram
<img width="1920" height="1020" alt="Screenshot 2026-06-15 164831" src="https://github.com/user-attachments/assets/3ca8c52e-9b1b-4cec-83bb-78892d3fe84e" />
<img width="1920" height="1020" alt="Screenshot 2026-06-15 164429" src="https://github.com/user-attachments/assets/0817971b-749b-450f-ac37-d53c51134aff" />

---

# 📊 Project 4: Multi-Stage AI Content Filtering & Email Pipeline

A highly optimized Google Sheets triggered workflow featuring multi-stage OpenAI context processing and execution filters for targeted email drafting.

## 📊 Workflow Structure & Logic

1. **Google Sheets (Watch New Rows):** Triggers automatically whenever a new row of raw data or user input is logged.
2. **Execution Filters:** Advanced logical constraints placed between modules to ensure only qualified data passes to the AI processing stage.
3. **OpenAI GPT (Module 2 - Initial Processing):** Analyzes the raw sheet inputs to synthesize core concepts, draft initial copy, or categorize intent.
4. **OpenAI GPT (Module 3 - Refinement & SEO):** Takes the output of the first AI model, reviews it, and refines it into a polished, professional messaging layout.
5. **Gmail (Create a Draft):** Automatically compiles the multi-stage refined AI response into a structured, ready-to-send email draft.

## 🛠️ Tech Stack & Concepts Used
* **Data Guardrails:** Implementing Make.com filters between modules for criteria validation.
* **Sequential AI Refinement:** Chaining two distinct LLM layers to improve final copy quality.
* **Asynchronous Execution:** Seamlessly transforming static spreadsheet data into active marketing assets.

## 🖼️ Workflow Diagram
<img width="1920" height="1020" alt="Screenshot 2026-06-15 164943" src="https://github.com/user-attachments/assets/bb1be96a-1944-4c67-b8fe-4d9f04473b8a" />
<img width="1920" height="1020" alt="Screenshot 2026-06-15 164928" src="https://github.com/user-attachments/assets/e3f6dcb9-00c6-4031-a8c1-8b595c8b3eea" />
