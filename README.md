# Macroly Fit (MacroTracker) 🤖

### **The AI-Agentic Nutrition Logistics Engine**
*An execution-first system powered by n8n orchestration, OpenAI intelligence, and Claude-driven interfaces.*

---

## 🚀 The Agentic Vision
Macroly Fit isn't a traditional app; it's a **coordinated swarm of AI agents**. By leveraging **n8n** as the orchestrator, we bypass traditional backend constraints to build a "Logistics Engine" that handles the friction of meal planning and grocery purchasing automatically.

---

## 🛠 The "Agentic" Stack

| Role | Technology | Responsibility |
| :--- | :--- | :--- |
| **Orchestrator** | **n8n** | The "Brain." Connects APIs, manages state, and triggers workflows. |
| **Logic Engine** | **OpenAI 5.2 (o-series)** | Complex reasoning: Goal-to-Macro conversion and Accuracy validation. |
| **UI / UX** | **Claude 3.5 Sonnet** | Generates the frontend code dynamically and handles complex human-like check-ins. |
| **Database** | **Supabase / Airtable** | Persistent storage for user logs, weight trends, and verified food items. |
| **Integrations** | **n8n Nodes** | Direct connections to Instacart API, Google Vision (for logging), and WhatsApp/Telegram. |

---

## 📂 System Architecture

```text
macroly-fit-agent/
├── n8n-workflows/          # JSON exports of the "Neural" logic
│   ├── wf_goal_planning.json
│   ├── wf_grocery_sync.json
│   └── wf_ai_logging_v5.json
├── frontend-claude/        # Claude-generated React/Tailwind views
│   ├── Dashboard.jsx
│   └── GroceryCart.jsx
├── prompts/                # System prompts for OpenAI & Claude
│   ├── nutrition_specialist.md
│   └── code_architect.md
└── docker-compose.yml      # Self-hosting setup for n8n/Postgres
