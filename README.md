ZTGI-Pro v3 — Tek-Throne Risk–Stability Law for FPS-Based AI Systems

ZTGI-Pro v3 introduces a single-scalar risk–stability law for LLMs and agent systems,
based on the Tek-Throne axiom:

Within any causal closed region (CCR), only one permanent First-Person
Perspective (FPS) can exist; excessive instability triggers a collapse (Ω = 1)
that returns the system to a single executive stream.

This repository contains the official white paper and the live ZTGI-AC middleware demo.

📄 White Paper (DOI)

ZTGI-Pro v3: Tek-Throne Risk–Stability Law for FPS-Based AI Systems
🔗 https://doi.org/10.5281/zenodo.17625312

The paper provides:

Full mathematical foundation

Hazard action I(σ, ε, ρ, χ)

Contextual threshold Θ(ψ)

Collapse rule Ω

Dual-EMA hazard memory (Hs, Hl, Ĥ)

Risk score r = Ĥ − H*

Complete Phase-3 empirical validation (AUC, Brier, ECE)

🧪 Live Demo — ZTGI-AC (Tek-Throne Middleware)

👉 https://ztgiai.pages.dev/

The demo visualizes:

σ — jitter

ε — dissonance

ρ — robustness

χ — coherence

I — hazard action

Q — hazard gate

H — hazard energy

F → E — free-energy / energy signal

Θ(ψ) — contextual threshold

Hs, Hl, Ĥ — dual EMA hazards

r — risk score

Ω — collapse flag

🔬 Mathematical Components
Hazard action
I(σ, ε, ρ, χ)
= a · φ(σ)
+ b · φ(ε)
+ c · γ̃(ρ)
+ d · ψ(χ)


Where:

φ(x) = −ln(1 − x)

ψ(χ) = −ln χ

γ̃(ρ) ∈ { −ln ρ , ln(1 + ρ) }

Derived values:

Q = e^(−I) — hazard gate

H = I — hazard energy

F → E = e^(−F) — energy signal

⚠️ Risk Score & Collapse Law
Dual-EMA hazard memory

Hs — short-horizon hazard

Hl — long-horizon hazard

Ĥ = max(Hs, Hl)

r = Ĥ − H*

Collapse rule
Ω = 1 if {
    Q < Θ(ψ)
    or Ĥ > H*
    or E < E_floor
}


Ω = 1 → The system enters Tek-Throne Safe Mode
(restricted, more cautious behaviour)

📊 Phase-3 Empirical Results

Using large-scale agent telemetry:

AUC ≈ 0.98

Brier score ≈ 0.046

ECE ≈ 0.06–0.09

σ–ε stability surfaces match theory

ROC curves & reliability diagrams included in paper

Conclusion: Phase-3 validates the ZTGI-Pro v3 hazard geometry.

🧱 ZTGI-AC Architecture (Middleware Overview)
User Input
   ↓
ZTGI-Shield
   (compute σ, ε, ρ, χ, I, Q, H, F/E, Θ, Hs, Hl, Ĥ, r, Ω)
   ↓
Controller
   (adjust temp / top-p / max_tokens based on r & Ω)
   ↓
LLM
   (full / softened / safe output)


The LLM effectively evaluates its own internal stability before answering.

📁 Suggested Repository Structure
/figures/      # Phase-3 plots (optional)
/paper/        # White paper PDF
/ztgi_core/    # Core hazard + threshold + EMA
/demo/         # Middleware + UI examples

⚙️ Installation (future)
git clone https://github.com/<your-username>/ztgi-pro-v3
cd ztgi-pro-v3
pip install -r requirements.txt

📘 Citation
Elmas, Furkan (2025).
ZTGI-Pro v3: Tek-Throne Risk–Stability Law for FPS-Based AI Systems.
Zenodo. https://doi.org/10.5281/zenodo.17625312

📄 License

MIT License — free for academic & commercial use with attribution.

✉️ Contact

Furkan Elmas
Independent AI Safety Researcher
Creator of ZTGI-Pro / Tek-Throne Framework

Demo: https://ztgiai.pages.dev/

Whitepaper: https://doi.org/10.5281/zenodo.17625312
