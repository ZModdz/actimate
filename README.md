# ActiMate — UMS Campus Activity-Matching & Last-Minute Replacement Platform

> **"Find Your People. Do More Together."**  
> An interactive mobile app prototype built specifically for Universiti Malaysia Sabah (UMS) students, designed for pitch presentations, lecturer evaluation, and user validation.

---

## 📌 Project Overview

ActiMate solves a universal university problem: **last-minute dropouts that ruin sports matches, group study sessions, and campus hangouts.**

When a student cancels right before a futsal match, badminton session, or study crunch, ActiMate allows organisers to broadcast an **Urgent Replacement Request** to nearby peers in seconds. Combined with **"Find Your Vibe" (mood-based recommendations)** and an **objective attendance-based Reliability Score**, ActiMate creates a dependable, safe, and vibrant campus lifestyle ecosystem.

---

## 🚀 How to Run the Prototype

No compilation or external database setup is needed to preview or evaluate the prototype.

### Method 1: Instant Browser Preview (Recommended)
Simply open `index.html` in any web browser (Google Chrome, Apple Safari, Microsoft Edge, or Mozilla Firefox):
```bash
# On macOS
open /Users/moddz./.gemini/antigravity/scratch/actimate/index.html

# Or simply double-click index.html in Finder
```

### Method 2: Local HTTP Server
If you prefer running via a local development server:
```bash
cd /Users/moddz./.gemini/antigravity/scratch/actimate

# Using npx (Node.js)
npx serve .

# Or using Python
python3 -m http.server 3000
```
Then visit `http://localhost:3000` in your browser.

### Method 3: React + TypeScript Source Code
The repository also contains the canonical modular React 18 + TypeScript architecture:
```bash
npm install
npm run dev
```

---

## 📱 Implemented Screens & Interactive User Flows

| Screen | Key Features & Realistic Interactions |
| :--- | :--- |
| **A. Welcome & Onboarding** | Brand presentation, value props, UMS student single-sign-on verification modal (`@student.ums.edu.my`), and a **1-click Lecturer Demo Entry Mode**. |
| **B. Home Dashboard** | Greeting with user's reliability badge (`Farhan Azman`, 94/100), campus location selector (UMS Sports Complex, Dewan Canselor, Library), prominent **"How are you feeling today?"** mood check-in card, category chips, **"Needs 1 More Player"** urgent carousel, and happening near you. |
| **C. Explore Activities** | Live instant search, category filtering (Futsal, Badminton, Basketball, Run/Gym, Study, Chill), urgent slot toggle, sorting (Recommended, Soonest, Most slots), budget selector, and empty state handler. |
| **D. Activity Details** | Rich sports photography, host reliability rating, UMS venue tips, participant progress bar with avatars, transparent fee vs commitment deposit breakdown, cancellation policy, **Join confirmation modal**, save toggle, and report sheet. |
| **E. Last-Minute Replacement Hub** | **Differentiating feature**: Displays countdown urgency, dropout reason, and applicant queue (`Looking` → `Applicants Available` → `Confirmed`). Includes a **"Simulate Incoming Applicant"** button so evaluators can test instant approvals. |
| **F. Create Activity** | 2-step organiser form with live real-time card preview as you type, UMS venue picker, deposit rules, and instant insertion into Home & Explore feeds via local state. |
| **G. "Find Your Vibe" (Mood Recommendations)** | Step 1 (Energy check: Energetic, Happy, Calm, Tired, Stressed) → Step 2 (Interaction style: Active group, small casual, quiet, study) → Step 3 (Curated suggestions with friendly, non-clinical explanations). Guaranteed private. |
| **H. Inbox & Alerts** | Multi-channel chat with interactive message sending & automated host replies, plus a campus notification centre with clickable alert links. |
| **I. Profile & Reliability** | Verified student credentials, attendance history (18 attended, 94% rate), interests editor, and a deep-dive **Reliability Score Breakdown Modal** (+3 for punctuality, -5 for ghosting). |
| **J. Subscriptions & Upgrades** | Clear comparison between Free Student Plan (RM0), ActiMate Plus (RM4.90/mo), and Organiser Pro (RM9.90/mo). Interactive mock checkout (FPX / TNG) and active plan switcher. |
| **K. Settings & Safety** | UMS matric verification status, privacy toggles (private vibe check-ins), UMS community guidelines, and data reset tool. |

---

## 🎨 Design Direction

- **Primary Colors:** Deep Indigo (`#4F46E5`, `#3730A3`) & Fresh Mint Green (`#10B981`, `#059669`).
- **Surface:** Soft off-white with crisp border contours and rounded corners (`rounded-3xl`).
- **Typography:** Plus Jakarta Sans for clean readability.
- **Evaluator Switch:** Use the **"Mobile Frame" / "Wide View"** button on the presentation bar to toggle between an iPhone 15 Pro frame mockup and a full responsive layout.
