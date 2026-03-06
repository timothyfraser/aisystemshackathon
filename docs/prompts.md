![](images/banner_thin.png)
---

# 🗨️ Prompts

[**This document**](https://github.com/timothyfraser/aisystemshackathon/blob/main/docs/prompts.md) will be updated at the start of the Hackathon event to contain 3 short prompts. Teams will be asked to pick 1 prompt and design an AI-powered tool around it. Please check back at kickoff for details!

---

## Quick Links

- 💡 [The Challenge](https://github.com/timothyfraser/aisystemshackathon/blob/main/docs/prompts.md#-the-challenge)
- ⚙️ [Requirements](https://github.com/timothyfraser/aisystemshackathon/blob/main/docs/prompts.md#-requirements)
- 🗨️ [Example Prompt](https://github.com/timothyfraser/aisystemshackathon/blob/main/docs/prompts.md#-example-prompt)
- ⏰ [Prompts](https://github.com/timothyfraser/aisystemshackathon/blob/main/docs/prompts.md#-prompts)
- 💬 [Frequently Asked Questions (FAQs)](https://github.com/timothyfraser/aisystemshackathon/blob/main/docs/prompts.md#-frequently-asked-questions-faqs)
- 🔧 [Example Techniques](https://github.com/timothyfraser/aisystemshackathon/blob/main/docs/prompts.md#-example-techniques)
- 📚 [Resources for Building Your Tool](https://github.com/timothyfraser/aisystemshackathon/blob/main/docs/resources.md)
- 👍 [Advice](https://github.com/timothyfraser/aisystemshackathon/blob/main/docs/prompts.md#-advice)
- [🏠 Homepage](https://github.com/timothyfraser/aisystemshackathon/tree/main)

---

### 💡 The Challenge

Over 24 hours, your team will build and deploy a new **AI-powered system** in response to one of three prompts.

- 3 prompts released at kickoff — each tied to a stakeholder need that you will address
- Incorporate **generative AI** (e.g., OpenAI or Ollama Cloud) into your solution
- Build something functional and **demo-ready** (REST API, Dashboard, or other deployable app)
- Meet a specific stakeholder need in response to your chosen prompt

In this Hackathon, you will build a tool that uses AI to solve a real-world problem.

### ⚙️ Requirements

1. 🚀 **Possible Outputs**: A publicly available, deployable tool with:
   - A Dashboard (e.g., Shiny app in R or Shiny in Python)
2. 🤖 **Generative AI**: Your tool must incorporate queries to a generative AI model (OpenAI or Ollama Cloud, or similar).
3. 📈 **2–3 test datasets** that demonstrate the tool’s effectiveness. These can be synthetic but should represent real-world data your tool would use.
4. 📑 **A codebook and README** for your datasets and tool — what each file and variable means, and how to run the tool.

### 🗨️ Example Prompt

Prompts will be released at the start of the Hackathon on this page. Example style (solution-neutral; many different tools could address it):

> Design a system that helps a stakeholder monitor a key metric and get AI-generated summaries or recommendations. Provide synthetic data and a working demo (e.g., API or dashboard).

---

### 💡 Prompts

Please pick **1** of the following prompts below and create an AI-powered tool to address the problem. **Prompts will be released at kickoff on this page.**

*You do not need prior domain expertise. Use what you know and what you can find quickly to build a sensible, useful tool.*

When building your tool, refer to the [**🔢 Evaluation Criteria**](https://github.com/timothyfraser/aisystemshackathon/blob/main/docs/criteria.md) and 📚 [**Resources for Building Your Tool**](https://github.com/timothyfraser/aisystemshackathon/blob/main/docs/resources.md).


#### Prompt 1 — Industrial Logistics
**AI-Augmented Delivery System**

A global logistics company is struggling to track shipments in real time, predict delivery delays, and optimize warehouse routing across multiple distribution centers.

Your team's job is to build an AI-augmented delivery database system that uses synthetic logistics data to create live tracking profiles and generate actionable predictions for operations managers.

You pick the domain — everyday packages, semiconductor supply chains... or even beanie babies. If it ships, you can track it.

**Example Queries**
- *"Which shipments are at highest risk of missing their delivery window in the next 48 hours?"*
- *"Under current warehouse load, when will Fulfillment Center B reach full capacity?"*
- *"How does this shipment's route compare to historical cases with similar delay risk factors?"*

**Reference Data**
- Design your own shipment/order schema (e.g., shipment ID, origin, destination, status, timestamps, delay flags - up to you!) and generate synthetic records.

---

#### Prompt 2 — Digital Health
**Patient Digital Twins**

A regional hospital network is struggling to allocate ICU beds, predict readmissions, and manage appointment no-shows.

Your team's job is to build a data-driven platform that uses synthetic patient data to create 'digital twin' profiles and generate actionable predictions for clinical decision-makers.

**Example Queries**
- *"Which patients in this cohort are at highest risk of 30-day readmission?"*
- *"Under today's admission forecast, when will ICU capacity reach 90%?"*
- *"How does this patient's profile compare to historical cases with similar risk factors?"*

**Reference Data**
- Design your own patient schema (e.g., patient ID, age, diagnosis codes, admission date, vitals, risk scores - up to you!) and generate synthetic records. 

---

#### Prompt 3 — NYC Urban Risk
**Urban Early Warning System**

The NYC Department of Emergency Management needs to act before small signals turn into citywide crises. Weather, hospital capacity, and transit data all exist — but they are disconnected and difficult to analyze together.

Your team's job is to build a cloud-based AI decision-support system that stores and analyzes structured data organized by neighborhood and time, and surfaces AI-generated risk summaries for decision-makers.

**Example Queries**
- *"Which neighborhoods show rising heat and hospital strain?"*
- *"How does today compare to similar historical patterns?"*
- *"Where is the risk accelerating the fastest?"*

**Reference Data**
- Design your own neighborhood-level schema (e.g., zip code, date, temperature index, hospital capacity %, transit delay index, composite risk score - up to you!) and generate synthetic time-series data representing different scenarios across NYC neighborhoods.

---

### 🔧 How to Build It

We recommend structuring your project around four components — but build it however works for your team.

**1. Data Ingestion** — Get data into your system:
- Synthetic data generator
- CSV uploads

**2. Database** — Store your data in a structured way. A good schema usually covers:
- Entities — shipments, patients, neighborhoods
- Events / signals — time-series updates
- Predictions — risk scores, capacity forecasts

**3. Backend API** — Wire up ingestion, predictions, and query results with Plumber (R) or FastAPI (Python).

**4. Dashboard** — A simple Shiny app to query your system and display results.

---

### 🖥️ Recommended Tech Stack

| Layer | Tool |
|-------|------|
| Frontend | Shiny (R or Python) |
| Backend API | Plumber (R) or FastAPI (Python) |
| Database | Supabase (PostgreSQL) |
| AI | OpenAI API or Ollama Cloud |


---

### 💬 Frequently Asked Questions (FAQs)

- **I signed up for one topic in the signup survey. Can I pick a different topic?** Yes.
- **How long do I have to pick a topic?** Pick your topic within the first 15–30 minutes of the Hackathon and then stick to it so you have maximum build time.
- **Where do I find tutorials?** 📚 [Resources for Building Your Tool](https://github.com/timothyfraser/aisystemshackathon/blob/main/docs/resources.md)

### 🔧 Example Techniques

- Storing and querying data (e.g., Supabase/PostgreSQL)
- Descriptive Statistics on Chunks of Big Data
- Quality Control Analytics
- Building and calling REST APIs
- Querying generative AI (OpenAI API, Ollama Cloud)
- Prompt engineering for summaries, recommendations, or classifications
- RAG (Retrieval Augmented Generation)

### 👍 Advice

- This project is short-term. Define a narrow scope so you can finish on time.
- A small product that works is better than a large one that doesn’t.
- Delegate: use your team — different people can own data, API, AI, and deployment.
- Use the optional trainings early (Query AI, Supabase, API, Cursor, Posit Connect) to unblock yourself.

---

![](images/banner_icons.png)

<p align="center">
  <b><a href="https://github.com/timothyfraser/aisystemshackathon/tree/main">🏠 Return to Home Page</a></b>
</p>
