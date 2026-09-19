# My Homelab (Self-Hosted Server)

This repository documents everything running in my homelab. I built this server (over my family's existing Wi-Fi) to practice infrastructure management, networking, and service deployment. It's built on a single Proxmox node handling infrastructure, security, monitoring, and self-hosted apps, with everything accessed remotely over Tailscale.

I chose Proxmox (Type-1 hypervisor) over a Type-2 setup for better resource efficiency and closer-to-bare-metal control. (Plus, it looks cooler 🎉) This is a work in progress as I'm still updating, adding services, and expanding it.

## 📍 Navigation
- [Apps](./Apps) — General tools and services for managing the homelab.
- [Media](./Media) — Self-hosted entertainment and streaming services.
- [Monitoring](./Monitoring) — Uptime tracking and alerting for the lab.
- [Network](./Network) — DNS, VPN, and remote access setup.

## 🖥️ Server Hardware
|          |  Hardware  |
|:--------:|:--------:|
| PC       | OptiPlex 7010 SFF - $40 |
| Role     | Main Server Computer |
| OS       | Proxmox  |
| CPU      | Intel Core i5-3550 |
| RAM      | 8GB DDR3 |
| Storage  | Samsung 2TB SSD, Seagate 1TB HDD |

## 🪢 Networking
There's no dedicated networking hardware beyond a basic 5-port switch connecting my server to my family's existing internet. From there, all my devices connect to the server through Tailscale, creating a secure private network without needing any additional routers, VLANs, or enterprise gear.

## 🎥 Security
Security-wise, this is still early. Tailscale is currently the only layer protecting the homelab, handling both encrypted access and keeping services off the open LAN. I haven't yet implemented additional measures like a reverse proxy with SSL, firewall rules, or fail2ban, but they're on the list as the project matures.
