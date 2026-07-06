# Edison Scientific Literature Scan — Autonomous Structural Alloy Discovery (July 2026)

This document summarizes a set of five high-effort literature queries run through
[Edison Scientific](https://www.edisonscientific.com/) (FutureHouse `paperqa3-high`
/ `LITERATURE_HIGH`) on 2026-07-06 to find related work — in the US and
internationally — on **autonomous discovery of structural metallic alloys**,
including **additively manufactured** alloys. The queries deliberately favored
groups building **experimental** self-driving labs (SDLs) and studies with
**experimental validation**, while still capturing more isolated ML / automation
studies.

The candidates surfaced here feed the workshop speaker shortlist in
[`../SPEAKERS.md`](../SPEAKERS.md); the strongest experimentally grounded, on-topic
names have been added to that file.

> Caveat: Edison answers are AI-generated literature syntheses with citations.
> Affiliations, platform claims, and career stage should be spot-checked before
> issuing invitations. A couple of citations were flagged by the tool as weakly
> resolved (noted below).

## Queries run

1. **SDL builders** — groups directly building self-driving / closed-loop
   experimental platforms for structural alloys (favoring demonstrated hardware).
2. **Additive manufacturing** — autonomous / high-throughput / ML-guided discovery
   and process optimization of AM structural alloys (LPBF, DED, WAAM).
3. **High-throughput experimental** — HT synthesis + characterization combined with
   ML / Bayesian optimization for structural alloys.
4. **Isolated ML + automation** — ML / active-learning campaigns that were
   experimentally validated by fabricating and testing the proposed alloys.
5. **International** — non-US efforts (Europe, UK, Japan, China, Korea, etc.).

## Key groups and platforms (experimentally grounded)

### United States

| PI / group | Institution | Platform / approach | Alloy systems | Representative citation |
|---|---|---|---|---|
| Sebastian A. Kube | University of Wisconsin–Madison | **AlloyBot** — autonomous weighing + arc-melting bulk alloy synthesis (~1 alloy/hr, >150/week) | Ti-6Al-4V; Ti20Zr20Hf20Nb20Ta20 refractory HEA; Zr-Cu-Ni-Al metallic glass | Selvaraj et al., *AlloyBot: On-Demand Synthesis of Bulk Alloys by Automatic Arc-Melting* (2026), doi:10.21203/rs.3.rs-9761885/v1 |
| Ichiro Takeuchi; A. Gilad Kusne; Ji-Cheng Zhao | Univ. of Maryland; NIST | **AMASE** — autonomous phase-diagram search coupling processing, XRD, CALPHAD & Bayesian active learning (6× fewer experiments) | Sn-Bi thin-film phase diagram; alloy phase-boundary mapping | Liang et al., *Real-time experiment-theory closed-loop interaction for autonomous materials science*, *Sci. Adv.* (2025), doi:10.1126/sciadv.adu7426 |
| A. Gilad Kusne; Ichiro Takeuchi | NIST; Univ. of Maryland | **CAMEO** — autonomous synchrotron beamline phase mapping & property optimization | Ge-Sb-Te composition spreads (exemplar autonomous alloy experimentation) | Kusne et al., *On-the-fly closed-loop materials discovery via Bayesian active learning*, *Nat. Commun.* (2020) |
| Todd C. Hufnagel; K. T. Ramesh | Johns Hopkins University | **AIMD-L** — robotic HT characterization lab (laser shock, XRD/XRF, nanoindentation) accepting AI-agent instructions | Cu-Ti combinatorial alloys; structural metals for extreme environments | Hufnagel et al., *AIMD-L: An automated laboratory for high-throughput characterization of structural materials for extreme environments* (2026) |
| Dan J. Thoma; Jason R. Hattrick-Simpers; Phalgun Nelaturu | University of Wisconsin–Madison | High-throughput **DED** MPEA discovery with independent hopper control + batch active learning | Cr-Fe-Mn-Ni MPEAs | Nelaturu et al., *Multi-principal element alloy discovery using directed energy deposition and machine learning* (2024) |
| Raymundo Arróyave; Ibrahim Karaman; James Paramore | Texas A&M University | **BIRDSHOT** — batch Bayesian optimization + vacuum arc melting + automated/HT mechanical characterization | Al-V-Cr-Fe-Co-Ni FCC HEAs; Ti-V-Nb-Mo-Hf-Ta-W refractory CCAs | Paramore et al., *Two-shot optimization of compositionally complex refractory alloys*, *Acta Mater.* (2025); Hastings et al. (2024) |
| Kenneth S. Vecchio | UC San Diego | **HT-READ** — DED 16-sample ring libraries + automated XRD/EDS/EBSD + autoML closed loop | Ni-based superalloys (IN625 variants) | Vecchio et al., *Acta Mater.* 221, 117352 (2021) |
| Paulette Clancy | Johns Hopkins University | **PAL 2.0** — closed-loop Gaussian-process Bayesian active learning + rapid arc melting | Hard multi-principal-element alloys | Priyadarshini et al., *Machine-learning-driven closed-loop* (ChemRxiv, 2025) |
| Brad L. Boyce; David P. Adams; John F. Curry | Sandia National Laboratories | **BeyondFingerprinting** — AI-guided combinatorial PVD + automated HT tribology / tensile / XRD | Pt-Au, Ni-Fe thin-film alloys | Boyce et al. (2024); Babuska et al. (2026); Bassett et al., *IMMI* 12, 430 (2023) |
| Surya R. Kalidindi; Christopher J. Saldana | Georgia Institute of Technology | High-throughput AM + ML process–structure–property linkages (spherical indentation, small-punch) | DED Ni superalloys (IN625/IN100), Ti-Ni, Ti-6Al-4V, IN718 | Adapa et al., *Annu. Rev. Mater. Res.* (2025); Adapa et al. (2026) |
| Sergei V. Kalinin; Dayakar Penumadu | University of Tennessee, Knoxville | Cost-aware Bayesian nanoindentation planning on combinatorial libraries | Multi-component structural alloy spaces | Chawla et al., arXiv (2024/2025) |
| Karen Chen-Wiegart | Stony Brook Univ. / Brookhaven National Lab | Autonomous synchrotron mapping of alloy dealloying over multi-D parameter space | Ti-Cu (dealloyed by Mg); ternary systems | Noack & Sethian, *Autonomous discovery in science and engineering* (2021) |
| Daniel B. Miracle; Katharine M. Flores | AFRL; Washington University in St. Louis | Roadmap + partial demo for closed-loop combinatorial HT structural-alloy discovery (AM libraries, robotics, ML) | HEAs/MPEAs (Al_xCoCrFeNi via HT laser deposition) | Miracle et al., *Emerging Capabilities for the High-Throughput Characterization of Structural Materials* (2021) |
| Benji Maruyama | Air Force Research Laboratory | **ARES / ARES OS** — foundational autonomous experimentation & orchestration stack (enabling infrastructure) | CNT growth (demonstrated); generalizable | Sloan et al., *ARES OS 2.0* (2026); Stach et al. (2021) |

### International

| PI / group | Institution | Country | Approach | Alloy systems | Representative citation |
|---|---|---|---|---|---|
| Alfred Ludwig | Ruhr University Bochum | Germany | Combinatorial magnetron-sputtered thin-film libraries + active-learning (GPR) HT characterization | NiTi-based SMAs; CoCrFeNi HEA libraries | Thelen et al., *Digital Discovery* (2023); Ludwig, *npj Comput. Mater.* (2019) |
| Ziyuan Rao; Dierk Raabe; Hongbin Zhang | Max-Planck-Institut für Sustainable Materials (MPIE); TU Darmstadt | Germany | Active learning + generative models + ensemble regression with experimental casting/dilatometry feedback | Invar HEAs, magnetic alloys, TRIP steels | Rao et al., *Science* 378, 78 (2022); Rao et al., *Phil. Trans. R. Soc. A* (2024) |
| Penghui Yang; Zheng Liu; Bo An | Nanyang Technological Univ.; Singapore Management Univ. | Singapore | **AutoMAT** — LLM-guided ideation + automated CALPHAD + AI search + experimental validation | Low-density Ti alloys; AlCoCrFeNi HEAs | Yang et al., *AutoMAT: A Hierarchical Framework for Autonomous Alloy Discovery* (2025) |
| KIMS autonomous alloy-development lab (Hwang et al.) | Korea Institute of Materials Science (KIMS), Changwon | South Korea | Self-driving alloy lab: robotic handling, arc melting, tube-furnace annealing, XRD, RL-based process refinement | Alloy-development platform (systems unspecified) | Hwang et al., *Digital Discovery* (2026) |
| Lijun Zhang | Central South University | China | High-throughput CALPHAD + Bayesian optimization / active learning with experimental casting & hardness/corrosion validation | Al-Si-Mg-Sc casting alloys; die-casting Al; lightweight refractory HEAs | Gao et al., *STAM* (2023); Gao et al., *npj Comput. Mater.* (2024) |
| Hyoung Seop Kim; Seungchul Lee | POSTECH | South Korea | Deep-learning HEA phase prediction (Bayesian HPO, cGAN augmentation, interpretability) | HEAs across phase classes | Lee et al., *Mater. Des.* (2021) |
| Tong-Yi Zhang; Qinghua Wei | Materials Genome Institute, Shanghai University | China | Multi-objective Bayesian active learning (twin GPR) with full experimental validation | SAC387-based lead-free solder alloys | Wei et al., *npj Comput. Mater.* 11, 10 (2025) |
| Jan Rossmeisl; Jack K. Pedersen (CHEAC) | University of Copenhagen | Denmark | Bayesian optimization + DFT with targeted composition-spread validation | Ag-Ir-Pd-Pt-Ru & Ir-Pd-Pt-Rh-Ru HEAs (catalysis-focused) | Pedersen et al., *Angew. Chem. Int. Ed.* (2021) |
| Ehsan Ghassemali | Jönköping University | Sweden | High-throughput CALPHAD + ML compositional pruning before experimental validation | HEAs / MPEAs (phase-stability screening) | Ghassemali & Conway, *Front. Mater.* (2022) |
| Xun-Li Wang / Turab Lookman collaborators (Tian et al.) | Xi'an Jiaotong Univ.; Los Alamos National Lab | China; USA | Active learning (Kriging + SVM + Bayesian design) with experimental phase-diagram validation | NiTi-based shape-memory alloys | Tian et al., *Adv. Sci.* 8, 2003165 (2021) |

## Notes and gaps

- **US-dominated field.** Fully closed-loop SDLs that autonomously synthesize
  *bulk* structural alloys, characterize microstructure + mechanical properties,
  and iterate composition/processing end-to-end are still emerging; most groups
  have demonstrated individual building blocks or partially closed loops.
- **Additive manufacturing** autonomy is concentrated at Georgia Tech
  (Kalidindi/Saldana), Texas A&M (Arróyave/Elwany/Karaman), UW–Madison
  (Thoma/Hattrick-Simpers), and Northwestern (Chen/Cao), plus international LPBF
  ML efforts (e.g., Su et al., NUS/SIMTech, Singapore; Kosarava et al., Warsaw
  Univ. of Technology, Poland — H13 tool steel).
- **Weakly resolved citations** (treat with caution): the Jörg Kaspar group
  (TU Dresden / Fraunhofer IWS) combinatorial DED entry was flagged by Edison as
  unobtainable in the retrieved evidence and is included only as a lead.
- **Adjacent SDL precedents** (not alloy-specific): Leroy Cronin (Univ. of
  Glasgow) and Andrew I. Cooper (Univ. of Liverpool) — strong autonomous-lab
  precedents but not demonstrated on structural metallic alloys.
