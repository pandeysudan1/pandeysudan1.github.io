# Sudhan Pandey — Research & Engineering Repositories

This repository is the index for my GitHub work. The projects are grouped by purpose so that packages, benchmarks, studies, and applications are easier to navigate.

## 1. Hydropower modelling, dynamics and control

### Core modelling packages
- [OpenHPLjl](https://github.com/pandeysudan1/OpenHPLjl) — nonlinear component-based hydropower modelling in Julia/ModelingToolkit; reservoir → waterways → turbine → shaft → generator → grid.
- [VannKraft.jl](https://github.com/pandeysudan1/VannKraft.jl) — acausal hydropower component library built around ModelingToolkit connectors and DAEs.
- [HydroPowerDynamics.jl](https://github.com/pandeysudan1/HydroPowerDynamics.jl) — compact dynamic and control-oriented hydro models for frequency response, FCR, governor and AGC studies.
- [HydroSyncBridge.jl](https://github.com/pandeysudan1/HydroSyncBridge.jl) — bridge between hydropower plant dynamics and synchronous-machine/grid dynamics.
- [HYDROSIM-PY](https://github.com/pandeysudan1/HYDROSIM-PY) — lightweight Python hydropower simulation work.

### Reference / legacy
- [OpenHPL](https://github.com/pandeysudan1/OpenHPL) — original OpenHPL codebase and physical-model reference.

### Benchmarks
- [HydroGovBenchmark.jl](https://github.com/pandeysudan1/HydroGovBenchmark.jl) — hydropower governor benchmark models and comparisons.
- [HydroPSSBenchmark.jl](https://github.com/pandeysudan1/HydroPSSBenchmark.jl) — hydro-generator and PSS benchmark studies.
- [HydroFlex-Screening](https://github.com/pandeysudan1/HydroFlex-Screening) — screening studies for hydropower flexibility.

### Notes
- [hydropower-control-notes](https://github.com/pandeysudan1/hydropower-control-notes) — hydropower control-system notes and worked studies.

## 2. Power-system dynamics and interconnected grids

- [PowerSystemODELibrary.jl](https://github.com/pandeysudan1/PowerSystemODELibrary.jl) — canonical ODE models for power-system dynamics.
- [InterconnectedAreas.jl](https://github.com/pandeysudan1/InterconnectedAreas.jl) — multi-area frequency control, tie-line power and AGC/LFC studies.
- [PowerSystemMultiphysics.jl](https://github.com/pandeysudan1/PowerSystemMultiphysics.jl) — multiphysics power-system modelling framework.
- [Nordic44-2026](https://github.com/pandeysudan1/Nordic44-2026) — modernization and dynamic studies of the Nordic-44 benchmark toward a 2026-oriented system model.
- [DyadSync.jl](https://github.com/pandeysudan1/DyadSync.jl) — synchronization-oriented dynamic modelling experiments.

## 3. Frequency control, FCR and AGC research

The main frequency-control studies are intentionally kept close to the modelling packages rather than split into many standalone repositories.

- **HydroPowerDynamics.jl** — compact FCR/FREKI/prequalification studies.
- **OpenHPLjl** — nonlinear FCR, turbine-governor-generator-grid and AGC studies.
- **InterconnectedAreas.jl** — tie-line control and multi-area AGC.
- **Nordic44-2026** — system-level disturbance propagation and coordinated frequency response.

Research path:

```text
Hydraulic physics
      |
   OpenHPLjl
      |
Turbine / governor / shaft / generator
      |
HydroPowerDynamics.jl ---- HydroSyncBridge.jl
      |                         |
     FCR / AGC          Power-system dynamics
                                |
                     InterconnectedAreas.jl
                                |
                         Nordic44-2026
```

## 4. Electricity markets and optimization

- [FairReactiveMarkets.jl](https://github.com/pandeysudan1/FairReactiveMarkets.jl) — reactive-power pricing, procurement, OPF and fair compensation studies.
- [FBMC.jl](https://github.com/pandeysudan1/FBMC.jl) — Flow-Based Market Coupling and transmission-constrained electricity-market studies.

## 5. Modelling infrastructure and research notes

- [MTK-notes](https://github.com/pandeysudan1/MTK-notes) — ModelingToolkit experiments: symbolic systems, DAEs, initialization, structural simplification, connectors and nonlinear-model workflows.
- [Papers](https://github.com/pandeysudan1/Papers) — private manuscript/research-paper workspace.
- [builder_mind_os](https://github.com/pandeysudan1/builder_mind_os) — private personal research/build workflow system.

## 6. Nepal resilience and disaster-response engineering

- [nepal-flood-warning](https://github.com/pandeysudan1/nepal-flood-warning) — camera/sensor/satellite-assisted flash-flood warning, downstream ETA and public alert concepts.
- [nepal-drone-response-team](https://github.com/pandeysudan1/nepal-drone-response-team) — drone-assisted disaster mapping and rapid-response engineering.
- [-nepal-drone-response-team](https://github.com/pandeysudan1/-nepal-drone-response-team) — earlier/duplicate drone-response repository; candidate for archival after content review.

## 7. Business and SME systems

- [VippaStallOps](https://github.com/pandeysudan1/VippaStallOps) — private food-stall operating tools and procedures.
- [himalayan-dumplings](https://github.com/pandeysudan1/himalayan-dumplings) — private Himalayan Dumplings business and digital operations repository.
- [sasto-salad](https://github.com/pandeysudan1/sasto-salad) — private food/SME concept and software work.
- [BenchmarkLabs-LinkedinApp](https://github.com/pandeysudan1/BenchmarkLabs-LinkedinApp) — private outreach/content-management application.

## 8. Portfolio / website

- [pandeysudan1.github.io](https://github.com/pandeysudan1/pandeysudan1.github.io) — this repository; portfolio and navigation layer for the projects above.

## Suggested repository hierarchy

```text
Research
├── Hydropower core
│   ├── OpenHPLjl
│   ├── VannKraft.jl
│   ├── HydroPowerDynamics.jl
│   └── HydroSyncBridge.jl
├── Benchmarks
│   ├── HydroGovBenchmark.jl
│   ├── HydroPSSBenchmark.jl
│   └── HydroFlex-Screening
├── Power systems
│   ├── PowerSystemODELibrary.jl
│   ├── InterconnectedAreas.jl
│   ├── PowerSystemMultiphysics.jl
│   └── Nordic44-2026
├── Markets
│   ├── FairReactiveMarkets.jl
│   └── FBMC.jl
└── Research support
    ├── MTK-notes
    ├── hydropower-control-notes
    └── Papers

Applications
├── nepal-flood-warning
├── nepal-drone-response-team
├── VippaStallOps
├── himalayan-dumplings
├── sasto-salad
└── BenchmarkLabs-LinkedinApp
```

## Main research storyline

**Nonlinear hydropower physics → plant control → synchronous-machine interaction → FCR/AGC → interconnected-area dynamics → Nordic system studies → market and flexibility value.**
