<h1 align="center">🔒 Pludix</h1>
<h3 align="center">Private, Invite-Only Real-Time Communication Platform</h3>

<p align="center">
  A Discord-style app for small, close-knit communities — built from scratch as a
  full-stack + real-time systems project.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/status-private_beta-blue?style=flat-square" />
  <img src="https://img.shields.io/badge/type-portfolio_showcase-lightgrey?style=flat-square" />
</p>

---

> **Note:** This repository is for portfolio/demonstration purposes only.
> Source code is proprietary and not licensed for reuse or distribution.

---

### 💡 What it is

Pludix is a voice/video/text communication platform designed for small groups who want
a private, self-hosted alternative to mainstream chat apps — with a focus on a premium,
minimal aesthetic (**"Vercel × Apple × near-future"**) rather than a generic clone.

---

### 🛠️ Tech Stack

**Backend**
![NestJS](https://img.shields.io/badge/-NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![Fastify](https://img.shields.io/badge/-Fastify-000000?style=flat-square&logo=fastify&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Prisma](https://img.shields.io/badge/-Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)

**Frontend**
![React](https://img.shields.io/badge/-React%2019-61DAFB?style=flat-square&logo=react&logoColor=black)
![Vite](https://img.shields.io/badge/-Vite-646CFF?style=flat-square&logo=vite&logoColor=white)

**Real-Time**
![WebRTC](https://img.shields.io/badge/-WebRTC-333333?style=flat-square&logo=webrtc&logoColor=white)
![LiveKit](https://img.shields.io/badge/-LiveKit-FF3B30?style=flat-square)

**Desktop**
![Tauri](https://img.shields.io/badge/-Tauri-FFC131?style=flat-square&logo=tauri&logoColor=black)

---

### 🏗️ Architecture Highlights

- **One frontend, two platforms** — a single React codebase serves both the web app
  and the Tauri desktop shell. No duplicated UI logic between web and desktop.
- **Self-hosted real-time layer** — LiveKit deployed independently, giving full control
  over media infrastructure instead of depending on a third-party WebRTC SaaS.
- **Deliberate codec choices** — VP9 over AV1 (CPU budget constraints), Opus with DTX
  and noise suppression tuned for the target hardware profile.
- **Decoupled admin surface** — a separate authenticated management panel with its own
  login flow and env-seeded first-admin bootstrap, fully independent from the main
  app's auth system.

---

### 📌 Status

Actively developed, currently running as a private beta for a closed group of users.

<p align="center">
  <sub>Built solo · NestJS · React · PostgreSQL · LiveKit · Tauri</sub>
</p>
