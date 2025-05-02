# HackInia-Spark-7-2025-Pragati



# 🧑‍⚖️ NyayaMitra – Your AI-Powered Legal Companion

**NyayaMitra** is an AI-powered chatbot built on **Retrieval-Augmented Generation (RAG)**, designed to make **Indian legal knowledge** accessible, understandable, and trustworthy for every citizen.

From the **Indian Penal Code (IPC)** to **RTI**, **labor laws**, and **FIR procedures**, NyayaMitra breaks down complex legal concepts and delivers **clear, citation-backed answers** — just like a reliable legal companion would.

---

## 🚀 Features

- ✅ **Ask Legal Questions**: Understand your rights under IPC, RTI, labor, and criminal laws.
- 🔎 **Cite-Based Answers**: Every answer comes with references from official legal texts.
- 🤖 **Powered by LLaMA 2 + RAG**: Uses LLaMA 2 as the base LLM with real-time retrieval of legal documents.
- 📍 **Find Nearby Lawyers**: Users can discover verified lawyers around them.
- 📬 **Lawyer Registration & Profile Upload**: Lawyers can register themselves and upload credentials.
- 💳 **Subscription System**: Lawyers can subscribe and get listed after profile review.
- 🛡️ **Privacy & Local Processing**: Runs on-device using Ollama, ensuring low cost and privacy.

---

## 🧱 Tech Stack

| Layer            | Technology Used                   |
|------------------|------------------------------------|
| **Frontend**     | React.js, Bootstrap                |
| **Backend**      | Flask, Python                      |
| **AI**           | LLaMA 2, LangChain, FAISS, Ollama  |
| **Deployment**   | Localhost                          |

---

## 🧠 How It Works (RAG + LLaMA 2)

NyayaMitra uses **Retrieval-Augmented Generation (RAG)** architecture:

1. **User inputs a legal question**
2. **Legal documents (IPC, RTI, etc.)** are searched using **FAISS**
3. The top relevant docs are sent with the prompt to **LLaMA 2**
4. **NyayaMitra generates a contextual, accurate, and citation-backed response**

> All of this happens locally with **Ollama**, making it affordable, fast, and privacy-friendly.

---

## 📲 User Flows

### 👤 For Citizens:
- Ask legal questions via chat
- Get clear, accurate, law-based answers
- Find and contact nearby lawyers

### ⚖️ For Lawyers:
- Register via the **“Become a Lawyer”** form
- Upload details, documents, and select subscription plan
- Post-approval, appear in the public **“Find a Lawyer”** directory

---
## 📂 Project Structure
📁 Project Root

├── GENERATOR/                        # Backend for legal notice generation
│   ├── __pycache__/                 # Compiled Python bytecode
│   │   └── legal_notice_generator.cpython-*.pyc
│   ├── generated/                   # Folder to store generated documents
│   ├── static/                      # Static assets like CSS
│   │   └── style.css
│   ├── templates/                   # HTML templates
│   │   └── index.html
│   ├── utils/                       # Utility scripts and files
│   │   ├── __pycache__/
│   │   └── docx_template.docx       # Template for legal notice generation
│   ├── app.py                       # Flask application entry point
│   ├── generate_notice.py           # Logic for generating notices
│   └── legal_notice_generator.py    # Main legal notice logic

├── front_end/                       # Frontend (React + TypeScript)
│   ├── node_modules/                # Node dependencies
│   ├── public/                      # Public assets
│   ├── src/
│   │   ├── components/              # Reusable UI components
│   │   │   ├── contexts/            # React context API for state management
│   │   │   ├── data/
│   │   │   │   └── lawyersData.ts   # List of lawyers
│   │   │   ├── ui/                  # UI-specific components
│   │   │   │   ├── ContactForm.tsx
│   │   │   │   ├── ContactInfo.tsx
│   │   │   │   ├── Features.tsx
│   │   │   │   ├── FloatingContactButton.tsx
│   │   │   │   ├── Footer.tsx
│   │   │   │   ├── Hero.tsx
│   │   │   │   ├── InteractiveImage.tsx
│   │   │   │   ├── LawyerCard.tsx
│   │   │   │   ├── LoadingAnimation.tsx
│   │   │   │   ├── LoadingScreen.tsx
│   │   │   │   ├── Navbar.tsx
│   │   │   │   ├── PageLayout.tsx
│   │   │   │   ├── Process.tsx
│   │   │   │   ├── ProductPlatform.tsx
│   │   │   │   ├── ProjectPageLayout.tsx
│   │   │   │   ├── Projects.tsx
│   │   │   │   └── SEO.tsx
│   ├── package.json                 # Node dependencies and scripts
│   └── tsconfig.json                # TypeScript configuration
