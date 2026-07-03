# 🛡 VLAN Plan

## Goal

Segment Project Catalyst into separate networks for management, servers, clients, wireless, IoT, and lab equipment.

## Planned VLANs

| VLAN ID | Name | Purpose | Example Devices |
|---:|---|---|---|
| 10 | Management | Infrastructure management | SonicWall, Linksys LGS328PC, Proxmox |
| 20 | Servers | Virtual machines and services | Ubuntu Docker VM, Pi-hole, Grafana |
| 30 | Clients | Personal devices | PC, laptop |
| 40 | Wireless | Mesh Wi-Fi devices | Linksys MX2000 nodes |
| 50 | IoT | Smart home devices | Cameras, smart plugs, sensors |
| 60 | Lab | Cisco lab equipment | Cisco 3560-CX, Cisco ISR1100 |
| 99 | Native | Native VLAN for trunks | Switch trunk ports |

## Trunk Plan

| Port | Connected Device | Mode | VLANs Allowed |
|---|---|---|---|
| TBD | SonicWall Firewall | Trunk | 10,20,30,40,50,60,99 |
| TBD | HP EliteDesk Proxmox | Trunk | 10,20,60 |
| TBD | Cisco 3560-CX | Trunk | 10,60,99 |
| TBD | Linksys MX2000 | Access/Trunk TBD | 30,40 |

## Notes

- VLANs will be created on the Linksys LGS328PC.
- Inter-VLAN routing will be handled by the SonicWall firewall.
- Firewall rules will control traffic between VLANs.
- Trunk ports will use 802.1Q tagging.