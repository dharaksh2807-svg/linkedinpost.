# 🚀 LinkedIn Post Pro (LinkedIn Translator)

[![Next.js](https://img.shields.io/badge/Next.js-15-black?style=for-the-badge&logo=next.js)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19-blue?style=for-the-badge&logo=react)](https://reactjs.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3-38B2AC?style=for-the-badge&logo=tailwind-css)](https://tailwindcss.com/)

## 📖 About the Project

**LinkedIn Post Pro** is an AI-powered satirical web application designed to poke fun at modern corporate networking culture. Have you ever noticed how a simple, everyday event on LinkedIn gets spun into a 5-paragraph essay about leadership, synergy, and relentless growth? This project automates that exact phenomenon.

You simply type in a blunt, honest statement (e.g., *"I overslept and missed my meeting"* or *"I got fired"*), and the AI instantly transforms it into an overly enthusiastic, buzzword-filled corporate monologue ready for your LinkedIn feed. 

This project was built to explore Large Language Models (LLMs) and prompt engineering in a fun, relatable way, showcasing how AI can adapt to specific, highly stylized tones of voice.

> 🔒 **Note:** The source code for this project is currently held in a private repository. This public repository serves as a showcase of the project's features and architecture.

**Experience the satire yourself:**
👉 **[Visit the Live Application](https://linkedinpostpro.vercel.app)** 👈

---

## ✨ Features

- **Instant Translation:** Type in plain English and instantly get a corporate-ready LinkedIn post.
- **Context Aware:** Provide optional context (like your job title or degree) for more personalized cringe.
- **AI-Powered:** Uses OpenAI / Groq (e.g., `gpt-4o-mini`, `llama-3.3`) for highly accurate LinkedIn-speak.
- **Local Fallback:** Works gracefully via a built-in local translation engine if the AI provider is temporarily unavailable.
- **Sleek UI:** Clean, responsive interface built with Tailwind CSS.

---

## 🛠 Technical Implementation & Tech Stack

Under the hood, the application is built for speed and simplicity. It leverages a serverless architecture to communicate with AI models while providing a seamless, fast UI.

- **Framework:** Next.js 15 (App Router)
- **UI Library:** React 19
- **Styling:** Tailwind CSS 3
- **AI/LLM:** OpenAI SDK interfacing with OpenAI or Groq

---

## 🔌 API Integration Overview

The application utilizes a powerful Next.js backend route to handle prompt engineering and translations efficiently. Here is a look at how the API functions under the hood:

**POST** `/api/translate`

**Example Request Payload:**
```json
{ 
  "text": "I overslept and missed my meeting.",
  "context": "Software Engineer" 
}
```

**Example Response:**
```json
{
  "translation": "Today, I embraced the power of unstructured time management. By pivoting my morning routine, I created space for strategic rest, allowing me to approach my engineering challenges with renewed synergy and vigor! 🚀💡 #GrowthMindset #TechLeadership #RestIsProductivity",
  "mode": "ai"
}
```
