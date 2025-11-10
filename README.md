# Optical characterization of 2D TMDs — reproducible pipeline (embargoed)
**Status:** ⛔️ *Code & data under embargo until manuscript acceptance.*  
**Contact for early access:** german.amian.mata@univie.ac.at

This repository documents my MSc thesis project at the University of Vienna: a **reproducible Python pipeline** for optical characterization of 2D transition‑metal dichalcogenides (TMDs), combining **transfer‑matrix (TMM) modeling** with **spectral (Voigt) fits**, **model selection (AIC/BIC)**, and **bootstrap uncertainty**.  
It is intended for researchers who need **transparent, end‑to‑end analysis** where *models meet data*.

---

## TL;DR
- Goal: bridge **theory ↔ experiment** with an auditable pipeline for ΔR/R and PL spectra of 2D TMDs.  
- Approach: **TMM** + **Voigt components** (e.g., A⁰, A⁻), **diagnostics**, **AIC/BIC**, **bootstrap**; figure‑ready plots.  
- What’s public now: **overview, methods summary, and one figure**. Full code/data released **after journal acceptance**.

---

## Why this matters (for complexity & open science)
- Provides **simple, testable models** with clear assumptions and **limits**.  
- Emphasizes **reproducibility**: same inputs → same figures; auditable notebooks; versioned configs.  
- Designed to be **portable** to related spectroscopy problems and educational use.

---

## Methods at a glance
- **Transfer‑matrix modeling (TMM):** multilayer stacks; reflectance/contrast predictions.  
- **Spectral fitting (Voigt):** minimal components (A⁰/A⁻) over **transparent baselines**; residuals & sensitivity.  
- **Model selection:** **AIC/BIC** comparisons; avoid overfitting.  
- **Uncertainty quantification:** **bootstrap** CIs for peak parameters and composite fits.  
- **Diagnostics:** component overlays, residual plots, and marked peak centers for interpretability.  

<div align="center">
  
**Example figure (illustrative only)**  
  
<img src="assets/pl_fit.png" alt="PL Voigt fit example" width="640"/>
  
</div>

---

## What is released now
- This **documentation page** (README) describing the scope, structure, and methods.  
- One **illustrative figure** (no raw data).  
- **Embargo policy** and contact pathway for early access.

## What will be released after acceptance
- **Code:** packaged as `tmd-optics` (TMM + fits + UQ + plotting), with tests and examples.  
- **Data:** small example datasets + synthetic benchmarks.  
- **Environment:** `environment.yml` (conda) + `requirements.txt`; deterministic seeds.  
- **Reproduction scripts:** one‑click re‑generation of all main figures.  
- **Docs:** short API pages and usage tutorials.

> If you are a reviewer/collaborator and need access sooner, see **Early access** below.

---

## Early access (under embargo)
If you need to evaluate or build upon this work **before acceptance**, please email me with:
- Your affiliation and intended use (replication, extension, teaching, etc.).  
- Agreement to a short **confidentiality clause** (no public redistribution before release).  
- A GitHub/GitLab username (for private repo access).

**Template:**  
```
Subject: Early access request — TMD optics pipeline (embargoed)

Dear Germán,
I would like to request early access to your TMD optics pipeline for [purpose].
Affiliation: [lab/institution]. GitHub: [user]. I agree not to redistribute any
files publicly before the official release. Best, [Name]
```

---

## Planned repository structure
```
tmd-optics/               # package (to be released)
  ├─ src/tmdoptics/       # TMM, fits, UQ, plotting
  ├─ tests/               # unit tests
  ├─ notebooks/           # analysis & figures
  ├─ data/                # small sample datasets (post-release)
  ├─ docs/                # short API + tutorials
  ├─ environment.yml      # conda env (exact versions)
  └─ LICENSE
```

---

## Citation
Until the preprint is online, please cite as:  
**G. Amian Mata**, *Optical characterization of 2D TMDs via transfer‑matrix modeling and spectral fitting* (MSc thesis, University of Vienna, 2025), **manuscript in preparation**.

A formal citation (preprint DOI) will be added here upon release.

---

## License
- **Documentation (this README and figures):** CC BY 4.0.  
- **Code (upon release):** MIT License (unless constraints from co-authors require a different license).

---

## Acknowledgments
Supervision and lab support: Walther Group (University of Vienna). Thanks to collaborators and colleagues for feedback on modeling and measurement procedures.

---

## Contact
Questions or collaboration ideas: **german.amian.mata@univie.ac.at**
