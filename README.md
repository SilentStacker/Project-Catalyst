<div align="center">

# 🖥️ homelab-docs

**Physical Enterprise Network Homelab**

*Built from scratch while working full time*
*to develop real IT and network engineering skills*

---

![Status](https://img.shields.io/badge/Status-In%20Progress-yellow?style=for-the-badge)
![Rack](https://img.shields.io/badge/Rack-16U-blue?style=for-the-badge)
![Firewall](https://img.shields.io/badge/Firewall-SonicWall-red?style=for-the-badge)
![Router](https://img.shields.io/badge/Router-Cisco%20IOS%20XE-blue?style=for-the-badge)
![Switch](https://img.shields.io/badge/Switch-Managed%20PoE%2B-green?style=for-the-badge)
![Hypervisor](https://img.shields.io/badge/Hypervisor-Proxmox-orange?style=for-the-badge)

</div>

---

## 🎯 Goal

Build and document a physical enterprise network homelab
to develop hands on IT and networking skills while
working toward a career in IT support and network
engineering. Everything built solo on personal time
while working full time.

---

## 📸 The Build

> *Photo of rack goes here*

---

## 🔧 Hardware Stack

### Network Infrastructure
| Device | Model | Role | IP |
|--------|-------|------|----|
| 🔥 Firewall | SonicWall SOHO 250 | Gateway, VLANs, NAT, DPI | 10.10.10.1 |
| 🌐 Router | Cisco ISR 1100-4G | IOS XE, OSPF, ACLs | 10.10.10.2 |
| 🔀 Switch | Linksys LGS328PC | 24-port managed PoE+ | 10.10.10.3 |
| 📋 Patch Panel | LYSYMIXS 24-port CAT6 | Cable termination | — |

### Compute
| Device | Model | Role | IP |
|--------|-------|------|----|
| 💻 Hypervisor | HP ProDesk | Proxmox VE | 10.20.20.10 |
| 📊 Monitoring | HP EliteDesk | Grafana + Prometheus | 10.20.20.11 |

### Services — Raspberry Pi Cluster
| Device | Model | Role | IP |
|--------|-------|------|----|
| 🔐 VPN | Raspberry Pi 5 | WireGuard + Tailscale | 10.30.30.10 |
| 🛡️ DNS | Raspberry Pi 5 | Pi-hole DNS filter | 10.30.30.11 |
| 📈 Dashboard | Raspberry Pi 4 | Grafana dashboard | 10.30.30.12 |

### Wireless
| Device | Model | Role | IP |
|--------|-------|------|----|
| 📶 Node 1 | Linksys MX2000 | Lab WiFi VLAN 40 | 10.40.40.2 |
| 📶 Node 2 | Linksys MX2000 | Mom's room mesh | 10.40.40.3 |

### Management Station
| Device | OS | Role |
|--------|----|------|
| 💻 MacBook | Endeavour OS + Hyprland | SSH, console, Obsidian |
| 🖥️ Gaming PC | Fedora + Hyprland | Main workstation |

---

## 🌐 Network Design

### VLAN Segmentation
| VLAN | Name | Subnet | Purpose |
|------|------|--------|---------|
| 10 | Management | 10.10.10.0/24 | Network gear admin only |
| 20 | Servers | 10.20.20.0/24 | Proxmox, VMs, EliteDesk |
| 30 | Services | 10.30.30.0/24 | Raspberry Pi cluster |
| 40 | Lab WiFi | 10.40.40.0/24 | Wireless lab devices |
| 50 | Workstations | 10.50.50.0/24 | Gaming PC, wired clients |
| 99 | Guest | 10.99.99.0/24 | Isolated guest devices |

### Network Flow