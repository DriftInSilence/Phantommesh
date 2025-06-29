# 🎮 Simulation Harness – Orchestration Layer for PhantomMesh Testing

_The Simulation Harness is the behavioral testbed for PhantomMesh. It acts as the conductor between SDK profiles, entropy injection modules, and reactive scoring layers._

Where PhantomSDK gives you parts, the Harness brings rhythm.

---

## 🎯 Purpose

To enable:
- Full-stack simulation of a live session within PhantomMesh
- Controlled entropy injection to trigger detection paths
- End-to-end logging for trust trajectory, reroute cascades, and trap deployment
- Profiling of modules under varied stress, mimicry, and deception loadouts

---

## ⚙️ Core Capabilities

### `Session Orchestrator`
- Orchestrates flow of time, behavior, and trust-state transitions
- Reads simulation profiles (`*.sim.yaml`) to construct synthetic sessions
- Connects to PhantomSanity, PhantomPulse, PhantomChannel in dry-run mode

### `Injection Synchronizer`
- Times entropy anomalies with input cadence
- Fakes clock drift, IP/OS fingerprint shifts, jitter envelopes

### `Replay Mirror`
- Intercepts output from PhantomLedger in real-time
- Compares actual system reroute/logging outcomes against expected profiles

---

## 📐 Simulation Stack Overview

     +----------------------+
     |  simulation-harness  |
     +----------+-----------+
                |
         +------▼------+
         | PhantomSDK  |
         +------+------+     
                |
        +-------▼-------+
        | PhantomSanity |
        +-------+-------+
                |
        +-------▼-------+
        | PhantomPulse  |
        +-------+-------+
                |
        +-------▼--------+
        | PhantomChannel |
        +-------+--------+
                |
        +-------▼--------+
        | PhantomLedger  |
        +----------------+

---

## 📁 Usage Workflow

1. Select a profile from `sdk/profiles/`
2. Launch `harness.py` in `dry-run` or `introspect` mode
3. Observe trust score trajectory and reroute behavior
4. Export `session.jsonl` from PhantomLedger for replay/validation
5. (Optional) Inject on-the-fly modifiers (e.g. jitter spike mid-session)

---

## 📊 Metrics Captured

| Metric                      | Description                            |
|-----------------------------|----------------------------------------|
| Trust Drift Path            | How trust score fluctuates over time   |
| Schema Drift Decision Tree  | When/why protocol channels switched    |
| Entropy Injection Accuracy  | Whether triggers hit expected modules  |
| Replay Divergence Index     | Gap between expected and actual reroute |

---

## 🛠️ Configuration Notes

- Simulation parameters live in `.sim.yaml` profiles
- Entropy modules configured via `sdk/inject/*.py`
- Logging behavior respects current `phantomledger.yaml` mode
- Replay environment must be initialized before dry-run sessions

---

> “The simulation harness is where mirrors are polished, and the lies become rehearsed truth.”  
> It’s where you bend trust before deploying it to face the wild.

