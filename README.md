# 🧠 HealthcareLLM Chatbot MVP

A mental health assistant chatbot built using AnythingLLM and ChatGPT API, designed to support residents in **Halifax, Nova Scotia** with mood self-assessment and self-care strategies — based on validated tools like the **PHQ-9** and local mental health resources.

## 💡 Project Objective

The goal of this MVP is to build a helpful, empathetic chatbot that:
- Helps users identify signs of depression using the PHQ-9 self-assessment
- Offers supportive guidance and self-care strategies based on official CMHA and Nova Scotia Health materials
- Refers users to professional help or crisis support when needed
- Can run locally or via cloud-based APIs, with full RAG (retrieval-augmented generation) capability using AnythingLLM

## 🧠 Chatbot Capabilities

- Explains what depression is and how to identify it
- Guides users to complete the **PHQ-9** form independently
- Interprets PHQ-9 total scores with appropriate disclaimers
- Triggers immediate safety warnings if **Question 9** suggests self-harm risk
- Refers users to **local crisis lines and services** (e.g., 1-888-429-8167)
- Uses a supportive, non-diagnostic tone with strong ethical boundaries

## 🗂️ Folder Structure

```
/healthcarellm-chatbot-mvp
├─ knowledge_base/               # Key source materials (PDFs, markdown, txt)
│  ├─ NSH_Depression_Info.md
│  ├─ CMHA_SelfCare_Strategies.txt
│  ├─ PHQ-9_English.pdf
│  └─ PHQ9_Scoring_Guide.md
├─ prompt/
│  └─ system_prompt.md           # The full LLM prompt used for assistant setup
├─ documentation/
│  ├─ use_case_description.md    # Describes real-world scenario and user journey
│  └─ scenario_pack.md           # (Provided by instructors)
├─ demo/
│  ├─ demo_video.mp4             # Optional screen recording of chatbot interaction
└─ README.md                     # You're reading it!
```

## 🛠️ Tech Stack

- [AnythingLLM](https://github.com/Mintplex-Labs/anything-llm)
- Ollama/LLM local models
- Node.js, npm
- Markdown, PDF, TXT as RAG source formats

## 🚀 Setup Instructions

1. Clone the repo and install [Node.js](https://nodejs.org/)
2. Install & run [AnythingLLM](https://github.com/Mintplex-Labs/anything-llm)
3. Configure your **LLM provider** (OpenAI API key or local Ollama model)
4. Upload documents in `knowledge_base/` and `prompt/` folders to AnythingLLM
5. Test using provided scenario:  
   > *"I’ve been feeling down for a few weeks — how can I tell if it’s depression?"*

## 🧷 Ethics & Boundaries

- No personal data is stored or collected.
- The assistant does **not** provide medical advice or diagnoses.
- Any user response indicating **self-harm** (PHQ-9 Q9 > 0) triggers an immediate referral to crisis support.

## 📍 Key Local Resource

**Nova Scotia Provincial Mental Health and Addictions Crisis Line**  
📞 1-888-429-8167 (available 24/7)

---

## 📝 License

This project is for educational use only. All external documents are used under fair use for research and public health education.

---
