# ZTGI-Pro v3 – Tek-Throne Risk–Stability Law for FPS-Based AI Systems

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.17625312.svg)](https://doi.org/10.5281/zenodo.17625312)

ZTGI-Pro v3 defines a **single-scalar risk–stability law** for LLM/agent systems
based on the *Tek-Throne axiom*:  
> **Within any causal closed region (CCR), only one permanent First-Person  
> Perspective (FPS) can exist; instability triggers a collapse Ω → single stream.**

This repository accompanies the v3 white paper and the live ZTGI-AC demo.

---

## 📄 White Paper (DOI)

**ZTGI-Pro v3: Tek-Throne Risk–Stability Law for FPS-Based AI Systems**  
Zenodo, DOI: https://doi.org/10.5281/zenodo.17625312

The paper formalizes:

- log-barrier hazard action  
- dual-EMA hazard memory  
- collapse law Ω  
- contextual threshold Θ(ψ)  
- single-scalar risk score  
- Phase-3 empirical validation (AUC, Brier, ECE)

---

## 🧪 Live Demo (ZTGI-AC / Tek-Throne Middleware)

A running LLaMA-based prototype implementing the full ZTGI-AC loop:

👉 **https://ztgiai.pages.dev/**

The demo exposes:

- jitter σ  
- dissonance ε  
- robustness ρ  
- coherence χ  
- hazard I, gate Q, energy H  
- free-energy F → E  
- contextual threshold Θ(ψ)  
- EMA hazards Hs, Hl, Ĥ  
- risk score r = Ĥ − H*  
- collapse flag Ω

---

## 🔬 Model Overview

### **Hazard Action**

The core hazard function:

```math
I(\sigma, \varepsilon, \rho, \chi)
= a\,\phi(\sigma)
+ b\,\phi(\varepsilon)
+ d\,\psi(\chi)
+ c\,\tilde{\gamma}(\rho)

