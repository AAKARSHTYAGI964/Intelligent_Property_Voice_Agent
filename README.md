# 🏡 Project Title: Intelligent Property Voice Agent

## 📌 Overview

**Intelligent Property Voice Agent** is a real-time AI-powered conversational assistant designed to streamline real estate sales interactions through natural voice conversations.

The system is capable of:

* Conducting live microphone-based voice conversations
* Detecting speech using Voice Activity Detection (VAD)
* Transcribing speech into text with Faster-Whisper
* Understanding customer intent using the Gemini API
* Extracting structured business entities from conversations
* Classifying leads into different sales stages
* Managing interruptions seamlessly during conversations
* Generating executive-level Minutes of Meeting (MoM) after every call

This project demonstrates an end-to-end conversational AI pipeline that combines speech processing, natural language understanding, structured reasoning, and CRM-oriented business intelligence.

---

# What this project showcases

The project highlights:

* Real-time audio processing
* Intelligent conversational reasoning
* Automated lead qualification
* Stateful session memory
* Post-call business analytics
* Modular API-driven architecture

---

# ⚙️ Setup Instructions

## ❓How do I run the project?

Follow the steps below to get the application running locally.

---

## 🟢 Step 1: Install Python

Install **Python 3.10 or later** from:

https://www.python.org/downloads/

Verify the installation:

```bash
python --version
```

---

## 🟢 Step 2: Clone the Repository

```bash
git clone https://github.com/AAKARSHTYAGI964/Intelligent_Property_Voice_Agent.git
cd Intelligent_Property_Voice_Agent
```

---

## 🟢 Step 3: Create a Virtual Environment

```bash
python -m venv venv
```

Activate the virtual environment:

**Windows**

```bash
venv\Scripts\activate
```

**Linux/macOS**

```bash
source venv/bin/activate
```

---

## 🟢 Step 4: Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 🟢 Step 5: Configure Environment Variables

Create a `.env` file in the project's root directory.

Add your Gemini API credentials:

```text
GEMINI_API_KEY=your_gemini_api_key_here
reasoning_key=your_gemini_api_key_here
mom_key=your_gemini_api_key_here
```

---

## 🟢 Step 6: Launch the Voice Assistant

```bash
python src/main.py
```

Once the application starts, it will:

* Welcome the user
* Listen through the microphone
* Respond using synthesized speech
* Generate a structured MoM after the conversation concludes

---

# 🏗 System Architecture

![System Architecture](docs/mermaid-diagram.png)

---

# 🛠 Technology Stack

### Telephony

* Asterisk
* SIP (Zoiper)

### AI & Natural Language Processing

* Google Gemini API
* Faster-Whisper (Speech-to-Text)
* Prompt Engineering

### Speech Processing

* Voice Activity Detection (VAD)
* Piper TTS (Text-to-Speech)

### Backend

* Python
* FastAPI
* Uvicorn

### System Design

* Session Management
* Lead Qualification Engine
* Conversation Memory Tracking
* Post-Call Intelligence Generator

---

# 🧠 Core Features

### ✔ Intent Detection

Automatically identifies customer intents, including:

* Property Inquiry
* Pricing Inquiry
* Site Visit Request
* Objection Handling
* Call Termination

### ✔ Structured Entity Extraction

Captures key customer information such as:

* Budget
* Preferred Location
* Property Configuration (2BHK, 3BHK, Villa)
* Purchase Timeline
* Investment Type

### ✔ Lead Stage Classification

Classifies each conversation into one of the following stages:

* new
* qualified
* hot
* needs_followup
* closed

### ✔ Natural Interruption Handling

When a customer starts speaking while the assistant is responding:

* Speech synthesis stops immediately.
* The assistant instantly switches back to listening mode.

### ✔ Executive Minutes of Meeting (MoM)

At the end of every conversation, the system automatically generates a structured report containing:

* Executive Summary
* Customer Requirements
* Key Discussion Points
* Customer Objections
* Lead Assessment
* Recommended Action Items
* Sentiment Analysis



# 🚀 Future Enhancements

Planned improvements include:

* Native RTP streaming support
* Token-level response streaming
* Multi-language conversational support
* Cloud deployment on AWS or Azure
* CRM and database integration

---

# 👨‍💻 Developed By

Aakarsh Tyagi
