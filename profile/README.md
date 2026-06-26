# 🧑‍🌾 MutFarm Homelab

<div align="center">
  <img src="../img/MutFarm_Logo.png" alt="MutFarm Logo" width="200"/>
</div>

My Kubernetes playground where I break stuff and learn from it.

![Kubernetes](https://img.shields.io/badge/kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Talos](https://img.shields.io/badge/Talos-FF6C37?style=flat-square&logo=linux&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=flat-square&logo=helm&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)

---

## What's this?

Started this homelab to get my hands dirty with Kubernetes and DevOps stuff. No fancy cloud bills, just bare metal at home running Talos Linux. When things break, I actually learn something.

## Running on the farm

**Infrastructure:**
- ☸️ Kubernetes cluster on Talos Linux (4 nodes: Bela, Brina, Nerina, Dori le mie Ache ❤️)
- 📦 Longhorn for distributed storage
- ⚖️ MetalLB for load balancing
- 🔒 cert-manager + Let's Encrypt (wildcard certs via Cloudflare DNS)
- 🚪 ingress-nginx for routing
- 🐮 Rancher for cluster management UI

**Observability:**
- 📊 kube-prometheus-stack — Prometheus, Grafana, Alertmanager, node-exporter
- ⚡ Kepler — per-node & per-pod power consumption via RAPL hardware counters
- 📧 Alert notifications via Resend SMTP to email

**Applications:**
- 🕒 Custom Go app for Kimai time tracking automation (weekly/monthly reports)
- 📷 Immich — self-hosted photo library
- 🛡️ AdGuard Home — DNS filtering & ad blocking
- 🎮 Minecraft server
- 📹 Bash scripts for Reolink cameras API
- 🔧 it-tools, smtp-relay, and other self-hosted utilities

## The code

```
cert-manager/               → SSL automation
kubernetes/                 → Cluster configs and Talos setup
kube-prometheus-stack/      → Observability stack (Prometheus, Grafana, Alertmanager)
kepler/                     → Power consumption monitoring
kimai-export-scheduler/     → Go project (weekly/monthly time reports)
immich/                     → Photo library deployment
Adguard/                    → DNS filtering
reolink/                    → Camera API scripts
minecraft/                  → Game server deployment
rancher/                    → Management UI configs
longhorn/                   → Storage configuration
```

## Tech

Kubernetes • Talos Linux • Helm • Prometheus • Grafana • Kepler • Longhorn • MetalLB • cert-manager • ingress-nginx • Go • Docker • Bash

---
