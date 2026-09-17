# 🌊 Ocean-Based Climate Intervention — Episode Research Notes

> **Episode Theme:** Marine CDR, Ocean Circulation Models & Ocean Alkalinity Enhancement  
> **Last Updated:** June 2026  
> **Research Method:** GitHub repository search + commit history analysis

---

## 🎙️ Episode Angle Ideas

### Story 1: "The $1.6 Billion Open-Source Ocean"
**Focus repo:** [`CliMA/Oceananigans.jl`](https://github.com/CliMA/Oceananigans.jl)  
**Stars:** 1,333 | **Language:** Julia | **Last commits:** Daily (Sep 2026)

The **most actively developed open-source ocean simulation tool in the world**. Built by the Climate Modelling Alliance (CliMA) — a collaboration between Caltech, MIT, and NASA JPL. A GPU-accelerated, modular Julia package for ocean climate modeling.

**Recent commit trend (Sep 2026):** Near-daily commits on:
- **TripolarGrid** — enabling true global ocean simulations (was limited to regional)
- **Zarr I/O** — cloud-native data storage for simulation outputs
- **Tracer boundary conditions** — directly relevant to ocean intervention modeling (alkalinity additions)
- **Closure field restoration** from checkpoints (turbulence modeling improvements)

**Episode hook:** Why did Caltech, MIT, and NASA build a Julia ocean model? Because the old Fortran monoliths couldn't keep up — and this one gets daily commits from a global community.

### Story 2: "The Atmosphere Beside the Ocean"
**Focus repo:** [`CliMA/ClimaAtmos.jl`](https://github.com/CliMA/ClimaAtmos.jl)  
**Stars:** 119 | **Language:** Julia | **Last commits:** Daily (Sep 2026)

The companion atmospheric model to Oceananigans — a modular Julia package for climate modeling with cloud microphysics, albedo calculations, and atmosphere-ocean coupling.

**Recent commit trend (Sep 15–16, 2026):** Floor of daily commits, major refactoring — replacing deprecated ClimaCore with modular AtmosModel architecture. Key work: moving grid/param/setup fields into a single AtmosModel struct.

**Episode hook:** The CliMA ecosystem isn't just one model — it's three models (Ocean, Atmosphere, Land) that plug together like LEGO. Why does modularity matter for climate science?

### Story 3: "Marine Carbon Dioxide Removal — The Ocean's Secret Weapon"
**Focus repo:** [`Worthy-ocean/C-Star`](https://github.com/Worthy-ocean/C-Star)  
**Stars:** 21 | **Language:** Python | **Last update:** September 2026

A Python package for setting up and running ocean model simulations with a particular focus on **marine carbon dioxide removal (mCDR)** applications — ocean alkalinity enhancement, artificial upwelling, and iron fertilization modeling.

**Episode hook:** The ocean absorbs 30% of our CO₂. Can we make it absorb more? C-Star is the open-source toolkit for answering that question with real ocean models.

### Story 4: "From Monolith to Modules"
**Focus repo:** [`CliMA/ClimateMachine.jl`](https://github.com/CliMA/ClimateMachine.jl)  
**Stars:** 470 | **Language:** Julia | **Status:** Deprecated

The original CliMA Earth System Model. Now carries a deprecation notice; functionality split into the modular ClimaAtmos.jl, Oceananigans.jl, and ClimaLand.jl. Last real commits in 2021.

**Episode hook:** The deprecation story illustrates how the field is maturing — from monolithic Fortran codes to modular, community-driven Julia packages.

---

## 📈 Commit Trend Analysis — Ocean Intervention Projects

| Repository | Stars | Last Commit | Activity Pattern | Trend |
|---|---|---|---|---|
| Oceananigans.jl | 1,333 | Sep 17, 2026 | **Extremely active** — daily commits | 🟢 Dominant force |
| ClimaAtmos.jl | 119 | Sep 16, 2026 | **Extremely active** — daily commits | 🟢 Dominant force |
| ClimaLand.jl | 71 | — | Active but less than ocean/atmosphere | 🟡 Growing |
| C-Star | 21 | Sep 2026 | Steady, focused scope | 🟡 Niche but active |
| SCEPTER | 8 | Jul 2026 | Focused development | 🟡 Growing |
| NOAA-GFDL/SM2 | — | 2019 | Legacy, minimal updates | 🟰 Maintenance only |

### Key Trend: The Julia Ocean Revolution

- **From monolithic to modular:** Old approach = one giant Fortran codebase. CliMA's Julia approach = focused packages that can be independently developed, tested, and extended.
- **From CPU-bound to GPU-accelerated:** Oceananigans leverages Julia's native GPU support, making global ocean simulations feasible on single workstations.
- **From Fortran to Julia:** Julia offers Fortran's performance with Python's productivity — crucial for attracting a younger, broader contributor community.

### Key Trend: Ocean intervention is the least-developed frontier

- SRM has AI detection tools (actm-sai-csu) and economic models (ClimateMARGO).
- CDR has verification databases (carbonplan/cdr-database) and risk models (forest-risks).
- **Ocean intervention has models (C-Star, Oceananigans) but almost no governance, verification, or policy work.** This is the Wild West of climate tech.

### 🎙️ Podcast Soundbite

> *"We can model the atmosphere in our laptops now. The ocean? We just figured out how to simulate it in Julia. But we still don't have the first conversation about who decides to change the ocean's chemistry."*

---

## 🔑 Key Terminology

- **mCDR (Marine Carbon Dioxide Removal):** Ocean-based methods for removing CO₂ — alkalinity enhancement, artificial upwelling, ocean fertilization
- **Ocean Alkalinity Enhancement (OAE):** Adding alkaline minerals (e.g., olivine, limestone) to seawater to boost its CO₂ absorption capacity
- **Artificial Upwelling:** Pumping nutrient-rich deep water to the surface to stimulate phytoplankton growth and carbon uptake
- **Ocean Fertilization (Iron):** Adding iron to iron-limited ocean regions to trigger phytoplankton blooms that absorb CO₂
- **Marine Cloud Brightening (MCB):** Spraying sea salt aerosols into marine clouds to increase their reflectivity
- **Tripolar Grid:** A spherical grid system that avoids pole singularities in ocean models — important for global simulations
- **Zarr:** Cloud-native data format for large scientific datasets — enables sharing and versioning of simulation outputs
