# 🌐 IP Addressing

## Primary LAN

**Subnet:** `192.168.168.0/24`  
**Gateway:** `192.168.168.168`  
**Gateway Device:** SonicWall Firewall

| Device | Role | IP Address |
|---|---|---|
| SonicWall Firewall | Project Catalyst Gateway | 192.168.168.168 |
| HP EliteDesk 800 G4 Mini | Proxmox VE Host | 192.168.168.30 |
| Ubuntu Server VM | Docker / Monitoring Stack | 192.168.168.144 |
| Raspberry Pi 5 #1 | Monitoring Node | 192.168.168.200 |
| Raspberry Pi 5 #2 | Monitoring Node | 192.168.168.201 |

## Services

| Service | Host | Port |
|---|---|---:|
| Grafana | Ubuntu Server VM | 3000 |
| Prometheus | Ubuntu Server VM | 9090 |
| Node Exporter | Ubuntu Server VM / Pis / Proxmox | 9100 |
| cAdvisor | Ubuntu Server VM | 8080 |
| Pi-hole | TBD | 53 |