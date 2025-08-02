# 🎧 InTune – AI Roommate Compatibility Platform  
*A SheBuilds 2025 Hackathon Project by Team Naruto*

![React](https://img.shields.io/badge/Frontend-React-blue?logo=react)
![Firebase](https://img.shields.io/badge/Auth-Firebase-orange?logo=firebase)
![ML](https://img.shields.io/badge/AI-NLP%20%2B%20CosineSimilarity-green)
![Status](https://img.shields.io/badge/Version-1.0-brightgreen)
![Hackathon](https://img.shields.io/badge/Built%20For-SheBuilds%202025-%23e91e63)

---

## 🚀 What is InTune?

**InTune** is a voice-powered AI platform that helps users find emotionally and practically compatible roommates. Built for the real world — where trust, comfort, and communication matter — InTune ensures **secure onboarding**, **AI-powered matching**, **anonymous chatting**, **room decor suggestions**, and **expense tracking**, all in one seamless flow.

> 🧠 **Think Tinder meets LinkedIn, but for roommates — with AI listening to your vibe.**

---

## ✨ Key Features

| 🔹 Feature            | 🧩 Description |
|----------------------|----------------|
| **Secure Onboarding** | Aadhaar OCR Verification to block fake users |
| **VoiceMatch**        | Voice-based onboarding using Omnidim assistant |
| **AI Matching Engine**| SBERT + cosine similarity + custom logic |
| **MatchMeter**        | Top 5 matches with visual score breakdown |
| **ChatterBox**        | Anonymous, passkey-protected real-time chat |
| **StyleMatch**        | AI-powered room decor suggestions using uploaded room photos |
| **Roommate Gallery**  | Upload happy stories + photos post-match |
| **SplitMate**         | Expense tracker to fairly split shared costs |
| **Admin Dashboard**   | Moderation, reports, match control |
| **GuideBot**          | GPT-powered conflict resolution assistant |

---

## 🧠 How It Works (User Flow)

```mermaid
graph TD
A[Landing Page + Signup] --> B[OCR Aadhaar Verification]
B --> C[Voice Survey via Omnidim]
C --> D[Webhook to Express.js Backend]
D --> E[ML Matching Engine]
E --> F[MatchMeter Results]
F --> G[Anonymous Chatroom]
G --> H[Yes/No Confirmation]
H --> I{YES}
I --> J[StyleMatch]
I --> K[Roommate Gallery]
I --> L[SplitMate]
L --> M[Admin Dashboard]
````

---

## 🛠️ Tech Stack

| Layer              | Technology Used                                                     |
| ------------------ | ------------------------------------------------------------------- |
| **Frontend**       | React.js, Tailwind CSS, Framer Motion                               |
| **Backend**        | Express.js (Node.js)                                                |
| **Authentication** | Firebase Auth + Anonymous ID Generator                              |
| **Voice Survey**   | Omnidim.io + Webhook                                                |
| **OCR**            | EasyOCR + OpenCV                                                    |
| **Database**       | MongoDB Atlas, Firebase Firestore                                   |
| **AI Matching**    | sentence-transformers (`MiniLM`), cosine similarity, custom scoring |
| **Chat System**    | Firebase Realtime DB + chatroom passkey system                      |
| **Decor AI**       | Replicate API + OpenAI GPT                                          |
| **Conflict Bot**   | GPT 3.5 (GuideBot)                                                  |
| **Deployment**     | Vercel (Frontend), Render/Railway (Backend)                         |

---

## 🔐 Security & Privacy

* ✅ Aadhaar-based real name verification
* ✅ Anonymous user IDs until match is confirmed
* ✅ Chat encryption and access control
* ✅ Admin monitoring for reports and issues

---

## 🖥️ Screenshots / Demo

> Coming soon! (or insert screenshots here using markdown)

---

## 📂 Project Structure

```
/frontend    - React app
/backend     - Express API + webhook + ML model
/ML_Model    - Matching engine (Python: SBERT + logic)
utils/       - OCR, matching helpers
artifacts/   - Saved encoder, scaler, embeddings
```

---

## 🤝 Team Naruto – SheBuilds 2025

| Member        | Role                        |
| ------------- | --------------------------- |
| Lekhni Bakiwal | Voice Match + ML + OCR      |
|Suhani Gupta | Frontend (React + Tailwind) |
| Nnadani Goyal | Chat + Admin Panel          |


---

## 🧪 Run Locally

```bash
# clone repo
git clone https://github.com/YOUR_USERNAME/InTune.git

# frontend
cd frontend
npm install
npm run dev

# backend
cd ../backend
npm install
node server.js

# ML model (Python)
cd ../ML_Model
pip install -r requirements.txt
python match.py
```

---

## 💡 Future Plans

* 📱 Add mobile-first PWA
* 🌍 Multi-language voice onboarding
* 🎯 Personalized roommate tips after match
* 🛡️ Video KYC + AI moderation

---

## 📬 Feedback?

> Feel free to open issues or drop feedback!
> Let’s make AI roommate matching **emotional, ethical, and exciting**! 💜

---
