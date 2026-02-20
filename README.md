# 🚛 OptiRoute SWM & CitizenSync

**Digitizing the "Swachh Bharat" Fleet: Dynamic Routing & The Digital Horn**
*Submission for the Symbiosis Skill Hackathon (SSH-2026) | Theme: Smart Cities & Urban Development*

---

## 🚦 The Urban Challenge
Indore operates an incredible 100% Door-to-Door (D2D) waste collection system. However, the current model faces two major friction points:
1. **The Municipal Bottleneck:** 600+ tippers run on rigid, fixed routes. This leads to massive fuel waste during traffic spikes and leaves trucks overflowing or stranded during unpredicted high-waste days.
2. **The Citizen Annoyance:** The morning waste collection relies on loud music to alert citizens, causing daily city-wide noise pollution. Citizens lack accurate ETAs, leading to missed pickups or waiting outside unnecessarily when a truck fills up and leaves early.

## 💡 The Solution
**OptiRoute & CitizenSync** is a bidirectional digital ecosystem that optimizes municipal fleet routes dynamically while giving citizens real-time tracking, eliminating the need for noise-based alerts.

### 🚀 Key Features
* **The "Digital Horn":** Replaces the physical loudspeaker with automated push notifications and live geofenced ETAs via a lightweight PWA.
* **Predictive Load Balancing:** Citizens can flag "Excess Waste Today" in the app. The system generates a live heatmap, routing high-capacity compactors to surge areas *before* regular tippers overflow.
* **Dynamic Fleet Reallocation:** AI-driven micro-routing (utilizing Dijkstra’s & Minimum Spanning Trees) that adjusts truck paths in real-time based on traffic and live load capacities.
* **Radical Transparency:** If a truck hits 100% capacity and reroutes to the transfer station, citizens instantly get an updated ETA for the standby vehicle.

## 🛠️ Tech Stack
* **Frontend (Citizen App & Driver View):** Nuxt 3, Tailwind CSS (Progressive Web App)
* **Backend & Real-Time Sync:** Supabase (PostgreSQL, Auth, WebSockets for live tracking)
* **Core Routing Engine:** Python, FastAPI (Graph algorithms for nodal path calculation)

## ⚙️ Running the Prototype Locally

### Frontend (Nuxt 3)
\`\`\`bash
# Install dependencies
npm install

# Run the development server
npm run dev
\`\`\`

### Backend (Python/FastAPI Engine)
\`\`\`bash
# Create a virtual environment
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

# Install dependencies
pip install fastapi uvicorn

# Run the API server
uvicorn app:app --reload
\`\`\`

## 👥 Team
* **Aditya** - Team Leader / Full Stack Developer
* *(Add other team members here if applicable)*

---
*Built with ❤️ for Indore's Smart City infrastructure.*
