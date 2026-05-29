# SecureConnect-IPsec-VPN
# SecureConnect: Enterprise Site-to-Site IPsec VPN Deployment

A secure network infrastructure simulation demonstrating the deployment of a Site-to-Site IPsec VPN using Cisco Packet Tracer. This project ensures confidential data transmission between a Headquarters (HQ) and a Remote Branch over an insecure public internet (ISP).

## 🌐 Network Topology
- **HQ LAN:** 192.168.10.0/24 (Protected)
- **Branch LAN:** 192.168.20.0/24 (Protected)
- **Public WAN Subnets:** 200.1.1.0/24 & 200.2.2.0/24
- **Core Devices:** Cisco ISR 4321 Routers, Catalyst 2960 Switches.

## 🔒 Security Implementations & Features
- **Phase 1 (ISAKMP Policy):** AES Encryption, SHA Hash, Diffie-Hellman Group 2, and Pre-Shared Key (PSK) Authentication.
- **Phase 2 (IPsec Transform Set):** Encapsulating Security Payload (ESP) with AES encryption and SHA-HMAC for data integrity.
- **Interesting Traffic Definition:** Crypto Access Control Lists (ACLs) to isolate and encrypt strictly corporate traffic.
- **Routing:** Default Static Routing configured towards the ISP.

## 🧪 Verification & Results
- Successfully established end-to-end communication via encrypted tunnels.
- Verified traffic encapsulation using `show crypto ipsec sa` and checked crypto status via `show crypto isakmp sa` (Status: `QM_IDLE / ACTIVE`).

- <img width="1919" height="1010" alt="image" src="https://github.com/user-attachments/assets/67d8accc-765e-45a6-b30d-9fcde75a0bd8" />
<img width="975" height="275" alt="image" src="https://github.com/user-attachments/assets/2f33cfb0-bafe-401e-b63e-c8c3f3d8eadf" />
<img width="975" height="544" alt="image" src="https://github.com/user-attachments/assets/5cd4fd4f-2b45-44f7-ad84-a10b0ce9abb5" />
<img width="975" height="909" alt="image" src="https://github.com/user-attachments/assets/ff6ad3bc-802c-4da8-a7d8-b8c5dbc72a3c" />



