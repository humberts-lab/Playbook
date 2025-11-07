1. Data Link Layer
2. First usable host: 192.168.50.1, Last usable host: 192.168.50.62, Broadcast address: 192.168.50.63
3. Show VLAN brief: Checks whether VLAN 20 exists, is active, and which ports are assigned to it. show interfaces trunk→ Verifies whether trunk links are up and which VLANs are allowed to pass through the trunk.
4. To create a static route from Router A (network 10.10.10.0/24) to reach 172.16.0.0/24, use this Cisco IOS command: ip route 172.16.0.0 255.255.255.0 <next-hop-IP-address>
5. To block all external ICMP echo requests (pings coming from outside to inside), you would configure an access control list (ACL) entry like this:
access-list 100 deny icmp any any echo
Then, to allow other traffic afterward:
access-list 100 permit ip any any
6. Other wireless devices — such as microwave ovens, cordless phones, Bluetooth devices, or baby monitors operating on the 2.4 GHz band. And Overlapping Wi-Fi channels or nearby networks — neighboring access points using the same or overlapping channels can cause co-channel or adjacent-channel interference.
7. White/Orange, Orange, White/Green, Blue, White/Blue, Green, White/Brown, Brown
8. Network Layer
9. SNMP protocol

    | #  | Scenario                                        | Key OSI Layer / Concept   | Verification or Command                        | Expected Result                                                                 |
| -- | ----------------------------------------------- | ------------------------- | ---------------------------------------------- | ------------------------------------------------------------------------------- |
| 1  | Switch forwarding but router not seeing traffic | **Layer 2 – Data Link**   | Check VLAN/trunking                            | Frames forwarded; router sees traffic                                           |
| 2  | Subnet 192.168.50.0/26                          | **Subnetting**            | —                                              | 1st Host: 192.168.50.1<br>Last Host: 192.168.50.62<br>Broadcast: 192.168.50.63  |
| 3  | VLAN 20 PCs can’t communicate                   | **VLAN/Trunking**         | `show vlan brief` / `show interfaces trunk`    | VLAN active, trunk carries VLAN 20                                              |
| 4  | Router A → Router B (Static Route)              | **Layer 3 – Network**     | `ip route 172.16.0.0 255.255.255.0 10.10.10.2` | Route added, connectivity restored                                              |
| 5  | Block external ICMP echoes                      | **ACL Configuration**     | `access-list 100 deny icmp any any echo`       | Blocks inbound pings                                                            |
| 6  | Wi-Fi dropping randomly                         | **Wireless Interference** | —                                              | Check for microwave/Bluetooth overlap                                           |
| 7  | Mis-wired connector                             | **T568B Standard**        | —                                              | 1. W/Orange 2. Orange 3. W/Green 4. Blue 5. W/Blue 6. Green 7. W/Brown 8. Brown |
| 8  | Can ping gateway but not 8.8.8.8                | **Layer 3 – Routing**     | Check routing/NAT                              | Routing beyond LAN failing                                                      |
| 9  | Measure bandwidth & performance                 | **SNMP Monitoring**       | Use SolarWinds/PRTG/Nagios                     | Monitors bandwidth/device load                                                  |
| 10 | Network restored                                | **Verification**          | Ping test                                      | Successful end-to-end connectivity                                              |

<img width="305" height="143" alt="image" src="https://github.com/user-attachments/assets/40867812-7afb-422e-b489-ade73aabc93e" />


Reflection: During this troubleshooting project, I learned how each part of a network connects and communicates across the OSI model. I practiced identifying issues at different layers — from physical wiring and VLAN configuration to routing and ACL filtering. I strengthened my understanding of subnetting, static routing, and how to verify configurations using Cisco commands such as show vlan brief, show interfaces trunk, and ip route. Building and testing the network in Packet Tracer helped me apply these concepts hands-on. Seeing a successful ping confirmed that the devices were communicating correctly, which reinforced the importance of step-by-step verification and documentation. Overall, I gained confidence in diagnosing network problems, configuring routers and switches, and validating network performance — essential skills for any network technician.
