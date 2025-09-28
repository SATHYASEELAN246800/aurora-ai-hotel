# Aurora AI Hotel – Full Production-Level AI Agent Platform

[Workspace Link](https://app.base44.com/apps/68c58dd6938e5e877680c1ac/editor/preview/Dashboard) | [Published App](https://aurora-ai-hotel-7680c1ac.base44.app)

---

## Project Overview

**Aurora AI Hotel** is a production-ready AI simulation platform providing **29 distinct AI agents** for hotel management, automation, and customer engagement. The platform integrates **AI-powered simulations**, **admin monitoring**, **multi-login (social + email)**, **multi-language UI**, and a fully responsive food ordering system including age-verified alcohol.

This project showcases **AI-driven hotel management, immersive customer experiences, and real-world automation demos**.

---

## Key Features

### 1. AI Agent Simulation
- **29 AI agents** with unique live interactive demos:
  - Chatbots, flowcharts, decision sliders, timelines, Sankey diagrams, network graphs, predictive analytics, drone/robot simulations, immersive room holosuites, and more.
- Admin: full CRUD and system monitoring.
- Customer: view & interact with simulations.
- All routes fully functional, no 404s.
- Background/theme per agent tab.

### 2. Admin & Customer Modes
- Fixed admin password bug; supports full password with special chars.
- Admin: manage AI agents, logs, drone dispatch, global settings.
- Customer: browse menu, order food & drinks, parcel services.

### 3. Login / Signup
- Google OAuth (required) + optional Facebook/LinkedIn.
- Email/password fallback.
- Session management with secure HTTP-only cookies.
- Multi-language login page.

### 4. Food Ordering Simulation
- Responsive menu grid with images:
  - Breakfast/South Indian, North Indian, Chinese, Desserts, Beverages, Alcohol/Party Mode.
- Cart system: add/remove items, quantity, summary, checkout.
- Age verification for alcohol purchases.

### 5. Multi-Language Support
- Tamil, English, 20+ Indian languages.
- Live switching without page reload.
- All UI elements localized.

### 6. UI/UX & Responsiveness
- Mobile/tablet/desktop responsive design.
- Smooth hover effects, transitions, collapsible menus.
- Fully interactive sidebars, top bars, and agent dashboards.

### 7. Logging & Monitoring
- Agent activity logging
- Exportable CSV for admin.
- Drone/robot activity simulation.

---

## AI-Focused Tech Stack

### Frontend
- **Framework:** React.js + TypeScript (Vite/Next.js)
- **Styling:** Tailwind CSS, Framer Motion
- **Visualizations:** 
  - Mermaid.js (flowcharts), Cytoscape.js (network graphs)
  - D3.js, vis-timeline, vis-network
  - Chart.js / Recharts (analytics & predictive charts)
  - Konva / React-Sigma (2D/3D graph visualizations)
- **Animation:** Lottie, CSS transforms, Framer Motion
- **Voice & AI:** Web Speech API (STT/TTS), Chatbot UI, AI-guided decision sliders
- **Routing & State:** React Router, Zustand / Redux Toolkit
- **Internationalization:** react-i18next
- **Image Handling:** Web-optimized grids, object-fit: cover

### Backend
- **Framework:** Node.js + Express / FastAPI (Python)
- **Database:** Supabase (PostgreSQL + Auth + Realtime)
- **AI API Integration:** Groq API (server-side), simulated deterministic fallback
- **Authentication:** OAuth2 (Google), JWT, secure session cookies
- **Admin Controls:** Agent CRUD, logs, drone/robot dispatch, global overrides
- **Server-side AI Logic:** 
  - Recommendation engines
  - Predictive food waste & inventory
  - Dynamic pricing & occupancy prediction
  - Room automation control
  - Personalized cooking & nutrition AI
- **Logging:** Structured JSON `agent_logs` table

### AI & ML Libraries (optional / future enhancement)
- TensorFlow.js / PyTorch (for predictive simulations)
- Hugging Face Transformers (chatbot & language models)
- OpenCV.js (facial recognition & gesture detection)
- NLP Libraries: spaCy, NLTK (translation, recommendation)
- Reinforcement Learning Simulation (for agent optimization)

### DevOps & Deployment
- Base44 workspace
- Vercel / Cloud Run deployment
- Docker-compose for local dev
- Environment Variables: `SUPABASE_URL`, `SUPABASE_KEY`, `GROQ_API_KEY`, `JWT_SECRET`, `ADMIN_PASS_HASH`

### Accessibility
- ARIA attributes
- Keyboard navigation for all interactive elements
- Voice readouts / TTS for first-time user guidance

---

## Installation & Setup

1. Clone the repository:
```bash
git clone <your-repo-url>
cd aurora-ai-hotel
