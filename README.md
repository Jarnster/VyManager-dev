# VyManager

> **Multi-tenant network management platform** to configure, deploy, and monitor VyOS instances across multiple sites.

[![Discord](https://img.shields.io/badge/Discord-Join%20Community-5865F2?style=flat-square&logo=discord)](https://discord.gg/k9SSkK7wPQ)
[![Docs](https://img.shields.io/badge/Docs-VyProjects-0078D4?style=flat-square&logo=gitbook)](https://docs.vyprojects.org/)
[![GitHub stars](https://img.shields.io/github/stars/Community-VyProjects/VyManager?style=flat-square)](https://github.com/Community-VyProjects/VyManager/stargazers)
[![GitHub Container Registry](https://img.shields.io/badge/GitHub%20Container%20Registry-ghcr.io-1f6feb?style=flat-square&logo=github)](https://github.com/Community-VyProjects/VyManager/pkgs/container/vymanager-backend)

[Quick Start](#-quick-start) · [Documentation](https://docs.vyprojects.org/) · [Discord](https://discord.gg/k9SSkK7wPQ)

Give us a ⭐ star to support us❤️

---

## 📖 Table of Contents

- [About VyManager](#-about-vymanager)
- [Features](#-features)
- [Screenshots](#-screenshots)
- [Quick Start](#-quick-start)
- [Installation](#-installation)
  - [Automated Script (Linux)](#automated-script-linux)
  - [Manual Docker Setup](#manual-docker-setup)
- [Configuration](#-configuration)
- [Post‑Installation Setup Wizard](#-postinstallation-setup-wizard)
- [Managing Your Deployment](#-managing-your-deployment)
- [Managing Multiple VyOS Instances](#-managing-multiple-vyos-instances)
- [Version‑Aware Architecture](#-versionaware-architecture)
- [Tech Stack](#-tech-stack)
- [Development / Manual Setup](#-development--manual-setup)
- [AI Integration with VyMCP](#-ai-integration-with-vymcp)
- [Security Considerations](#-security-considerations)
- [Troubleshooting](#-troubleshooting)
- [Contributing](#-contributing)
- [License](#-license)
- [Support](#-support)

---

## 🖼️ Screenshots

*User Interface supports Light, Dark and Custom themes.*  
<img width="3799" height="1849" alt="Screenshot 1" src="https://github.com/user-attachments/assets/898081db-678f-4645-909d-f147baed23e7" />
<img width="3790" height="624" alt="Screenshot 2" src="https://github.com/user-attachments/assets/2bf95cc6-4ca8-4694-9822-d97bb90db1b8" />
<img width="3799" height="1335" alt="Screenshot 3" src="https://github.com/user-attachments/assets/74ccf55e-2839-492f-ad0e-4e9db2df5774" />

---

## 🚀 About VyManager

VyManager is an open‑source, enterprise‑grade control plane for **VyOS** routers. It provides a modern web interface to manage **multiple instances** across different sites, with role‑based access control, live dashboards, and configuration deployment – all from a single pane of glass.

- **Multi‑site** – organise routers into logical sites (e.g., datacenters, branch offices).
- **Version‑aware** – supports VyOS 1.4, 1.5, and rolling releases.
- **Secure** – API‑key authentication, encrypted SSH credentials, and fine‑grained permissions.
- **Extensible** – built with Next.js, FastAPI, and PostgreSQL.

---

## ✨ Features

- **Centralised Management** – add, remove, and configure VyOS instances from one UI.
- **Live Dashboards** – real‑time interface counters, system info, network graphs, and WireGuard peers via GraphQL.
- **Role‑Based Access Control** – OWNER, ADMIN, VIEWER per site.
- **Multi‑Version Support** – automatically adapts features based on the connected VyOS version.
- **Docker‑First Deployment** – runs anywhere with Docker Compose.
- **Light & Dark Themes** – choose what suits you.

---

## ⚡ Quick Start

The fastest way to get VyManager running is with our **automated install script** (Linux only) or the **manual Docker Compose** method.

- **Documentation**: [https://docs.vyprojects.org/](https://docs.vyprojects.org/)
- **Community**: [Discord](https://discord.gg/k9SSkK7wPQ)

---

## 📦 Installation

### Automated Script (Linux)

> [!IMPORTANT]  
> The install script supports **Ubuntu/Debian**, **Fedora**, **CentOS/RHEL**, **Arch Linux**, and **openSUSE**. It automatically installs Docker, Docker Compose, and pulls the VyManager stack.

Run the following command as **root** or a user with `sudo` privileges:

```bash
curl -fsSL https://raw.githubusercontent.com/Community-VyProjects/VyManager/beta/install.sh | bash
