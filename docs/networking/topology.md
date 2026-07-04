# 🗺 Network Topology

## Physical Topology

                         Internet
                             │
                      ARRIS Gateway
                  Living Room ISP Router
                             │
                      Home Network LAN
                             │
                    SonicWall Firewall
                    192.168.168.168
                  Project Catalyst Gateway
                             │
                    Linksys LGS328PC
                  Core Managed PoE Switch
          ┌──────────────────┼──────────────────┐
          │                  │                  │
   HP EliteDesk 800 G4   Raspberry Pi 5s   Cisco Lab Gear
      Proxmox VE          Monitoring       3560-CX / ISR1100
          │
   Ubuntu Server VM
   Docker / Monitoring

   Wireless Mesh
     Linksys MX2000
                My Room
                   ▲
                   │
                Mesh Link
                   │
                   ▼
              Linksys MX2000
              Mother's Room

              
              
              Logical Flow
ARRIS Gateway
    ↓
SonicWall Firewall
    ↓
Linksys LGS328PC
    ↓
VLANs / Trunks / Access Ports
    ↓
Proxmox Hosts, Servers, Clients, Wireless, Lab Devices

Proxmox Hosts
Host	              Device	                             Current Workloads	           IP Address
Proxmox Host 1	HP EliteDesk 800 G4 Mini	Ubuntu Docker VM, Monitoring Stack	     192.168.168.30
Proxmox Host 2	HP ProDesk 600 G1 SFF	Home Assistant, Active Directory Lab    192.168.168.20


Notes 

ARRIS is the main living room ISP router.
SonicWall is the Project Catalyst gateway/firewall.
SonicWall LAN IP: 192.168.168.168
Linksys LGS328PC will handle VLANs and trunk ports.
SonicWall will handle inter-VLAN routing and firewall policies.
HP EliteDesk 800 G4 Mini is the primary Proxmox host.
HP ProDesk 600 G1 SFF is the second Proxmox host.
Cisco 3560-CX and Cisco ISR1100 are used for lab practice.