# ferro-pcm-viz

**Interactive architecture simulation for the Diamond-Integrated 
FERRO-PCM Non-Volatile Photonic Weight Memory.**

*Research design and scientific direction: Nils Haaland 
(nhaaland@yahoo.com) — Solbakken Research Initiative (Independent)*
*Simulation built with Claude (Anthropic)*
*Licence: Apache 2.0*

## Live simulation

**[Open interactive simulation](https://bluebflatminor.github.io/ferro-pcm-viz)**

## What it shows

An interactive cross-section of the full device stack — write bus, 
TiN electrode, Al:HfO₂ ferroelectric gate, Al₂O₃ seed, epitaxial 
graphene monolayer, SCD(111) diamond substrate, SiO₂ bonding oxide, 
and SiN waveguide — with real-time physics readouts including Fermi 
level, carrier density, extinction ratio, and quantum-capacitance-
corrected gate voltage.

Key interactions:
- Write +Pr / −Pr — flip ferroelectric polarisation, watch graphene 
  switch between Pauli-blocked (transparent) and absorbing states
- Send light pulse — observe optical read with zero static power
- 16×16 array — toggle individual cells, track cumulative write 
  energy vs DRAM equivalent in real time

## Physics parameters displayed

| Parameter | Value | Source |
|-----------|-------|--------|
| Pauli blocking threshold | E_F = 0.40 eV | Kubo formalism |
| ON state Fermi level | 0.52 eV | n = 1.6×10¹³ cm⁻² |
| Write energy | 65 fJ/state | Xu et al. 2025 |
| Extinction ratio | 3 dB/cell | FDTD taper geometry |
| V_gate (corrected) | 1.49 V | Incl. quantum capacitance |
| Retention | 10 yr projected | Accelerated lifetime testing |
| Static inference power | 0 pW | Non-volatile |

## Programme context

This simulation accompanies a four-paper research programme on 
non-volatile photonic weight memory for AI acceleration:

- **Paper 1** — Ferroelectric grain boundary polarisation as a 
  hidden variability source
- **Paper 2** — The weight bottleneck: 192 pJ/weight DRAM reload 
  vs 0.1 fJ/MAC photonic compute
- **Paper 3** — Diamond-integrated FERRO-PCM device architecture
- **Paper 4** — Graphene integration route selection: Bayesian 
  Monte Carlo across ten process scenarios

Simulation code and prior parameter files:
[graphene-photonic-memory-routes](https://github.com/bluebflatminor/graphene-photonic-memory-routes)

Computational simulation specifications:
[espresso-ferro-pcm](https://github.com/bluebflatminor/espresso-ferro-pcm)

## Contact

Nils Haaland — nhaaland@yahoo.com  
Solbakken Research Initiative (Independent)
