# 🧠 Recursive Understanding Engine (RUE)

> **"If an answer is given, understanding is not automatically achieved."** > RUE is a pedagogical system that guarantees true conceptual clarity by breaking complex topics into recursive, interactive, load-bearing building blocks.

Built for the **HackMarch 2.0 Hackathon** | Sponsor: **BuilderThinking**

---

## 📸 System Interface

*(Add your screenshots here! Make sure to use the Light Mode ones with the Green/Blue tags)*

![Knowledge Map & Mastery Interface](./path-to-your-screenshot1.png)
*RUE mapping the prerequisites for Photosynthesis, adapting difficulty, and tracking mastery.*

---

## ✨ Core Features

RUE is not just a chatbot wrapper; it is an opinionated learning orchestration engine.

* **🎯 Intelligent Concept Extraction:** Uses Google Gemini to extract only "load-bearing" prerequisites, ignoring common filler words and reducing cognitive load.
* **🧬 Recursive Knowledge Graph:** Users can click on extracted concepts to go infinitely deeper, visually mapping their learning journey.
* **🧠 ELI5 Adaptive Logic:** As users reach deeper cognitive layers (Depth > 3), the backend dynamically alters the system prompt to use "Explain Like I'm 5" metaphors, preventing jargon fatigue.
* **✅ Mastery Progress Tracking:** A live checklist mathematically tracks a user's completion of a specific conceptual layer before they move on.
* **⚡ Live Backend Caching:** Built-in `node-cache` ensures that previously explored concepts load in 0ms, drastically reducing LLM API costs at scale.
* **📥 Markdown Study Guide Export:** Traverses the user's recursive click-history to compile a perfectly formatted Markdown study document.
* **👁️ 100% AI Transparency:** A clean UI toggle allows users to view the exact system prompts, token compute costs, and model architecture in real-time.

---

## 🛠️ Tech Stack

**Frontend (The UI & Graph)**
* **React.js**: For interactive state management and dynamic routing.
* **Framer Motion**: For buttery-smooth, zero-clutter animations.
* **React Markdown**: To elegantly format the LLM's educational prose.

**Backend (The Reasoning Engine)**
* **Node.js & Express**: Lightning-fast REST API architecture.
* **Google Generative AI SDK**: Utilizing `gemini-2.5-flash-lite` (via Gemini 1.5 Flash backend) for low-latency inference.
* **Strict JSON Schema (`responseSchema`)**: Forces the LLM to output highly-structured data payloads instead of unpredictable text.
* **Node-Cache**: For API cost-optimization and instant retrieval of common queries.

---

## 🚀 Getting Started

### Prerequisites
* Node.js (v16 or higher)
* A Google Gemini API Key
