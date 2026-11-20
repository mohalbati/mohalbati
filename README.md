# Mohammad Albati

**Safety and risk engineer · Probabilistic risk assessment (PRA) · Autonomous-vehicle safety · Bayesian methods for rare events**

I recently defended my Ph.D. in Nuclear, Plasma & Radiological Engineering at the University of Illinois Urbana-Champaign. I work on quantitative safety for complex systems: probabilistic risk assessment, human reliability analysis, common-cause failures, and uncertainty quantification for rare events. Before my Ph.D. I spent six years as a nuclear safety analysis engineer at the Jordan Research & Training Reactor, after two years at the Korea Atomic Energy Research Institute (KAERI). I'm now applying these methods to autonomous vehicles.

## Autonomous-vehicle safety portfolio

One question runs through these projects: **what evidence shows that a driverless vehicle is safe enough, and how far can each kind of evidence be trusted?**

**Crash-data rates → counterfactual uncertainty → field monitoring → simulation credibility → simulation as safety evidence**

| | Project | Question | Highlights |
|---|---|---|---|
| 1 | [**av-safety-bayesian-analysis**](https://github.com/mohalbati/av-safety-bayesian-analysis) [![DOI](https://zenodo.org/badge/1436574246.svg)](https://doi.org/10.5281/zenodo.23732384) | How much real-world evidence is enough? | Rebuilds a robotaxi crash record from public NHTSA reports (99.5% match to the published list) and applies rare-event Bayesian methods from nuclear PRA, including the miles a new operator needs before claiming a safety benefit |
| 2 | [**av-counterfactual-uq**](https://github.com/mohalbati/av-counterfactual-uq) [![DOI](https://zenodo.org/badge/1440901346.svg)](https://doi.org/10.5281/zenodo.23838254) | How certain is a counterfactual crash simulation? | Adds uncertainty to reference-driver benchmarking of reconstructed crashes: in 14 of 16 test conflicts the deterministic verdict flips with probability above 20%. Browser simulator, video and CARLA 3D demo |
| 3 | [**av-safety-monitoring**](https://github.com/mohalbati/av-safety-monitoring) [![DOI](https://zenodo.org/badge/1441811364.svg)](https://doi.org/10.5281/zenodo.23858361) | Can field data catch a safety regression? | Test coverage, Poisson CUSUM monitoring and an automated release health report: field data catch a 25% rise in all crashes in about 6 fleet-weeks, but serious-injury regressions only after decades, so release gating must rest on scenario testing |
| 4 | [**av-sim-credibility**](https://github.com/mohalbati/av-sim-credibility) | How far can simulated road users be trusted? | Compares closed-loop simulation (Waymax, simple rule-based drivers) with 2,000 recorded Waymo Open Motion Dataset scenes, scenario type by scenario type and in the dangerous tail, then decides what the simulation may be used for (ASME V&V 40 logic) and how much simulated exposure is worth |
| 5 | [**av-sim-vnv-evidence**](https://github.com/mohalbati/av-sim-vnv-evidence) | When does simulation save real-world testing? | Combines simulated and recorded outcomes of the same scenarios with prediction-powered inference (PPI, PPI++). The saving follows 1/(1 − ρ²) in the per-vehicle agreement, so matching the average rate is not enough; the fused estimates stay valid even when the simulator is biased |

**In progress:** *av-redundancy-ccf*: how much an independent safety guard adds to the main driving stack, measured with the common-cause failure methods of PRA (not yet public).

Each project has a technical report written for non-specialists, automated tests and one-command reproduction. The analysis code was written with AI assistance; I designed the studies and ran and checked every result. Waymo Open Dataset material is used under its non-commercial licence, and no scene data is redistributed.

## Research highlights (Ph.D.)

- **Simulation-Informed Probabilistic Dependency Analysis (SIP-DA).** MOOSE and RAVEN-based modelling of common-cause failures coupled with physical degradation and maintenance, developed with Constellation, Idaho National Laboratory, EPRI, Southern Company and X-energy.
- **Integrated Human Reliability Analysis (I-HRA).** Agent-based simulation combined with THERP, SPAR-H and IDHEAS for emergency response outside the main control room, applied to FLEX deployment under external flooding.
- **Fire PRA.** Experimental, uncertainty-based validation of simulations of fire-response team performance.

## Selected publications

- Albati M., et al. "Integrated Human Reliability Analysis Methodology for External Control Room Emergency Response Scenarios: Application to Modeling FLEX Human Actions in Nuclear Power Plants." *ASME J. Risk and Uncertainty in Engineering Systems, Part B*, 2025. [doi:10.1115/1.4068539](https://doi.org/10.1115/1.4068539)
- Albati M., et al. "Uncertainty-Based Validation Methodology and Experimental Analysis for External Control Room Human Performance Simulation: Application to Fire PRA of Nuclear Power Plants." *Nuclear Science and Engineering*, 2024. [doi:10.1080/00295639.2024.2366735](https://doi.org/10.1080/00295639.2024.2366735)
- Albati M., et al. "Simulation-Informed Dependency Treatment to Enhance Operational Flexibility, Avoid Production Loss, and Maintain Safety of Operating Plants and Advanced Reactors." *Proc. PSA 2025*, American Nuclear Society.

Full list: [Google Scholar](https://scholar.google.com/citations?user=hseZ6CIAAAAJ&hl=en)

## Tools

`Python` · `NumPy / SciPy` · `JAX (Waymax)` · `MATLAB` · `C++` · `MOOSE` · `RAVEN` · `RISKMAN` · `OpenBUGS` · `GeNIe` · `NetLogo` · `Monte Carlo and Bayesian inference` · `Linux / HPC (SLURM)` · `Git`

## Contact

[LinkedIn](https://www.linkedin.com/in/mohammad-a-4b03903b) · [Google Scholar](https://scholar.google.com/citations?user=hseZ6CIAAAAJ&hl=en) · [ORCID](https://orcid.org/0000-0002-3096-5650) · malbati2@illinois.edu · drmalbati2@gmail.com
