# 🚀 Project Catalyst

> Why Project Catalyst?

I built Project Catalyst to gain hands-on experience with enterprise infrastructure using the same technologies found in professional IT environments. Starting with an empty 16U rack, I've been documenting each stage of the project—from hardware installation and networking to virtualization and monitoring—while balancing a full-time, six-day work week. The goal is to continuously expand the lab and deepen my skills in systems administration, networking, and security.

![Status](https://img.shields.io/badge/Status-Active-success)
![Proxmox](https://img.shields.io/badge/Proxmox-VE-E57000)
![Docker](https://img.shields.io/badge/Docker-2496ED)
![Ubuntu](https://img.shields.io/badge/Ubuntu-Server-E95420)
![Grafana](https://img.shields.io/badge/Grafana-F46800)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C)
![Wazuh](https://img.shields.io/badge/Wazuh-SIEM-005571)
![SonicWall](https://img.shields.io/badge/SonicWall-NGFW-blue)

---

## 📖 About

Project Catalyst is my personal enterprise homelab where I design, build, secure, monitor, and document modern IT infrastructure.

The project began with an empty **16U rack** and has grown into a production-style environment featuring virtualization, enterprise networking, monitoring, and security tools.

Every major milestone is documented with photos, notes, and configuration files.

---

# 📑 Table of Contents
- Lab at a Glance
- Infrastructure
- Network
- Hardware
- Services
- Monitoring
- Security
- Build Timeline
- Documentation
- Roadmap

---
## 🏠 Lab at a Glance

| Category | Details |
|----------|---------|
| Rack | 16U |
| Gateway | SonicWall (192.168.168.168) |
| ISP Router | ARRIS Gateway |
| Core Switch | Linksys LGS328PC |
| Lab Switch | Cisco Catalyst 3560-CX |
| Router Lab | Cisco ISR 1100 |
| Wireless | 2× Linksys MX2000 Mesh Nodes |
| Virtualization | 2× Proxmox Hosts |
| Monitoring | Grafana, Prometheus, Node Exporter, cAdvisor |
| DNS | Pi-hole |
| Future | Wazuh, VLANs, Active Directory Expansion |

# 🏗 Current Infrastructure

- 🖥 HP EliteDesk 800 G4 Mini (Proxmox VE)
- 🔥 SonicWall Firewall (Primary Gateway)
- 🌐 ARRIS ISP Gateway
- 🔀 Linksys LGS328PC Managed PoE 24-port Switch
- 📡 Linksys MX2000 Mesh Wi-Fi (Bedroom)
- 📡 Linksys MX2000 Mesh Wi-Fi (Mother's Room)
- 🔧 Cisco Catalyst 3560-CX
- 🌍 Cisco ISR1100
- 🍓 Raspberry Pi 5 #1
- 🍓 Raspberry Pi 5 #2

---

# 🎯 Goals

- Learn enterprise networking
- Master virtualization
- Build secure infrastructure
- Practice Linux administration
- Implement monitoring and observability
- Document everything
- Continuously improve the lab

---

# 🚧 Current Status

## ✅ Operational

- 16U Rack Complete
- Proxmox VE Host
- Ubuntu Docker VM
- Grafana
- Prometheus
- Node Exporter
- cAdvisor
- Pi-hole
- SonicWall Gateway
- Linksys LGS328PC Managed Switch
- Linksys MX2000 Mesh Wi-Fi
- Raspberry Pi Monitoring Nodes

## 🚧 In Progress

- VLAN Design
- 802.1Q Trunk Configuration
- Firewall Rule Documentation
- Network Diagrams
- GitHub Documentation

## 📋 Planned

- Wazuh SIEM
- WireGuard VPN
- Tailscale
- Active Directory
- Ansible Automation
- Home Assistant
---

# 📸 Build Journey

This repository documents the complete build process, including:

- Rack assembly
- Cable management
- Network configuration
- Virtualization
- Monitoring
- Security
- Troubleshooting

More than 100 photos will be added throughout the documentation.

## 📚 Documentation

### Infrastructure

- [Hardware Inventory](docs/hardware.md)
- [IP Addressing](docs/networking/ip-addressing.md)
- [VLAN Plan](docs/networking/vlan-plan.md)
- [Network Topology](docs/networking/topology.md)
### Services

- [Proxmox](docs/services/proxmox.md)
- [Docker](docs/services/docker.md)
- [Prometheus](docs/services/prometheus.md)
- [Grafana](docs/services/grafana.md)
- [Pi-hole](docs/services/pihole.md)
- [Home Assistant](docs/services/home-assistant.md)
- [Active Directory](docs/services/active-directory.md)
---

# 📜 License

This project is licensed under the MIT License.

# 🗺️ Roadmap

## Phase 1 — Foundation ✅

- [x] Build 16U rack
- [x] Install Proxmox
- [x] Deploy Ubuntu Server
- [x] Configure Docker
- [x] Install Grafana
- [x] Install Prometheus
- [x] Configure Node Exporter
- [x] Configure cAdvisor
- [x] Deploy Pi-hole

## Phase 2 — Networking 🚧

- [ ] Configure VLANs
- [ ] Configure Trunk Ports
- [ ] Create Management VLAN
- [ ] Create Server VLAN
- [ ] Create Client VLAN
- [ ] Document Firewall Rules

## Phase 3 — Security

- [ ] Install Wazuh
- [ ] Configure Log Collection
- [ ] Configure Alerts
- [ ] Configure VPN Access

## Phase 4 — Automation

- [ ] Infrastructure Backups
- [ ] Ansible Playbooks
- [ ] Automated Monitoring