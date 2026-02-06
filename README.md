# 🤖 n8n AI Automation Portfolio

This portfolio showcases **production-grade AI automation systems** built with **n8n**, focused on **real-world business use cases** such as voice agents, browser automation, RAG knowledge systems, content pipelines, email automation, and video publishing.

These projects reflect how **modern AI automation agencies** design, deploy, debug, and scale intelligent systems.

---

## 🚀 What This Portfolio Demonstrates

* Designing **production-ready n8n workflows**
* Building **AI agents** with tools, memory, and decision logic
* Implementing **RAG (Retrieval-Augmented Generation)** using vector databases
* Automating **voice, browser, email, content, inventory, and video pipelines**
* Integrating **OpenAI, Pinecone, Gmail, Google Sheets, OneDrive, LinkedIn, RunwayML, YouTube, Airtop, ElevenLabs, Vapi, and WhatsApp APIs**
* Solving real-world engineering problems (webhooks, parsing, validation, tunneling, orchestration)

---

## 📂 Projects

### (Ordered by Real-World Use, Complexity & Engineering Depth)

---

## 1. AI Voice-Powered Restaurant Ordering System ☎️🍔 **(FLAGSHIP PROJECT)**

A **full Voice-to-Action AI agent** that replaces a human restaurant order-taker.

The system answers phone calls, understands menu questions, takes complex orders, and instantly notifies the restaurant owner via **WhatsApp and Email**.

### Real-World Use Case

Designed for **restaurants, cafes, and food chains** to automate phone orders without human staff.

---

### Tech Stack

* **Voice AI:** Vapi.ai (GPT-4o-mini)
* **Automation Brain:** n8n (local)
* **Connectivity:** ngrok (secure tunneling)
* **Knowledge Base:** Pinecone (RAG over PDF menu)
* **Messaging:** Wassenger (WhatsApp), Gmail API

---

### How the Workflow Operates

1. Customer calls the AI phone number
2. AI answers and converses naturally
3. Menu questions are answered using **RAG from Pinecone**
4. Order intent is detected
5. Structured customer data is sent via webhook
6. n8n processes, validates, and formats the order
7. Instant notifications sent via:

   * 📱 WhatsApp (owner)
   * 📧 Email (receipt)

---

### Key Engineering Challenges Solved

* Fixed webhook failures due to **incorrect HTTP headers**
* Parsed **stringified JSON tool arguments** using `JSON.parse()`
* Prevented API crashes with **input validation & regex cleaning**
* Diagnosed missing **Node.js environment (ENOENT)**
* Routed live internet traffic to localhost using **ngrok**
* Built a production-grade **voice → AI → automation pipeline**

**Outcome:**
A live, working prototype used by calling the agent and receiving real-time order notifications.

---

## 2. AI Browser Automation & Web Research Agent 🌐🧠

An advanced AI system that can **open real browsers, navigate websites, interact with UI elements, extract data, and answer user queries autonomously**.

Used in **research, ops, scraping, and automation-heavy workflows**.

---

### A. Browser Session Manager

**Workflow**

* `Browser.json`

**Features**

* Real browser sessions via Airtop
* CAPTCHA handling
* Persistent profiles
* Live rendering (1280×720)
* Multi-workflow orchestration

**Tech Stack:** Airtop API, n8n

---

### B. AI Web Search & Interaction Agent

**Workflow**

* `Searcher.json`

**Capabilities**

* Browse, search, click, type, scroll
* Extract structured data
* Maintain memory across steps
* Auto-cleanup browser sessions

**Tech Stack:** OpenAI (GPT-4o-mini), Airtop API, LangChain Agents & Memory, n8n

---

## 3. AI-Generated Video Automation (Idea → Video → YouTube 🎥)

A **fully hands-free video creation and publishing pipeline**.

**Workflow**

* `AI Generated Videos.json`

**Features**

* Reads ideas from Google Sheets
* Generates cinematic prompts
* Creates videos using RunwayML
* Uploads to YouTube automatically
* Tracks publishing status

**Tech Stack:** OpenAI, RunwayML, Google Sheets, YouTube API, n8n AI Agents

---

## 4. AI Voice / Natural Language Email Agent ✉️🎙️

A webhook-driven AI agent that accepts **voice or text commands** and autonomously sends professional emails.

**Workflow**

* `voice-agent.json`

**Features**

* Voice input via ElevenLabs
* AI-powered drafting
* Recipient resolution via Google Sheets
* Gmail-based delivery
* Hands-free assistant-style UX

**Tech Stack:** OpenAI, ElevenLabs, Gmail API, Google Sheets, LangChain Tools, n8n

---

## 5. RAG Knowledge Base (Chat with Private Data)

A private AI system that allows users to **chat with their own documents**.

**Workflows**

* `rag-ingestion.json`
* `rag-chat.json`

**Features**

* OneDrive ingestion
* Chunking & embeddings
* Pinecone vector search
* Hallucination prevention

**Tech Stack:** OpenAI, Pinecone, OneDrive, n8n AI Agents

---

## 6. Smart Email Manager (Inbox Zero)

An intelligent inbox automation system for creators and businesses.

**Workflow**

* `email-classifier.json`

**Features**

* Email classification
* AI-generated replies
* Gmail draft creation for review

**Tech Stack:** OpenAI, Gmail API, n8n

---

## 7. AI-Powered LinkedIn Post Generator 📢

An end-to-end LinkedIn content automation workflow.

**Workflow**

* `linkedin-post-generator.json`

**Features**

* Research agent
* Unicode-optimized content
* AI image generation
* Automatic posting via LinkedIn API

**Tech Stack:** OpenAI, LinkedIn API, n8n AI Agents

---

## 8. Inventory Management Agent

An AI-powered inventory assistant using natural language.

**Workflow**

* `inventory-agent.json`

**Tech Stack:** OpenAI, Google Sheets, LangChain, n8n

---

## 9. Simple Mail Sender

A lightweight natural-language email sender.

**Workflow**

* `gmail-sender.json`

**Tech Stack:** OpenAI, Gmail API, n8n

---

## 🛠️ Setup & Usage

1. Open **n8n**
2. Add Workflow → Import from File
3. Import the required `.json` workflows
4. Configure credentials (not included)

---

## 🔐 Required Credentials

* OpenAI
* Pinecone
* Google Cloud (Gmail & Sheets)
* Microsoft OneDrive
* LinkedIn API
* RunwayML
* YouTube API
* Airtop API
* ElevenLabs API
* Vapi.ai
* Wassenger (WhatsApp)

---

## 📌 Notes

* Built for **real businesses, not demos**
* Modular, scalable, and extensible
* Covers **voice AI, agents, RAG, browser automation, and media pipelines**
* Mirrors production systems used by AI automation agencies

---

## 📄 License

Licensed under the **MIT License**.
