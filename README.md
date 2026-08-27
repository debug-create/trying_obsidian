# 🛡️ OBSIDIAN — Autonomous Cyber-Defense & Threat Deception Platform

[![Build Status](https://img.shields.io/badge/build-passing-3EE7C6.svg?style=flat-square)](https://github.com/debug-create/obsidian)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.8-blue.svg?style=flat-square)](https://www.typescriptlang.org/)
[![React](https://img.shields.io/badge/React-19-61dafb.svg?style=flat-square)](https://react.dev/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-v4-38bdf8.svg?style=flat-square)](https://tailwindcss.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg?style=flat-square)](LICENSE)

> **OBSIDIAN** is a next-generation autonomous Security Operations Center (SOC) and cyber-deception engine. It combines real-time identity anomaly detection, interactive threat geospatial intelligence, synthetic honeynet entrapment, and an immutable cryptographic evidence ledger.

---

## 📑 Table of Contents

- [Architectural Overview](#-architectural-overview)
- [Key Capabilities & Modules](#-key-capabilities--modules)
  - [1. Threat Radar & Global Vector Matrix](#1-threat-radar--global-vector-matrix)
  - [2. Organization Identity Sentinel (18 Vectors)](#2-organization-identity-sentinel-18-vectors)
  - [3. Multi-Phase Cyber Kill Chain Simulation](#3-multi-phase-cyber-kill-chain-simulation)
  - [4. Synthetic Deception Honeynet & Decoy Engine](#4-synthetic-deception-honeynet--decoy-engine)
  - [5. Cryptographic Audit Ledger (SHA-256)](#5-cryptographic-audit-ledger-sha-256)
  - [6. Acoustic Breach Alerting (Web Audio API)](#6-acoustic-breach-alerting-web-audio-api)
- [Tech Stack & Dependencies](#-tech-stack--dependencies)
- [Project File Structure](#-project-file-structure)
- [Getting Started & Local Development](#-getting-started--local-development)
- [Production Deployment Guide](#-production-deployment-guide)
  - [Deploy to Vercel / Netlify](#option-a-deploy-to-vercel--netlify)
  - [Deploy with Docker / Cloud Run](#option-b-docker--container-deployment)
  - [Deploy to GitHub Pages](#option-c-github-pages)
- [Context Handover Guide for LLMs & AI Agents](#-context-handover-guide-for-llms--ai-agents)
- [Roadmap & High-Impact Feature Suggestions](#-roadmap--high-impact-feature-suggestions)

---

## 🏛️ Architectural Overview

OBSIDIAN is built around **autonomous containment and active deception**: rather than merely alerting human analysts to intrusions, the platform dynamically reconfigures zero-trust boundaries, routes compromised tokens to high-fidelity containerized decoys, and records forensic evidence with cryptographic nonces.

```
┌────────────────────────────────────────────────────────────────────────┐
│                        OBSIDIAN CORE PLATFORM                          │
└──────┬──────────────────────┬───────────────────────────┬──────────────┘
       │                      │                           │
┌──────▼────────┐      ┌──────▼─────────────┐      ┌──────▼─────────────┐
│ Threat Radar  │      │  Identity Matrix   │      │ Deception Honeynet │
│ • Vector Map  │      │ • 18 Synthetic Emps│      │ • Decoy DB Clones  │
│ • Country ASN │      │ • OAuth Anomaly    │      │ • Canary API Keys  │
│ • Beams/Filters      │ • Instant Breach   │      │ • Attacker Mirror  │
└──────┬────────┘      └──────┬─────────────┘      └──────┬─────────────┘
       │                      │                           │
       └──────────────────────┼───────────────────────────┘
                              │
               ┌──────────────▼──────────────┐
               │ Cryptographic Audit Ledger  │
               │ • SHA-256 Block Chaining    │
               │ • Forensic Nonce & Hashes   │
               │ • JSON Telemetry Export     │
               └─────────────────────────────┘
```

---

## ⚡ Key Capabilities & Modules

### 1. Threat Radar & Global Vector Matrix
- **Geospatial Vector Visualization**: High-contrast, dark-mode SVG map projection with pulsating attack origins, target headquarters, and parabolic attack beams.
- **Interactive Multi-Filter Controls**:
  - **Threat Category Filter**: `Malware`, `Phishing`, `DDoS`, `Brute Force`, `Ransomware`, `Zero-Day`, `Credential Stuffing`, `Port Probe`, `API Fuzzing`.
  - **Origin Country Dropdown**: Live parsing of active threat origins (e.g. Romania, Russia, China, Brazil, Germany, Japan, Singapore, etc.).
  - **Severity Multi-Select**: Toggleable severity filters (`CRITICAL`, `HIGH`, `ELEVATED`, `MEDIUM`) with cyber glow indicators.
  - **Real-Time Forensic Search**: Filters by IP, ASN, adversary handle, or target asset.
  - **Attack Beam Visualizer**: Toggleable dynamic attack vectors (`BEAMS: ON/OFF`).
  - **Dynamic Threat Counter**: Live aggregate calculations that update responsively based on filter state.

### 2. Organization Identity Sentinel (18 Vectors)
- **Real-Time Monitoring**: Tracks 18 employee identities across Engineering, Security, DevOps, Finance, Legal, HR, and Product.
- **Profile Visualization**: High-resolution circular photo avatars with status rings indicating health:
  - 🟢 `NOMINAL`: Normal baseline activity.
  - 🟡 `ELEVATED`: Suspicious OAuth token request or unusual geolocation.
  - 🔴 `BREACHED`: Active credential theft or session hijack with pulsing ring and sound alert.
  - 🟣 `ISOLATED`: Token invalidated and redirected to synthetic digital twin.
- **Instant Adversary Emulation**: One-click **"EMULATE ADVERSARY BREACH"** trigger to test SOC response workflows.
- **Detailed Forensic Inspector**: Click any identity to open an inspection HUD displaying active tokens, risk telemetry, device fingerprints, and remediation actions.

### 3. Multi-Phase Cyber Kill Chain Simulation
An interactive 5-stage automated attack and response pipeline:
1. **Phase 0: Nominal Baseline** — Continuous zero-trust geo-fencing.
2. **Phase 1: Weaponized Spear-Phishing** — Rogue OAuth token exchange from an unapproved ASN.
3. **Phase 2: Privilege Escalation** — Attacker attempts IAM role assumption to access production clusters.
4. **Phase 3: Digital Twin & Decoy Redirection** — Autonomous honeynet swap; attacker is isolated without their knowledge.
5. **Phase 4: Containment & Ledger Verification** — Root token revocation, forensic memory dump, and immutable block creation.

### 4. Synthetic Deception Honeynet & Decoy Engine
- **Decoy Database & Canaries**: Spawns isolated PostgreSQL/Redis clones seeded with realistic fake financial & user records.
- **Telemetry Trapping**: Captures adversary SQL payloads, exfiltration queries, and command keystrokes in real time.

### 5. Cryptographic Audit Ledger (SHA-256)
- **Immutable Block Hashing**: Every defense event, token invalidation, and containment step is sealed with a cryptographic hash and nonce.
- **Forensic Export**: One-click JSON export of the entire blockchain-backed audit trail for compliance and legal review.

### 6. Acoustic Breach Alerting (Web Audio API)
- **Zero-Dependency Sound Synthesizer**: Native browser Web Audio API generating a dual-harmonic metallic chime (`1760Hz` A6 note with `3520Hz` shimmering harmonics).
- **Audio Control HUD**: Mute/unmute toggle and instant audio test button.

---

## 🛠️ Tech Stack & Dependencies

| Layer | Technology | Purpose |
| :--- | :--- | :--- |
| **Framework** | **React 19** + **TypeScript 5.8** | Component architecture and type-safe state management |
| **Build Tool** | **Vite 6** | Lightning-fast development & production tree-shaken bundling |
| **Styling** | **Tailwind CSS v4** | Dark cyberpunk utility design system (`#060A0E`, `#0C131A`, `#3EE7C6`, `#FF3B5C`) |
| **Animations** | **Motion (`framer-motion`)** | Smooth UI transitions, radar sweeps, and modal animations |
| **Icons** | **Lucide React** | Clean, minimalist SVG iconography |
| **Sound** | **Web Audio API** | Native procedural audio synthesis without external MP3 assets |
| **AI Integration** | **`@google/genai`** | Ready for Gemini 2.5/3.7 threat analysis and playbook generation |

---

## 📂 Project File Structure

```text
├── index.html                   # HTML entry point with cyberpunk fonts
├── metadata.json                # AI Studio application configuration
├── package.json                 # Dependency manifests and scripts
├── vite.config.ts               # Vite configuration with Tailwind plugin
├── tsconfig.json                # TypeScript compiler configuration
├── src/
│   ├── main.tsx                 # Application mounting entry point
│   ├── App.tsx                  # Root state router (Landing vs. Dashboard)
│   ├── index.css                # Tailwind CSS imports and custom glow rules
│   ├── types.ts                 # Shared TypeScript interfaces & types
│   ├── utils/
│   │   └── audio.ts             # Web Audio API alert synthesizer & sound engine
│   ├── data/
│   │   └── mockData.ts          # Simulation scenarios, 18 employees, threat vectors & ledger
│   └── components/
│       ├── BootSequence.tsx     # Terminal initialization animation
│       ├── Dashboard.tsx        # Main SOC telemetry cockpit & scenario runner
│       ├── EmployeeDetailModal.tsx # Forensic identity inspector dialog
│       ├── Hero.tsx             # Cyberpunk hero section & interactive particle canvas
│       ├── LandingPage.tsx      # Comprehensive landing view with architecture & live demo preview
│       ├── RiskGauge.tsx        # SVG circular risk score metric with dynamic gradients
│       └── ThreatMap.tsx        # High-density interactive threat radar & country/vector filters
```

---

## 🚀 Getting Started & Local Development

### Prerequisites
- **Node.js**: v18.0.0 or later
- **npm** or **bun** / **pnpm** / **yarn**

### Quick Start

1. **Clone the repository:**
   ```bash
   git clone https://github.com/debug-create/obsidian.git
   cd obsidian
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Start the development server:**
   ```bash
   npm run dev
   ```
   Open [http://localhost:3000](http://localhost:3000) in your browser.

4. **Verify TypeScript & Linting:**
   ```bash
   npm run lint
   ```

5. **Build for Production:**
   ```bash
   npm run build
   ```
   The compiled assets will be output to the `dist/` directory.

---

## 🌐 Production Deployment Guide

### Option A: Deploy to Vercel / Netlify
OBSIDIAN is a pure client-side SPA (React + Vite) and can be deployed with zero backend configuration:

1. Push this repository to GitHub (`https://github.com/debug-create/obsidian`).
2. Import the repository in [Vercel](https://vercel.com) or [Netlify](https://netlify.com).
3. Set the build settings:
   - **Framework Preset**: `Vite`
   - **Build Command**: `npm run build`
   - **Output Directory**: `dist`
4. Click **Deploy**.

### Option B: Docker / Container Deployment (Cloud Run / AWS ECS)

Create a `Dockerfile` in the root:

```dockerfile
# Build Stage
FROM node:20-alpine AS build
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
RUN npm run build

# Production Stage (Nginx)
FROM nginx:alpine
COPY --from=build /app/dist /usr/share/nginx/html
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
```

Build and run:
```bash
docker build -t obsidian-soc .
docker run -p 3000:80 obsidian-soc
```

### Option C: GitHub Pages
In `vite.config.ts`, set `base: '/obsidian/'` if deploying to `username.github.io/obsidian`, then push `dist/` to your `gh-pages` branch.

---

## 🤖 Context Handover Guide for LLMs & AI Agents

If you are an **LLM (Claude, GPT-4o, Gemini, Cursor AI, Windsurf)** taking over this repository:

1. **Design System & Palette**:
   - Canvas: `#060A0E` (Deep Cyber Void)
   - Containers/Cards: `#0C131A` (Obsidian Gray), `#111A23` (Dark Slate)
   - Primary Cyber Accent: `#3EE7C6` (Neon Cyan)
   - Alert / Breach Accent: `#FF3B5C` (Laser Red)
   - Warning Accent: `#FFB84D` (Amber)
   - Deception / Isolation Accent: `#B48CFF` (Electric Violet)
   - Typography: Monospace telemetry font (`font-mono`) paired with bold modern display headings (`font-display`).
2. **State Hierarchy**:
   - `App.tsx` controls view switching (`landing` vs `dashboard`).
   - `Dashboard.tsx` manages simulation playback (`currentStageIndex`, `isSimulating`, `streamedLogs`, `employees`).
   - `audio.ts` manages Web Audio context (`playBreachAlertTing()`, `playCyberClick()`).
   - `ThreatMap.tsx` manages map markers, beams, category/country/severity filters, and inspection HUDs.
3. **Sound System**:
   - Uses Web Audio API without audio files. Avoid introducing heavy `.mp3` assets unless requested.
4. **Data Contract**:
   - `src/types.ts` is the single source of truth for `Employee`, `ThreatVector`, `ScenarioStage`, and `LedgerBlock`. Always update `types.ts` before modifying state interfaces.

---

## 💡 Roadmap & High-Impact Feature Suggestions

Here are 8 powerful features you can implement next to elevate OBSIDIAN to an enterprise-grade cyber-deception suite:

### 1. 🧠 Autonomous Gemini Incident Commander & LLM Playbook Generator
- Integrate Google Gemini (`@google/genai`) to generate live **MITRE ATT&CK mitigation playbooks** in real time as attacks unfold.
- Analysts can ask natural language questions (e.g. *"What is the threat actor's exfiltration vector?"*) and receive instant forensic summaries.

### 2. 🪤 Interactive Deception Sandbox Terminal (Live Honeypot TTY)
- Add an interactive web-based terminal simulating a decoy Linux server.
- Watch simulated attackers execute bash commands in real time while logging their IP, keystrokes, and payload signatures.

### 3. 🗺️ 3D Three.js / WebGL Threat Globe
- Upgrade the 2D world map to an interactive 3D WebGL globe with dynamic rotating arcs, atmospheric glow, and particle clouds representing global attack traffic.

### 4. 🔗 SIEM / Webhook Integrations
- Enable real webhook dispatching (Slack, Discord, PagerDuty, Splunk, Datadog) whenever a breach occurs.

### 5. 🛡️ Custom Policy & Rule Builder
- Visual drag-and-drop Zero-Trust rule creator (e.g. *"If employee risk > 70 AND origin != HQ Geolocation, redirect to Decoy Database"*).

### 6. 📊 MITRE ATT&CK Matrix Heatmap View
- Interactive matrix mapping detected attack techniques against the official MITRE ATT&CK framework with active technique highlights.

### 7. 👥 Multi-Tenant Organization Switcher
- Switch between multiple corporate workspaces or cloud providers (AWS, GCP, Azure, Kubernetes clusters) to inspect multi-cloud security posture.

### 8. 📜 PDF Incident Report Generator
- Export a branded forensic incident report with executive summaries, blockchain proof certificates, and timestamped forensic logs ready for compliance audit.

---

## 📄 License
This project is open-source and available under the [MIT License](LICENSE).
