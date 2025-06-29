# 🛰️ PhantomPulse – Signal Integrity Core

_PhantomPulse monitors the rhythms that most systems ignore—timing, pressure, and continuity. It serves as PhantomMesh’s “sixth sense,” identifying anomalies in signal flow that may indicate tampering, spoofing, or physical compromise._

It’s the watchdog for latency lies and clock-drift smokescreens.

---

## 🎯 Purpose

To detect:
- Link-level spoofing or mirroring attempts
- Clock skew or entropy injection
- Layer 1 or Layer 2 side-channel probes
- Timing discrepancies caused by adversarial man-in-the-middle behavior

---

## 🔑 Key Features

### `Heartbeat Monitor`
- Continuously pings subsystems, physical nodes, and sensors
- Baselines normal response time and jitter
- Flags asynchronous packet flow or injected response queues

### `Entropy Divergence Detection`
- Monitors input variance in microtiming
- Flags patterns that defy biological consistency (e.g. robotic keystrokes)
- Can emit entropy deltas into PhantomSanity or Ledger

### `Clock Integrity Watchdog`
- Cross-references NTP and local hardware clocks
- Detects drift suggesting sandbox emulation or time-shift evasion
- Supports attestation from secure TPM-based modules

---

## 📉 Observable Metrics

| Metric                     | Role                                         |
|----------------------------|----------------------------------------------|
| Round-trip latency jitter  | Link trustworthiness baseline                |
| Timestamp drift            | Emulator detection, latency spoof flags     |
| Keystroke timing harmony   | Entropy shaping metric for user profiling    |
| Signal sync failure rate   | Possible relay or fragmentation behavior     |

---

## 🔒 Trust Hooks

PhantomPulse feeds real-time metrics into:
- [`phantomsanity.md`](./phantomsanity.md): for live trust scoring input
- [`phantomledger.md`](./phantomledger.md): for timestamp signing
- [`lockdown-protocol.md`](./lockdown-protocol.md): for override key enforcement

---

## 🧰 Configuration

Currently controlled via `phantompulse.conf` (not yet exposed for public config):

- Pulse interval
- Acceptable jitter thresholds
- Entropy anomaly shaping parameters
- Clock attestation validation window

---

## 🧪 Simulation Usage

For red team exercises:
- Can simulate timing jitter profiles
- Will auto-detect scripted sequences with identical cadence
- Ideal for identifying macro-based or remote GUI injection

---

> “Every attack has a tempo. PhantomPulse listens to the rhythm between the moves.”  
