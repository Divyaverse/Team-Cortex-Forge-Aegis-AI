# 🛡️ Aegis.AI — Neuro-Behavioral Anti-Bot Defense

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-v4.8.2--Stable-success)
![Next.js](https://img.shields.io/badge/Next.js-14-black?logo=next.js)
![React](https://img.shields.io/badge/React-18-blue?logo=react)
![Three.js](https://img.shields.io/badge/Three.js-3D_Engine-white?logo=three.js)
![Tailwind](https://img.shields.io/badge/Tailwind_CSS-Enterprise-38B2AC?logo=tailwind-css)

> **Eradicate Bots. By Behavior.** <br />
> An enterprise-grade Cybersecurity Command Center built to detect automated attacks on FinTech platforms using behavioral AI, Spatio-Temporal Analysis, and Isolation Forest anomaly detection.

Developed by **Team Leviosa** for **HackUp 2026** (Navi Mumbai's Largest Hackathon by Hack The Core).

---

## 🛑 The Problem
Traditional anti-bot systems rely on static IP blocking and rate-limiting. Modern hackers bypass this using rotating proxies, distributed botnets, and IP spoofing to launch Credential Stuffing, API Abuse, and Low & Slow attacks. 

## 💡 The Aegis.AI Solution
Aegis.AI shifts the paradigm from **Identity-based detection** (IPs) to **Behavior-based detection**. By analyzing the exact spatio-temporal rhythms of user interactions—such as the time gaps between requests ($\Delta t$), interaction velocity, and behavioral entropy—our machine learning model can distinguish a human from a bot script with **99.8% accuracy in under 42ms**.

---

## ✨ Enterprise Features

### 📡 1. Command Overview Dashboard
- **Behavioral Intelligence Graph:** Real-time HTML5 Canvas network visualization mapping IPs to Internal Users, highlighting anomalous bot clusters in real-time.
- **Risk Level Telemetry:** Dynamic doughnut charts computing the global threat index.
- **Network Activity:** Recharts-powered area charts tracking normal vs. suspicious vs. attack packets per second (PPS).
- **Live Intercept Feed:** Real-time logging of blocked malicious requests and auto-deflection events.

### 🧠 2. ML Tuner (Isolation Forest Configuration)
- **Rhythm Telemetry Analysis:** Interactive 3D scatter plots comparing Human vs. Bot request intervals.
- **Dynamic Thresholding:** Adjust the sensitivity of outlier detection nodes with live metrics on False Positives and Inference Latency.

### 🌍 3. Global Threat Radar
- **Live Geolocation Tracking:** A custom-built CSS/React radar sweeping for active IP vectors across global regions.
- **Auto-Deflection Scoring:** Metrics on deep-inspection scrubbing and threat routing.

### 🔬 4. Threat Simulation Engine
- **Target Application:** Embedded mock FinTech Auth/Payment APIs.
- **Split-Testing:** Send manual (human) requests alongside automated botnet payload deployments to test the ML parameters live.

### 📖 5. Developer Integration Portal
- **API Config:** Sandbox/Production key management and webhook routing interfaces.
- **Integration Docs:** Clean, Stripe-inspired documentation for embedding the Aegis SDK.

---

## 🏗️ System Architecture

Aegis.AI operates on a robust, asynchronous data pipeline:

1. **Log Ingestion Engine:** Captures telemetry (IP, Timestamp, Action, User ID).
2. **Feature Extraction Layer:** Converts raw logs into behavioral signals ($\Delta t$ variance, Request Velocity, IP Rotation Entropy).
3. **ML Microservice (The Brain):** Scikit-Learn **Isolation Forest** evaluates the feature vector against the human baseline.
4. **Risk Scoring Engine:** Assigns Threat Levels (`Safe`, `Suspicious`, `Critical`).
5. **SOC Dashboard (This Repository):** Next.js frontend fetches live telemetry and renders tactical data.

---

## 💻 Tech Stack (Frontend Repository)

- **Framework:** [Next.js 14](https://nextjs.org/) (App Router)
- **Language:** TypeScript
- **Styling:** Tailwind CSS (Custom Enterprise Zinc/Slate Palette)
- **3D & Graphics:** Three.js, `@react-three/fiber`, `@react-three/drei`, HTML5 Canvas API
- **Data Visualization:** Recharts
- **Icons:** Lucide React
- **Fonts:** Inter (Sans), JetBrains Mono (Data/Code), Syne (Display)

---

## 🚀 Getting Started

### Prerequisites
Ensure you have Node.js (v18.x or later) installed.

### Installation
1. Clone the repository:
   ```bash
   git clone [https://github.com/your-username/aegis-ai.git](https://github.com/your-username/aegis-ai.git)
   cd aegis-ai

Install dependencies:(Note: Using specific Three.js versions for React 18 compatibility)Bashnpm install
# If 3D dependencies are missing:
npm install three @react-three/fiber@8 @react-three/drei@9
Run the development server:Bashnpm run dev
Open your browser and navigate to:http://localhost:3000 — Marketing / 3D Landing Pagehttp://localhost:3000/dashboard — Aegis Command Centerhttp://localhost:3000/integration — Developer Docshttp://localhost:3000/demo — Target FinTech App🤫 Presentation ShortcutWhile presenting the dashboard, press Ctrl + Shift + A to seamlessly trigger the global botnet simulation hook without clicking any buttons.📁 Directory StructurePlaintextaegis-ai/
├── app/
│   ├── dashboard/page.tsx     # SOC Command Center route
│   ├── demo/page.tsx          # Target Application route
│   ├── integration/page.tsx   # Developer API Docs route
│   ├── globals.css            # Enterprise CSS & Animations
│   ├── layout.tsx             # Root layout
│   └── page.tsx               # 3D Landing Page
├── components/
│   ├── charts/                # Recharts implementations
│   ├── dashboard/             # All sidebar tabs (Overview, ML, Logs, Sims)
│   ├── network/               # Threat Map & Canvas Network Graph
│   └── ui/                    # Badges, ScoreBars, Pills
├── hooks/
│   ├── useSimulation.ts       # Global state for demo telemetry
│   └── useClock.ts
├── lib/
│   ├── simulation.ts          # Math logic for attack simulation
│   └── utils.ts               # Tailwind mergers & mock data generators
└── types/
    └── index.ts               # TypeScript interfaces

## Team
🏆 Team Leviosa Built with ❤️ 
| Name           | Role       | College                                |
|----------------|------------|----------------------------------------|
| Harman Saini   | ML         | Chhatrapati Shivaji Maharaj University |
| Divya Tiwari   | Backend    | SIES Graduate School of Technology     |
| Shrishti Singh | Frontend   | Chhatrapati Shivaji Maharaj University |
| Swapnil Harad  | Presenter  | Datta Meghe College of Engineering     |
