# 👁️ PhantomSentinel – Passive Signature Correlation Layer

_PhantomSentinel is the passive intelligence layer of PhantomMesh. It watches without influence. Listens without reacting. Tracks entropy, behavior bleed, and routing outcomes in real-time, forming the statistical backbone of anomaly propagation._

It’s not here to engage. It’s here to remember.

---

## 🎯 Purpose

- Aggregate behavioral signals across multiple modules
- Create passive correlation clusters without affecting trust scores directly
- Feed emerging patterns back into the simulation and scoring pipeline
- Record “soft signals” that don’t justify immediate reroute but still deserve memory

---

## 🧠 Passive Signal Models

### `Session Fingerprint Delta`
- Compares current session markers to anonymized deltas from past sessions
- Assigns a non-executing "similarity tension score"

### `Anomaly Decay Logic`
- Calculates likelihood that a mild anomaly is a false positive or a pattern emerging
- Supports decay timers per anomaly type

### `Shadowmap Generator`
- Creates per-device behavior heatmaps over time
- Highlights frequency hotspots of:
  - Deception triggers
  - Trust wavers (0.45–0.60 score band)
  - Unrouted fluctuations

---

## 📉 Recorded Signals (Sample)

| Signal Type               | Value Range   | Used For                        |
|---------------------------|---------------|----------------------------------|
| Trust Tension Score       | `0.00–1.00`   | Identifies “almost anomalies”   |
| Schema Drift Frequency    | integer       | Tracks evasive communication    |
| Temporal Recurrence Delay | ms or ticks   | Detects botnet retry loops      |
| Unacted Entropy Spikes    | float (0–1)   | Potential probe signal          |

---

## 🔁 Feedback Loop

PhantomSentinel does **not** act directly. It:
- Suggests patterns to PhantomSanity during low-load cycles
- Provides correlation maps for audit via PhantomLedger
- Flags decay thresholds to PhantomPulse for tuning

---

## 🧰 Configuration

Not currently configurable at runtime. This module is:
- Passive by design
- Tuned in pre-deploy environment snapshots
- Influence scores reviewed post-deployment for future tuning

---

## ⚠️ Notes

- PhantomSentinel’s data can be selectively trained on by adversaries. Avoid surfacing its metrics outside replay tools or analytics consoles.
- Ideal for red team exercises where real-time aggression is not permitted.
- Works especially well in long-session environments (e.g., persistent shell engagement, malware orchestration sandboxing).

---

> “If PhantomSanity is reflex, PhantomSentinel is memory.”  
> Sometimes the mind doesn’t react—because it’s too busy remembering everything.
