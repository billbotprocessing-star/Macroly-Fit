# Macroly Fit (MacroTracker) 🎯

### **The Execution-First Nutrition System**
*Turning fitness goals into daily decisions through automated planning, purchasing, and verified accuracy.*

---

## 🚀 The Vision
Most nutrition apps fail because they are **tracking-first**, requiring high willpower and exhaustive manual data entry. **Macroly Fit** is **execution-first**. 

Instead of asking *"What did you eat?"*, we answer *"What should you buy and eat right now?"* by bridging the gap between a macro goal and a digital grocery cart. It is built for the busy professional (25–45) who wants body recomposition results without the administrative overhead of traditional calorie counting.

---

## 🛠 Core Pillars & Features

### 🛒 Plan-to-Purchase Workflow
* **Auto-Planning:** Converts goals (Fat Loss, Recomposition, Endurance) into weekly meal plans with macro/micro guardrails.
* **Cart Automation:** Automatically builds grocery lists and populates retailer carts (Instacart, Walmart, etc.) based on your plan.
* **Smart Substitutions:** AI-driven swaps based on dietary preferences, allergies, and real-time budget constraints.

### 🎯 The Accuracy Layer
* **Confidence Scoring:** Every log includes a confidence score. If the AI is uncertain about a portion size, it prompts the user for clarification—preventing "garbage-in, garbage-out" data.
* **Verified Database:** Curated nutrition data for the top 5,000 most-purchased grocery items and major restaurant chains.

### 📈 Progress Ops (Dynamic Adjustment)
* **Closed-Loop Feedback:** Weekly check-ins adjust targets based on *actual* weight trends, training load, and adherence, rather than relying on static BMR equations.
* **Hybrid Logging:** Frictionless entry via **Photo**, **Voice**, or **Manual** logging with AI-assisted portion estimation.

---

## 📂 Repository Structure

This project follows a **Feature-Based Architecture** to support scalability and domain isolation.

```text
macroly-fit/
├── src/
│   ├── components/         # Atomic UI (Button, Input, Card)
│   ├── features/           # Domain-specific logic
│   │   ├── dashboard/      # Daily meal plans & logging UI
│   │   ├── grocery/        # Cart automation & Retailer APIs
│   │   └── progress/       # Weight trends & check-in logic
│   ├── hooks/              # Global hooks (useMacros, useAuth)
│   ├── services/           # External API wrappers (AI, Instacart)
│   ├── store/              # State management (Zustand/Context)
│   └── utils/              # Macro formulas & accuracy logic
├── tailwind.config.js      # Design system configuration
└── vite.config.js          # Build tool configuration
