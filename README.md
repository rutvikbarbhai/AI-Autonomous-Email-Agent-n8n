
# <img src="https://github.com/user-attachments/assets/cf684a77-bb13-475a-9cba-b639ece52c8e" width="35" style="vertical-align: middle;" /> AI Autonomous Email Agent Using (n8n) Workflow Automation Platform 

An autonomous, goal-aware AI email assistant built using **n8n**, **Groq (LLaMA 3 70B)**, and **Google APIs** to reduce cognitive load during high-stakes academic and professional phases.

This system automatically:
- Reads incoming emails
- Understands semantic intent
- Checks real-time availability
- Aligns responses with long-term goals
- Drafts and sends replies autonomously

## <img src="https://github.com/user-attachments/assets/f3dcee8e-e008-457a-97fb-d3848b425713" height="30px" style="vertical-align:text-bottom;"> Repository Structure
```bash
AI Autonomous Email Agent Using (n8n) Workflow Automation Platform 
├── 📁 workflow
├── 📁 prompts 
├── 📁 docs
├── 📁 screenshots
└── README.md
```

## ✨ Problem Statement 
As a final-year undergraduate navigating the overlap of:
- academic closure,
- internships,
- placements,
- sponsorships, and
- professional collaborations,

I found myself spending excessive cognitive bandwidth parsing and responding to emails.
Existing solutions (filters, auto-replies) were:
- stateless,
- reactive,
- and unaware of personal priorities.

I wanted a system that could **reason, decide, and act autonomously** — similar to a human executive assistant.

## <img src="https://github.com/user-attachments/assets/d3a7713c-0fa3-4fba-a8b3-1cb60e4dafce"  height="25px" style="position: bottom;">  Objective
To design an autonomous AI system that can:
- understand email intent,
- reason using real-world context,
- make decisions aligned with long-term goals,
- act independently without human intervention.


## What This Agent Does ?
The agent performs a complete pipeline without human intervention.
```bash
Read → Reason → Decide → Act
```
![1](https://github.com/user-attachments/assets/86c5678a-7b84-4cdc-8986-fd248b5415e2)



## <img src="https://github.com/user-attachments/assets/dcdcffb4-c4e2-40ee-84cc-aca8612d257e" height="30px" style="vertical-align: text-bottom; margin-bottom:-3050px;">  Core Capabilities
- Semantic intent classification using LLMs
- Goal-aware decision making
- Temporal reasoning using calendar availability
- Autonomous response generation and dispatch

---

## <img src="https://github.com/user-attachments/assets/6672ee8c-15ed-4fb5-9cd5-63c04ac747c1" height="24px" style="vertical-align:bottom;"> System Architecture

### 1️⃣. Email Ingestion
- Triggered via **Gmail API**
- Extracts sender, subject, body, and metadata

### 2️⃣. Semantic Classification (LLM-based)
- Powered by **Groq’s LLaMA 3 70B**
- Classifies emails into:
  - `SPAM`
  - `PROMOTIONAL`
  - `EDUCATIONAL`
  - `SPONSORSHIP`
  - `IMPORTANT`

### 3️⃣. Context Awareness Layer
- **Google Calendar API**
  - Checks real-time schedule availability
- **Airtable**
  - Stores long-term goals and priorities
  - Acts as persistent memory

### 4️⃣. Autonomous Execution
- Crafts personalized, professional replies
- Sends responses automatically via **Gmail API**
- No manual review required

![2](https://github.com/user-attachments/assets/2741cef5-df47-4800-9ae3-22403d5f0160)

---

## Email Classification Logic

| Category       | Action Taken |
|----------------|--------------|
| SPAM           | Labeled, no response |
| PROMOTIONAL    | Labeled only |
| EDUCATIONAL    | Conditional response |
| SPONSORSHIP    | Goal-aligned response |
| IMPORTANT      | Immediate autonomous reply |

---

##  <img src="https://github.com/user-attachments/assets/612137fd-b2de-411c-acd7-f94c4811e9f2" height="30px" style="vertical-align:text-bottom;">Tech Stack

- **n8n** – Visual, event-driven workflow orchestration
- **Groq + LLaMA 3 70B** – High-throughput LLM for reasoning and generation
- **Gmail API** – Email ingestion and replies
- **Google Calendar API** – Temporal reasoning
- **Airtable** – Goal memory and personalization

---

## <img src="https://github.com/user-attachments/assets/dcdcffb4-c4e2-40ee-84cc-aca8612d257e" height="30px" style="vertical-align: text-bottom; margin-bottom:-3050px;"> Key Takeaways (What I learned in this process ?)

- Designing **memory-aware autonomous agents**
- Prompt engineering under dynamic system state
- Orchestrating multiple APIs into a cohesive agent
- Applying LLMs beyond text generation into decision engines
- Building real-world agentic systems using low-code infrastructure

---

## <img src="https://github.com/user-attachments/assets/cf684a77-bb13-475a-9cba-b639ece52c8e" width="35" style="vertical-align: middle;" /> AI Usage Disclosure

AI tools were used as **design collaborators** to:
- Validate system architecture
- Refine prompts and output schemas
- Reason about edge cases and safety constraints

All implementation decisions, workflows, and integrations were designed and executed manually.

---
> Note: Workflow JSON is instance-specific and can be shared upon request.
---

# <img src="https://github.com/user-attachments/assets/d91c2841-14ca-4283-a7fc-a93fc1e996af" height="22px" style="vertical-align:text-bottom;"> Screenshots

The screenshots included in this repository demonstrate:
## 1️⃣. End-to-end n8n workflow
![1](https://github.com/user-attachments/assets/c0b3e7bf-9a9b-4dcc-a046-f51ea052e718)

## 2️⃣. AI agent classification output
![2](https://github.com/user-attachments/assets/68120403-35c3-4e0a-9dc7-80f979e7a8e1)

## 3️⃣. Prompt configuration
![3](https://github.com/user-attachments/assets/dcd4c2d8-1dd1-45df-b0d3-182e57ac0f5c)

## 4️⃣. Gmail draft and send execution
![4](https://github.com/user-attachments/assets/155b0431-e142-4e98-8af3-db910cba6ba0)

These provide visual proof of the system operating in real conditions.

---

## <img src="https://github.com/user-attachments/assets/64abffeb-9a67-4e47-a3ec-69036aa3a343" height="25px" style="position: bottom;"> Disclaimer

- No credentials or secrets are included in this repository
- API keys and OAuth configurations must be set up locally
- This project is intended for educational and experimental purposes

---




