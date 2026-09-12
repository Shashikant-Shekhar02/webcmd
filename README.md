# 🏥 AarogyaRoute — Autonomous Medical Concierge Browser Agent

> **SLAB Hackathon (VIT Bhopal Edition)**  
> *Built with Webcmd Architecture, Playwright, and Claude Code.*  
> **Core Thesis:** *Explore Once. Learn the Workflow. Enforce Responsible Human-in-the-Loop. Dispatch Live Care.*

---

## 📌 The Problem
Over 2 million patients travel across India annually for specialized tertiary medical care (orthopedics, cardiology, oncology, organ transplants). However, cross-referencing accredited NABH/JCI hospital specialists, calculating procedure estimates, and booking verified recovery lodging within 2 km of that exact hospital requires **4+ hours of manual, repetitive tab-switching**.

Standard LLM chatbots only return generic, hallucinated text. Pure vision agents burn 90,000+ tokens taking raw screenshots. **AarogyaRoute** replaces this friction with an autonomous browser agent that drives real websites, extracts structured DOM intelligence, and coordinates multi-portal logistics in under 45 seconds.

---

## 🏗️ System Architecture & Workflow

---

---

## 🚨 Hard Rules Compliance

1. **Live or Real Execution Verification:** The application launches a live, headed Chromium instance on screen during execution, with timestamped logs streamed via Server-Sent Events (SSE).
2. **Responsible AI & Human Approval:** Strictly adheres to the requirement that sensitive submissions, payments, and inquiry dispatches must contain a human approval step. The agent cannot proceed past Step 3 without manual authorization.

---

## 🛠️ Tech Stack

* **Browser Automation & CLI Infrastructure:** Playwright, `@agentrhq/webcmd` concepts
* **Backend API Server:** Node.js, Express, Server-Sent Events (SSE)
* **Frontend Dashboard:** Next.js / Tailwind CSS, Lucide Icons, Shadcn UI styling
* **Failsafe & Resilience:** Local JSON fallback adapter layer for 0% crash probability

---

## 🚀 Quick Start (Local Setup)

### Prerequisites
* Node.js v18+
* Google Chrome / Chromium

### Installation
```bash
# 1. Clone the repository
git clone [https://github.com/](https://github.com/)<your-username>/aarogya-route.git
cd aarogya-route

# 2. Install dependencies
npm install

# 3. Install Playwright browser binaries
npx playwright install chromium

# 4. Launch the local server
node server.js