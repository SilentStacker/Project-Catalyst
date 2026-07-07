# 🖥 Hardware Inventory

## Network Edge

| Device | Role | Location | IP Address |
|---|---|---|---|
| ARRIS Gateway | ISP Router / Main Home Router | Living Room | TBD |
| SonicWall Firewall | Project Catalyst Gateway / Firewall | Rack | 192.168.168.168 |

## Switching

| Device | Role | Location | IP Address |
|---|---|---|---|
| Linksys LGS328PC | Core Managed PoE Switch / VLANs / Trunks | Rack | TBD |
| Cisco Catalyst 3560-CX | Cisco Lab Switch | Rack | TBD |

## Wireless

| Device | Role | Location | IP Address |
|---|---|---|---|
| Linksys MX2000 #1 | Mesh Wi-Fi Node | My Room | TBD |
| Linksys MX2000 #2 | Mesh Wi-Fi Node | Mother's Room | TBD |

## Servers & Compute

| Device | Role | Location | IP Address |
|---|---|---|---|
| HP EliteDesk 800 G4 Mini | Proxmox VE Host | Rack | 192.168.168.30 |
| HP ProDesk 600 G1 SFF | Second Proxmox VE Host / Home Assistant / Active Directory Lab | Rack | 192.168.168.20 |
| Ubuntu Server VM | Docker / Monitoring Stack | Proxmox | 192.168.168.144 |
| Raspberry Pi 5 #1 | Monitoring Node | Rack | 192.168.168.200 |
| Raspberry Pi 5 #2 | Monitoring Node | Rack | 192.168.168.201 |


## Power

| Device | Role | Location | IP Address |
|---|---|---|---|
| EMB Smart PDU | Rack Power Distribution | Rack | TBD |

## Planned Additions

- Wazuh SIEM
- VLAN segmentation
- Trunk ports
- Firewall rule documentation
- Network diagrams
- Automation scripts