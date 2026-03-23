# 🧑‍🌾 MutFarm Homelab

<div align="center">
  <img src="MutFarm_Logo.png" alt="MutFarm Logo" width="200"/>
</div>

My Kubernetes playground where I break stuff and learn from it.

![Kubernetes](https://img.shields.io/badge/kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Talos](https://img.shields.io/badge/Talos-FF6C37?style=flat-square&logo=linux&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)

---

## What's this?

Started this homelab to get my hands dirty with Kubernetes and DevOps stuff. No fancy cloud bills, just bare metal at home running Talos Linux. When things break, I actually learn something.

## Running on the farm

**Infrastructure bits:**
- ☸️ Kubernetes cluster on Talos Linux (3 nodes: Bela, Brina, Nerina le mie Ache <3)
- 📦 Longhorn for storage (because I like my data distributed)
- ⚖️ MetalLB for load balancing
- 🔒 cert-manager + Let's Encrypt (wildcard certs via Cloudflare DNS)
- 🚪 ingress-nginx for routing
- 🐮 Rancher when I need a GUI

**Stuff I actually use:**
- 🕒 Custom Go app for Kimai time tracking automation (generates reports)
- 📹 Bash scripts for my Reolink cameras API
- 🎮 Minecraft server (because why not)
- 🛡️ AdGuard for DNS filtering
- 🔧 Various self-hosted tools

## The code

```
cert-manager/            → SSL automation
kubernetes/              → Cluster configs and Talos setup
kimai-export-scheduler/  → My Go project (weekly/monthly reports)
reolink/                 → Camera API scripts
minecraft/               → Game server deployment
rancher/                 → Management UI configs
```

## Tech

Kubernetes • Talos Linux • Go • Longhorn • MetalLB • cert-manager • Kustomize • Docker • Bash

---

