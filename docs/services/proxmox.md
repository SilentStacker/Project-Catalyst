# 🖥 Proxmox Virtual Environment

## Overview

Project Catalyst uses two Proxmox VE hosts to run virtual machines and provide a flexible environment for learning enterprise infrastructure.

---

## Host 1

**Device**

HP EliteDesk 800 G4 Mini

### Purpose

Primary virtualization host

### Virtual Machines

| VM | Purpose |
|----|----------|
| Ubuntu Server | Docker, Prometheus, Grafana, cAdvisor |

---

## Host 2

**Device**

HP ProDesk 600 G1 SFF

### Purpose

Secondary virtualization host

### Virtual Machines

| VM | Purpose |
|----|----------|
| Home Assistant | Home automation |
| Windows Server (Active Directory Lab) | Identity and directory services |

---

## Why Proxmox?

- Open-source virtualization platform
- Web-based management
- Supports virtual machines and LXC containers
- Snapshot support
- Backup capabilities
- Excellent for enterprise lab environments

---

## Future Plans

- Automated backups
- Additional Linux VMs
- Additional Windows Server roles
- Shared storage evaluation
- High Availability (HA) lab experiments