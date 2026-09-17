# 🌱 Carbon Dioxide Removal (CDR) — Episode Research Notes

> **Episode Theme:** Carbon Debt, Removal Technologies & the Open-Source CDR Verification Stack  
> **Last Updated:** June 2026  
> **Research Method:** GitHub repository search + commit history analysis

---

## 🎙️ Episode Angle Ideas

### Story 1: "The Carbon Detectives"
**Focus repo:** [`carbonplan/cdr-database`](https://github.com/carbonplan/cdr-database)  
**Stars:** 29 | **Language:** Jupyter (Python) | **Last commit:** February 2025

An open-source database and analytical toolkit for evaluating carbon dioxide removal projects. Developed by CarbonPlan (a nonprofit research lab), it provides transparent, data-driven assessments of CDR project claims — critical in a market plagued by double-counting and over-crediting.

**Commit trend:** Activity peaked in early 2025 with infrastructure cleanup — migrating from Google Analytics to Plausible. The project is in **maintenance mode** — the scientific backbone is built, focus shifted to data quality.

**Episode hook:** When a offsets company claims "we removed 10,000 tons of CO₂," how do you verify that? CarbonPlan built an open-source answer.

### Story 2: "The Forest Carbon Risk Models"
**Focus repo:** [`carbonplan/forest-risks`](https://github.com/carbonplan/forest-risks)  
**Stars:** 35 | **Language:** Python | **Last commit:** January 2024

Statistical models that assess risks to forest-based carbon projects — fire, disease, climate-induced mortality. Forest carbon is the largest CDR pathway, but forests can burn, and the carbon they stored returns to the atmosphere.

**Commit trend:** Active development 2022–2023, final commits Jan 2024 (pyproject.toml config updates). **Effectively frozen** — the science is done, the data is published.

**Episode hook:** The biggest carbon removal method on Earth is trees — but what happens when the trees burn? Open-source models quantify the risk that carbon offsets might vanish in a wildfire.

### Story 3: "Modeling Rock Weathering for Carbon"
**Focus repo:** [`cdr-laboratory/SCEPTER`](https://github.com/cdr-laboratory/SCEPTER)  
**Stars:** 8 | **Language:** Fortran | **Last commit:** July 2026

A reaction-transport code for simulating carbon dioxide removal through **enhanced rock weathering** — spreading crushed silicate rocks on farmland to accelerate natural weathering processes that absorb CO₂. **Most recently active CDR-specific simulation tool** in our dataset.

**Episode hook:** Speeding up geology — how computed rock weathering could be the carbon removal method that actually scales.

### Story 4: "The CDR Lab Where Experiments Live"
**Focus repo:** [`hsbay/cdrmex`](https://github.com/hsbay/cdrmex)  
**Stars:** 13 | **Language:** Python (Jupyter) | **Last commit:** May 2025

**CDR Modeling Experiments** — a Jupyter-based toolkit for running and comparing different carbon dioxide removal scenarios. Maintained by Shannon Fiume.

**Commit trend:** Active 2022–2023 with code development, mathpix tools, dependabot updates (numpy 1.19→1.22). README update May 2025. Steady maintenance.

---

## 📈 Commit Trend Analysis — Carbon Capture Projects

| Repository | Stars | Last Code Commit | Activity Pattern | Trend |
|---|---|---|---|---|
| forest-risks | 35 | Jan 2024 | 2022–2023 burst, then freeze | 🟰 Research complete |
| cdr-database | 29 | Feb 2025 | Active through early 2025, transition phase | 📉 Migrating, not adding features |
| cdrmex | 13 | May 2025 | Steady maintenance since 2022 | 📉 Maintenance mode |
| SCEPTER | 8 | Jul 2026 | Active development | 🟢 Growing |
| clisops (roocs) | 25 | Sep 2026 | Climate sim operations | 🟢 Active |
| C-Star (Worthy-ocean) | 21 | Sep 2026 | Marine CDR focus | 🟢 Active |

### Key Trend: CDR is shifting from "build models" to "verify claims"

- **Phase 1 (2020–2023):** The open-source CDR community focused on building models and datasets. CarbonPlan's forest-risks and cdr-database, CDRMEX, and SCEPTER were all created during this burst.
- **Phase 2 (2024–2026):** The science is largely built. The frontier has moved to **verification and governance** — can we trust carbon credit claims? CarbonPlan's migration projects (GA→Plausible) suggest a pivot toward transparency infrastructure.
- **Blue Ocean:** Enhanced weathering (SCEPTER) and marine CDR (C-Star) are the least-developed but potentially highest-impact pathways.

### 🎙️ Podcast Soundbite

> *"We spent a decade building models that say we CAN remove carbon. Now we need to build systems that prove we DID — and that's where the really hard problems begin."*

---

## 🔑 Key Terminology

- **CDR (Carbon Dioxide Removal):** Techniques that remove CO₂ from the atmosphere — nature-based and engineered
- **DAC (Direct Air Capture):** Chemical processes that strip CO₂ directly from ambient air (Climeworks, Carbon Engineering)
- **Enhanced Weathering:** Accelerating natural rock weathering by spreading crushed silicates on land/ocean
- **Bioenergy with CCS (BECCS):** Growing biomass for energy, capturing and storing the CO₂
- **Carbon Credit Verification:** Independently confirming that a CDR project delivered the claimed removal
- **Buffer Pool:** A reserve of carbon credits held back to cover project failures (e.g., forest fires)
