---
title: Proxmox Ve
description: 
published: true
date: 2026-04-08T06:55:34.719Z
tags: 
editor: markdown
dateCreated: 2026-03-25T05:19:51.848Z
---

<!--- Intro --->

# Proxmox
<div style="text-align: center; margin-top: 20px;">

  <img src="https://cdn.jsdelivr.net/gh/selfhst/icons@main/png/proxmox.png" style="width:500px; height:500px; margin-bottom: 10px;">
</div>

Proxmox VE is a **free and open-source hypervisor** that allows you to run and manage virtualized workloads on a single system.

It is built on **Debian Linux** and combines multiple technologies into one platform:

- **KVM (Kernel-based Virtual Machine)** for full virtual machines  
- **LXC (Linux Containers)** for lightweight containers  
- Built-in tools for **storage, networking, and backups**  

Most services in this environment are running inside **LXC containers**, while some applications run inside **Docker containers** within those LXCs.

---

<div style="text-align: center; margin-top: 20px;">

## KVM vs LXC (Quick Breakdown)

</div>

- **KVM (Virtual Machines)** = full-on separate computers  
  - Runs its own OS (Windows, Linux, etc.)  
  - More powerful, but heavier on resources  

- **LXC (Containers)** = shared house, separate rooms  
  - Uses the host’s Linux kernel  
  - Way lighter, faster, and perfect for most apps  

👉 Use **KVM** when you need a full OS  
👉 Use **LXC** for most services  

---

<div style="text-align: center; margin-top: 20px;">

## Proxmox Helper Scripts

</div>

Many of the services here were deployed using **Proxmox Helper Scripts**.

These are community-created scripts that automate:

- Creating LXC containers  
- Installing applications  
- Configuring Docker  
- Setting up dependencies  

Project:  <a href="https://community-scripts.org/scripts" target="_blank">https://community-scripts.org/scripts</a>

> ⚠️ These scripts are **community maintained**, not official Proxmox tools.  
> Always review scripts before running them.

---

Proxmox is commonly used in **homelabs and enterprise environments** to consolidate hardware and run multiple services on one machine through an easy-to-use **web interface**.

---


<!--- Links --->

<div style="text-align: center; margin-top: 30px; margin-bottom:30px;">
  
# Installations

</div>

<div style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">

  
  <div style="border: 1px solid #ccc; border-radius: 8px; padding: 15px; width: 160px; min-height: 160px; box-shadow: 0px 4px 6px rgba(0,0,0,0.1); display: flex; flex-direction: column; align-items: center; justify-content: center; text-align:center;">
  <a href="/proxmox/proxmox" style="text-decoration: none; color: inherit; display: flex; flex-direction: column; align-items: center; justify-content: center;">
    <img src="https://cdn.jsdelivr.net/gh/selfhst/icons@main/png/proxmox.png" style="width:100px; height:100px; margin-bottom: 10px;" alt="Docker & Portainer">
    <h4 style="margin: 0;">Installation</h4>
  </a>

</div>

  <div style="border: 1px solid #ccc; border-radius: 8px; padding: 15px; width: 160px; min-height: 160px; box-shadow: 0px 4px 6px rgba(0,0,0,0.1); display: flex; flex-direction: column; align-items: center; justify-content: center; text-align:center;">
  <a href="/proxmox/docker_and_portainer" style="text-decoration: none; color: inherit; display: flex; flex-direction: column; align-items: center; justify-content: center;">
    <img src="https://cdn.jsdelivr.net/gh/selfhst/icons@main/png/docker.png" style="width:100px; height:100px; margin-bottom: 10px;" alt="Docker & Portainer">
    <h4 style="margin: 0;">Docker & Portainer</h4>
  </a>

</div>
  
  
</div>
---



<div style="text-align: center; margin-top: 30px; margin-bottom:30px;">

# Storage & Backup

</div>

<div style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">

<div style="border: 1px solid #ccc; border-radius: 8px; padding: 15px; width: 160px; min-height: 160px; box-shadow: 0px 4px 6px rgba(0,0,0,0.1); display: flex; flex-direction: column; align-items: center; justify-content: center; text-align:center;">
  <a href="/truenas/PBS" style="text-decoration: none; color: inherit; display: flex; flex-direction: column; align-items: center; justify-content: center;">
    <img src="https://cdn.jsdelivr.net/gh/selfhst/icons@main/png/proxmox.png" style="width:100px; height:100px; margin-bottom: 10px;" alt="Proxmox Backup Storage">
    <h4 style="margin: 0;">Proxmox Backup Storage</h4>
  </a>

</div>

</div>
---

<div style="text-align: center; margin-top: 30px;">

# Services

</div>

<div style="text-align: center; margin-top: 10px; margin-bottom: 30px;">

## Networking

</div>

<div style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">

  

<div style="border: 1px solid #ccc; border-radius: 8px; padding: 15px; width: 160px; min-height: 160px; box-shadow: 0px 4px 6px rgba(0,0,0,0.1); display: flex; flex-direction: column; align-items: center; justify-content: center; text-align:center;">
  <a href="/proxmox/my-speed" style="text-decoration: none; color: inherit; display: flex; flex-direction: column; align-items: center; justify-content: center;">
    <img src="https://cdn.jsdelivr.net/gh/selfhst/icons@main/png/myspeed.png" style="width:100px; height:100px; margin-bottom: 10px;" alt="My Speed">
    <h4 style="margin: 0;">My Speed</h4>
  </a>
  
</div> 

<div style="border: 1px solid #ccc; border-radius: 8px; padding: 15px; width: 160px; min-height: 160px; box-shadow: 0px 4px 6px rgba(0,0,0,0.1); display: flex; flex-direction: column; align-items: center; justify-content: center; text-align:center;">
  <a href="/proxmox/Network_Optimizer" style="text-decoration: none; color: inherit; display: flex; flex-direction: column; align-items: center; justify-content: center;">
    <img src="https://github.com/Ozark-Connect/NetworkOptimizer/blob/main/docs/images/app-logo-v2.png?raw=true" style="width:100px; height:100px; margin-bottom: 10px;" alt="Network Optimizer">
    <h4 style="margin: 0;">Network Optimizer</h4>
  </a>
  
</div>  

  
  <div style="border: 1px solid #ccc; border-radius: 8px; padding: 15px; width: 160px; min-height: 160px; box-shadow: 0px 4px 6px rgba(0,0,0,0.1); display: flex; flex-direction: column; align-items: center; justify-content: center; text-align:center;">
  <a href="/proxmox/immich" style="text-decoration: none; color: inherit; display: flex; flex-direction: column; align-items: center; justify-content: center;">
    <img src="https://cdn.jsdelivr.net/gh/selfhst/icons@main/png/nginx-proxy-manager.png" style="width:100px; height:100px; margin-bottom: 10px;" alt="Nginx Proxy Manager">
    <h4 style="margin: 0;">Nginx Proxy Manager</h4>
  </a>
  
</div>

</div>


<div style="text-align: center; margin-top: 10px; margin-bottom:30px;">

## Security & Monitoring

</div>

<div style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">

  <div style="position: relative; border: 1px solid #ccc; border-radius: 8px; padding: 15px; width: 160px; min-height: 100px; text-align:center; box-shadow: 0px 4px 6px rgba(0,0,0,0.1);">
    <a href="/proxmox/vaultwarden" style="position:absolute; top:0; left:0; width:100%; height:100%;"></a>
    <img src="https://cdn.jsdelivr.net/gh/selfhst/icons@main/png/vaultwarden.png" style="width:100px; height:100px; margin-bottom: 10px; align:center;" alt="Vaultwarden">
    <h4>Vaultwarden</h4>
  </div>

  <div style="position: relative; border: 1px solid #ccc; border-radius: 8px; padding: 15px; width: 160px; min-height: 100px; text-align:center; box-shadow: 0px 4px 6px rgba(0,0,0,0.1);">
    <a href="/proxmox/cloudflared" style="position:absolute; top:0; left:0; width:100%; height:100%;"></a>
    <img src="https://cdn.jsdelivr.net/gh/selfhst/icons@main/png/cloudflare-zero-trust.png" style="width:100px; height:100px; margin-bottom: 10px; align:center;" alt="Cloudflared">
    <h4>Cloudflared</h4>
  </div>

  <div style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">

  <div style="position: relative; border: 1px solid #ccc; border-radius: 8px; padding: 15px; width: 160px; min-height: 100px; text-align:center; box-shadow: 0px 4px 6px rgba(0,0,0,0.1);">
    <a href="/proxmox/uptimekuma" style="position:absolute; top:0; left:0; width:100%; height:100%;"></a>
    <img src="https://cdn.jsdelivr.net/gh/selfhst/icons@main/png/uptime-kuma.png" style="width:100px; height:100px; margin-bottom: 10px; align:center;" alt="Uptime Kuma">
    <h4>Uptime Kuma</h4>
  </div>
</div>

</div>


<div style="text-align: center; margin-top: 10px; margin-bottom:30px;">

## Media / arr stack

</div>

<div style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">

  <div style="position: relative; border: 1px solid #ccc; border-radius: 8px; padding: 15px; width: 160px; min-height: 100px; text-align:center; box-shadow: 0px 4px 6px rgba(0,0,0,0.1); align:center;">
    <a href="/proxmox/immich" style="position:absolute; top:0; left:0; width:100%; height:100%;"></a>
    <img src="https://cdn.jsdelivr.net/gh/selfhst/icons@main/png/immich.png" style="width:100px; height:100px; margin-bottom: 10px; align:center;" alt="Immich">
    <h4>Immich</h4>
  </div>
  
  

  <div style="position: relative; border: 1px solid #ccc; border-radius: 8px; padding: 15px; width: 160px; min-height: 100px; text-align:center; box-shadow: 0px 4px 6px rgba(0,0,0,0.1);">
    <h4>Qbittorrent</h4>
  </div>

  <div style="position: relative; border: 1px solid #ccc; border-radius: 8px; padding: 15px; width: 160px; min-height: 100px; text-align:center; box-shadow: 0px 4px 6px rgba(0,0,0,0.1);">
    <h4>Prowlarr</h4>
  </div>

</div>


---

<div style="text-align: center; margin-top: 30px; margin-bottom:30px;">

## Other

</div>

<div style="display: flex; gap: 20px; flex-wrap: wrap; justify-content: center;">

  <div style="position: relative; border: 1px solid #ccc; border-radius: 8px; padding: 15px; width: 160px; min-height: 100px; text-align:center; box-shadow: 0px 4px 6px rgba(0,0,0,0.1);">
    <a href="/proxmox/mealie" style="position:absolute; top:0; left:0; width:100%; height:100%;"></a>
    <img src="https://cdn.jsdelivr.net/gh/selfhst/icons@main/png/mealie.png" style="width:100px; height:100px; margin-bottom: 10px; align:center;" alt="Mealie">
    <h4>Mealie</h4>
  </div>

  <div style="position: relative; border: 1px solid #ccc; border-radius: 8px; padding: 15px; width: 160px; min-height: 100px; text-align:center; box-shadow: 0px 4px 6px rgba(0,0,0,0.1);">
    <a href="/proxmox/reactive_resume" style="position:absolute; top:0; left:0; width:100%; height:100%;"></a>
    <img src="https://cdn.jsdelivr.net/gh/selfhst/icons@main/png/reactive-resume.png" style="width:100px; height:100px; margin-bottom: 10px; align:center;" alt="Reactive Resume">
    <h4>Reactive Resume</h4>
  </div>
  
  <div style="border: 1px solid #ccc; border-radius: 8px; padding: 15px; width: 160px; min-height: 160px; box-shadow: 0px 4px 6px rgba(0,0,0,0.1); display: flex; flex-direction: column; align-items: center; justify-content: center; text-align:center;">
  <a href="/proxmox/wikijs" style="text-decoration: none; color: inherit; display: flex; flex-direction: column; align-items: center; justify-content: center;">
    <img src="https://cdn.jsdelivr.net/gh/selfhst/icons@main/png/wiki-js.png" style="width:100px; height:100px; margin-bottom: 10px;" alt="Wiki.JS">
    <h4 style="margin: 0;">Wiki.JS</h4>
  </a>

</div>

</div>