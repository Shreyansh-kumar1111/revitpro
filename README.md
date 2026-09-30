# Courtyard Commons: A Climate-Responsive Mixed-Use Hub
### Smart India Hackathon 2026 · Problem ID: SIH26116 (Autodesk Design Challenge)
**Team Name:** BRAIN.exe_N8G6  
**Category:** Software / Autodesk Revit-Led Proposal  
**Live Development Server:** `http://localhost:5173/`

---

## 🏛️ Project Overview
**Courtyard Commons** is a climate-responsive, high-performance urban mixed-use prototype designed entirely according to the **SIH26116 Autodesk Challenge** requirements. The building synthesizes three complementary urban roles into a singular, human-scaled architectural mass:

1. **Subsurface Mobility & Infrastructure (Basement -1):**  
   64 car parking bays with 100% EV readiness (12 x 50kW DC Fast Chargers + 52 x 22kW AC Smart Chargers), a 180,000-liter underground stormwater retention cistern, and centralized MEP plant.
2. **Active Commercial Edge & Community Podium (Ground + Level 1):**  
   2,060 m² of street-activating retail, artisan bakery, pharmacy, community co-working lounge, and a 3.5m sheltered pedestrian colonnade with dual North-South breezeway portals to the court.
3. **High-Performance Residential Stack (Levels 2 to 9):**  
   72 cross-ventilated modular homes (24x 1BHK, 32x 2BHK, 16x 3BHK) with 1.8m cantilevered private balconies and 32° vertical terracotta louvers (brise-soleil).
4. **Breathable Courtyard Lung (Central Core):**  
   A 24m x 20m open-to-sky courtyard driving thermal buoyancy (stack effect ventilation at 6.2 ACH) and an 85 m² shallow stepped reflecting pool producing a **-3.8°C evaporative microclimate cooling reduction**.
5. **Clean Energy Crown (Rooftop Level):**  
   A 120 kWp bifacial monocrystalline solar PV canopy generating ~175,200 kWh/year (offsetting 100% common loads) and a 280 m² urban community farm.

---

## 🚀 Key Interactive Prototype Modules

### 1. 🏢 3D Digital Twin & BIM Viewer (Three.js WebGL Engine)
- **Coordinated 3D Modeling (LOD 350):** Realistic structural concrete columns, transfer slabs, glass curtain walls, balconies with planters, solar canopy, and parked EV vehicles.
- **Exploded Axonometric View:** Interactive vertical slider (0% to 100%) separating Substructure, Commercial Podium, Residential Living, and Rooftop Solar to reveal internal structural coordination.
- **Level Isolation Filter:** Dropdown to isolate individual levels (Basement -1, Ground Colonnade, Level 2 Structural Transfer Floor, Living Stack, Rooftop).
- **Autodesk Forma Solar & Shadow Ray-Tracing:** Interactive slider (06:00 to 18:00) with dynamic sun vector, real soft shadow projections across the courtyard, and live Solar Flux ($W/m^2$) readouts.
- **CFD Wind & Stack Ventilation Simulation:** Real-time particle stream showing prevailing southwest winds entering ground breezeways, cooling over the reflecting pool, and swirling up through the courtyard chimney stack.
- **False-Color Solar Heatmap:** Toggle overlaying surface radiation absorption across facades and courtyard.
- **Revit Element Inspector:** Click any 3D element to inspect its Revit Family, Material, Volume, U-Value, and Structural Capacity.
- **30-Second Cinematic Walkthrough Tour (Slide 4 requirement):** Automated camera flight across 5 key architectural milestones with scrub bar and live narration.

### 2. 📐 Level 2 Structural Detailing (Sheet S-201 · IS 456 / Eurocode 2)
- **Interactive 2D Blueprint Canvas:** Zoom & pan over the structural layout of Grids 1–5 and Grids A–D with central courtyard open void.
- **Parametric Cross-Section Inspector:**
  - **Transfer Beam TB-1 (350 x 750 mm, Concrete M35):** 4-T25 top rebar, 6-T28 bottom tension rebar in two layers, 4-legged T10 stirrups @ 100/160 c/c, $M_u = 620\text{ kNm}$, $V_u = 385\text{ kN}$.
  - **Transfer Column C-1 (600 x 600 mm, Concrete M40):** 12-T25 longitudinal bars (2.83% steel), 4-legged T10 rectangular and diamond links @ 120 c/c, $P_u = 4,850\text{ kN}$.
  - **Typical Beam B-2 (250 x 500 mm, M30)** & **Transfer Slab S-1 (200 mm RC)**.
- **Bar Bending Schedule (BBS):** Complete takeoff table with concrete grade, rebar sizes, moment capacity, and code compliance checks.

### 3. ☀️ Autodesk Forma Environmental Analytics
- **Microclimate Cooling:** Ambient $38.2^\circ C \to 34.4^\circ C$ ($-3.8^\circ C$ drop via water vaporization and vegetative transpiration).
- **Spatial Daylight Autonomy (sDA 300/50%):** $88.4\%$ occupied area meeting LEED v4 / GRIHA standards.
- **Façade Solar Radiation:** $32^\circ$ terracotta louvers reduce peak solar heat gain by $46.3\%$.
- **Natural Air Ventilation:** $6.2\text{ ACH}$ stack ventilation rate.
- **Interactive Sensitivity Tuner:** Sliders for water pool area ($m^2$), tree canopy ($10-80\%$), and louver angle ($0-60^\circ$) recalculating thermal comfort in real time.

### 4. 📑 Building Program & Revit Quantity Takeoff (BOM)
- Detailed breakdown of all 5 building zones matching Slide 2.
- Revit Quantity Takeoff schedule filtered by discipline (Structural, Rebar, Façade, Solar PV).
- Export Schedule to CSV button.

### 5. 🛡️ Review Gate & Compliance Auditor (Slide 5 MVP)
- Compliance auditor verifying:
  - 100% native Autodesk Revit authoring (no copied external files).
  - LOD 350 multi-discipline coordination.
  - Complete Level 2 structural detailing floor.
  - Autodesk Forma microclimate verification.
- One-click audit runner with animated progress bar, confetti celebration, and verified submission certificate.
- Downloadable official SIH Pitch Package (.MD).

### 6. 📽️ SIH Pitch Presentation Companion (Slides 1–6)
- Interactive slide deck mapping 1:1 with the team's presentation slides.
- Interactive "Jump to Live Interactive Prototype View" button on each slide.

---

## 🛠️ How to Run Locally

```bash
# 1. Install dependencies
npm install

# 2. Start Vite development server
npm run dev

# 3. Open in browser
http://localhost:5173/
```
