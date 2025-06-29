# 🧠 PhantomSanity – Trust Logic Engine

_PhantomSanity is the behavioral confidence core of PhantomMesh. It continuously evaluates entropy, intent drift, and session rhythm to classify whether a session deserves trust—or diversion._

This module doesn't block—it redirects. Trust isn't binary here. It's spectral, adaptive, and always recalibrating.

---

## 🔍 Purpose

To determine:
- Whether a session adheres to known behavior patterns
- If entropy drift suggests intent shift or automation
- When to escalate from monitoring to active deception

PhantomSanity acts as the **dynamic perimeter**, constantly shifting and learning.

---

## 🧬 Core Components

### `Trust Drift Engine`
- Continuously evaluates live entropy signatures
- Compares against whitelisted baselines
- Calculates trust decay over time

### `Confidence Scorer`
- Produces a trust score between `0.0` (no trust) and `1.0` (full trust)
- Inputs include:
  - Entropy profile
  - Navigation cadence
  - Key/input timing
  - Session jitter
- Output drives session routing

### `Baseline Profile System`
- Stores known “legit” session shapes
- Can auto-learn baselines or rely on manual whitelisting
- Supports multi-device, multi-identity behavioral modeling

---

## 🧠 Trust Scoring Model

| Metric                  | Weight (%) | Description                              |
|-------------------------|------------|------------------------------------------|
| Entropy Stability       | 40%        | Measures randomness across session input |
| Navigation Predictivity | 25%        | Patterns consistent with known users     |
| Input Cadence Harmony   | 20%        | Rhythm coherence based on prior traces   |
| Device/Posture Match    | 15%        | Does this device “feel” familiar?        |

Trust scores below critical thresholds are rerouted into Phantom tiers.

---

## 📉 Behavior Triggers

| Trigger                         | Action                              |
|----------------------------------|-------------------------------------|
| Trust Score < 0.5               | Route to Phantom Sandbox (`Tier 2`) |
| Entropy drop > configured floor | Begin loop logging + flag for lock  |
| Drift from baseline > tolerance | Flag anomaly + log decision path    |
| Known exploit pattern detected  | Escalate directly to Tier 3 traps   |

---

## 🔁 Logging & Transparency

Supported logging modes:
- `statistical` – lightweight metrics only
- `narrative` – includes decision trees, thresholds hit, anomaly paths
- `forensic` – full replay-ready behavior telemetry

These are configured via `config/phantomsanity.yaml`.

---

## ⚠️ Notes

- PhantomSanity is **non-blocking by design**. It never denies traffic—it deflects and learns.
- Operates best in **adaptive mode**, with periodic tuning during low-traffic cycles.
- If deployed with `auto_baselining = true`, monitor early learning phases closely to avoid trust inflation.

---

## 🧾 Related Modules

- [`phantomledger.md`](./phantomledger.md) – Receives all trust scoring telemetry
- [`phantompulse.md`](./phantompulse.md) – Detects physical link anomalies that can inform scoring
- [`lockdown-protocol.md`](./lockdown-protocol.md) – Required if modifying trust decay constants in secure environments

---

> “The only true perimeter is perception.”  
> PhantomSanity bends perception until the threat either proves itself—or vanishes.

