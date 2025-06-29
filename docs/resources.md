# 🧠 PhantomMesh Resources & Node Traits

_This document defines the minimum, optimal, and extended resource profiles for deploying PhantomMesh. It also outlines node-level traits, environmental considerations, and simulation tier use cases._

Whether you're simulating trust drift in a VM or building a mirrored deception node—this is your operational baseline.

---

## 📊 Deployment Profiles

| Profile        | CPU Cores | RAM (GB) | Disk Space | Use Case                          |
|----------------|-----------|----------|------------|-----------------------------------|
| `whisper-node` | 2         | 4        | 10GB SSD   | Test harnesses, CI mocks          |
| `shadow-node`  | 4         | 8        | 25GB SSD   | Full trust engine simulation      |
| `phantom-core` | 8         | 16       | 100GB SSD  | Production trap deployment        |
| `sentinel-tier`| 16        | 32       | 200GB NVMe | Passive multi-node correlation    |
| `blackglass`   | 32+       | 64+      | 500GB+ SSD | High-fidelity deception grid lab  |

---

## 🧱 Node Role Traits

| Trait                  | Description                                  |
|------------------------|----------------------------------------------|
| `entropy-stable`       | Guaranteed timing precision                  |
| `mirror-capable`       | Can host redirector and fake interface sets  |
| `forensic-immortal`    | Has write-once vault and ledger bonding      |
| `pulse-synced`         | Linked to PhantomPulse NTP integrity mesh    |
| `lockdown-fused`       | Physically immutable trust boundaries        |

---

## 🌍 Environmental Profiles

| Environment     | Description                           |
|------------------|---------------------------------------|
| `sandboxed`      | Internal red team or CI simulation    |
| `mirror-grid`    | External-facing deception perimeter   |
| `isolation-lab`  | Air-gapped, behavioral pattern mining |
| `edge-node`      | Lightweight behavioral trap relay     |
| `replay-chamber` | Controlled environment for rerun logs |

---

## 🔁 Compatibility Notes

- All modules compatible with x86 and ARM64 Linux systems
- Best effort performance on macOS (dev only)
- Not recommended for Windows deployment (unless under WSL2)

---

## 🔒 Storage Notes

- Cold storage vault should be mounted with `noatime`, encrypted, and externally replicated
- High-write PhantomLedger nodes benefit from SSD with wear leveling
- Replay chambers may use write-once LFS block mappers (BPF or union mounts)

---

## 💡 Pro Tips

- Use `sentinel-tier` nodes to *learn* attacker behavior—not fight it
- Never run lockdown modules on VMs exposed to unknown hypervisors
- Name your nodes poetically. These aren’t servers—they’re characters in a story

---

> “Architecture is memory, and every node remembers differently.”  
> PhantomMesh lets each node whisper, observe, mislead—or simply wait.
