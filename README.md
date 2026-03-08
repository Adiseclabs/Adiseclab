# AdiSecLab — Elite Bug Bounty Intelligence Platform

<div align="center">

![AdiSecLab Banner](https://img.shields.io/badge/AdiSecLab-v5.0.0-00d4ff?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZmlsbD0iIzAwZDRmZiIgZD0iTTEyIDJMMiA3bDEwIDUgMTAtNS0xMC01ek0yIDE3bDEwIDUgMTAtNS0xMC01LTEwIDV6TTIgMTJsMTAgNSAxMC01LTEwLTUtMTAgNXoiLz48L3N2Zz4=)
![Platform](https://img.shields.io/badge/Platform-Web%20%7C%20Offline-7c6aff?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-00e5a0?style=for-the-badge)
![Tools](https://img.shields.io/badge/Tools-35%2B%20Integrated-ff4560?style=for-the-badge)
![Modules](https://img.shields.io/badge/Modules-30%2B%20Attack-ffd60a?style=for-the-badge)

<br/>

**A god-level, single-file bug bounty intelligence platform.**  
Built by [Aditya Bhosale](https://www.linkedin.com/in/bhsoaleaditya/) — Security Researcher · Bug Bounty Hunter · Penetration Tester

[🚀 Launch Tool](#-quick-start) · [📄 Features](#-features) · [🛠 Tools](#️-tool-arsenal) · [📋 Modules](#-scan-modules) · [📬 Contact](#-contact)

</div>

---

## 📸 Preview

```
┌─────────────────────────────────────────────────────────────┐
│  A  AdiSecLab          ⚡ Scanner                            │
│     Bug Bounty         ┌─────────────────────────┐          │
│     Intelligence       │ https://target.com      │ ▶ Launch │
│     Platform           └─────────────────────────┘          │
│                                                              │
│  ⚡ Scanner      🔥 3  ⚠️ 4  ⚡ 3  ℹ️ 2  📊 2              │
│  🔧 Modules 24   ───────────────────────────────            │
│  🎯 Findings 15  00:00:01 [SYS] AdiSecLab v5.0 — ready     │
│  💻 Commands     00:00:03 [INF] Subfinder — subdomain enum  │
│  💣 Payloads     00:00:07 [CRIT] SQL Injection at /api/...  │
│  🛠️  Tools        00:00:09 [OK] 253 subdomains found        │
│  📝 Notebook     00:00:12 ✓ Scan complete. 15 findings      │
│  ⚙️  Config                                                  │
│  👤 About        [ PDF Report ] [ JSON ] [ CSV ] [ Detail ] │
└─────────────────────────────────────────────────────────────┘
```

---

## ✨ Features

| Feature | Description |
|---|---|
| ⚡ **Live Scan Simulation** | Real-time terminal output with 16-step progress tracker |
| 🔧 **30+ Attack Modules** | Toggle individual modules — Critical ones highlighted in red |
| 🎯 **Vulnerability Findings** | Auto-sorted by severity with full descriptions |
| 📄 **PDF Report Export** | Professional report with cover page, per-finding focus, exploit guidance, remediation steps |
| ⬇️ **JSON / CSV Export** | Machine-readable formats for integration with other tools |
| 💣 **Payload Library** | 80+ curated payloads across 7 categories — click to copy instantly |
| 💻 **Command Reference** | 30+ production-ready terminal commands organized by phase |
| 🛠️ **Tool Arsenal** | 35+ open-source tools with descriptions and categories |
| 📝 **Hunter's Notebook** | Session notes for scope, credentials, recon findings, ideas |
| 🔬 **Detail View** | In-depth per-finding analysis with risk score, tool usage guide, and fix steps |
| ⚙️ **Full Configuration** | Threads, timeout, rate limit, depth, proxy, wordlist settings |
| 📊 **Risk Scoring** | Automatic risk score (0–100) calculated from finding severities |

---

## 🚀 Quick Start

### Option 1 — Direct Open (Recommended)
```bash
# Download the file
curl -O https://raw.githubusercontent.com/YOUR_USERNAME/adiseclab/main/AdiSecLab.html

# Open in browser
open AdiSecLab.html          # macOS
xdg-open AdiSecLab.html      # Linux
start AdiSecLab.html         # Windows
```

### Option 2 — Local Dev Server
```bash
# Python 3
python3 -m http.server 5500
# Then open http://localhost:5500/AdiSecLab.html

# Node.js (npx)
npx serve .
```

> **No installation required.** AdiSecLab is a single self-contained HTML file.  
> Works 100% offline — no backend, no dependencies, no npm install.

---

## 📋 Scan Modules

<details>
<summary><b>View all 30+ modules</b></summary>

| Module | Tool | Severity | Default |
|--------|------|----------|---------|
| Subdomain Enum | Subfinder / Amass | — | ✅ ON |
| Live Host Probe | HTTPX | — | ✅ ON |
| Port Scan | Nmap / RustScan | — | ✅ ON |
| Vulnerability Scan | Nuclei | 🔴 CRITICAL | ✅ ON |
| SQL Injection | SQLMap | 🔴 CRITICAL | ✅ ON |
| XSS Hunter | DalFox | 🔴 CRITICAL | ✅ ON |
| LFI / Path Traversal | Custom | 🔴 CRITICAL | ✅ ON |
| SSRF Scanner | SSRFMap | 🔴 CRITICAL | ✅ ON |
| XXE Injector | Custom | 🔴 CRITICAL | ⚫ OFF |
| SSTI Scanner | Custom | 🔴 CRITICAL | ⚫ OFF |
| CORS Scanner | Nuclei | 🟡 MEDIUM | ✅ ON |
| Security Headers | HTTPX | 🟡 MEDIUM | ✅ ON |
| Directory Fuzzer | FFUF / Gobuster | — | ✅ ON |
| Parameter Discovery | ParamSpider | — | ✅ ON |
| Subdomain Takeover | Subjack / Subzy | 🔴 CRITICAL | ✅ ON |
| Secret Hunter | TruffleHog / GitLeaks | 🔴 CRITICAL | ✅ ON |
| Wayback Machine | Waybackurls | — | ✅ ON |
| JS Analyzer | LinkFinder | — | ✅ ON |
| WAF Detector | wafw00f | — | ✅ ON |
| Open Redirect | Custom | — | ✅ ON |
| API Fuzzer | Custom | — | ✅ ON |
| SSL/TLS Scanner | TestSSL.sh | — | ✅ ON |
| CMS Scanner | WPScan | — | ✅ ON |
| 403 Bypass | Custom | — | ✅ ON |
| HTTP Smuggling | Custom | 🔴 CRITICAL | ⚫ OFF |
| OAuth Analyzer | Custom | 🔴 CRITICAL | ⚫ OFF |
| GraphQL Audit | Custom | — | ⚫ OFF |

</details>

---

## 🛠️ Tool Arsenal

<details>
<summary><b>View all 35+ tools</b></summary>

### Reconnaissance
`Subfinder` `Amass` `HTTPX` `DNSX` `Gau` `Waybackurls` `ParamSpider` `Arjun` `Cloudflair`

### Port Scanning
`Nmap` `RustScan` `Masscan`

### Vulnerability Scanning
`Nuclei` `Nikto`

### Exploitation
`SQLMap` `Ghauri`

### XSS
`DalFox` `KXSS`

### Fuzzing
`FFUF` `Gobuster` `Feroxbuster` `WFuzz`

### Web Crawling
`Katana` `Hakrawler`

### JavaScript Analysis
`LinkFinder` `SecretFinder`

### Secrets & Credentials
`TruffleHog` `GitLeaks`

### Subdomain Takeover
`Subjack` `Subzy`

### SSRF
`SSRFMap`

### Cloud
`S3Scanner`

### TLS/SSL
`TestSSL.sh`

### CMS
`WPScan`

</details>

---

## 💣 Payload Library

80+ curated payloads across 7 categories — click any chip to copy instantly.

| Category | Count | Use Case |
|----------|-------|----------|
| XSS | 9 | Reflected, DOM, Stored XSS |
| SQL Injection | 10 | Error-based, Union, Blind, Time-based |
| SSRF / LFI | 10 | AWS metadata, file read, path traversal |
| Auth Bypass | 10 | IDOR, JWT, role escalation |
| Command Injection | 8 | OS command execution |
| XXE / XML | 3 | File read, SSRF via XML |
| Open Redirect | 6 | Parameter-based redirect abuse |

---

## 📄 PDF Report

The PDF export generates a **professional security assessment report** containing:

- **Cover page** with target, risk score (0–100), date, mode, and developer signature
- **Executive Summary** with severity breakdown and risk bar
- **Table of Contents** with all findings indexed by severity
- **Per-Finding Detail** including:
  - 🎯 What to focus on (priority guidance)
  - 🛠️ How to use the tool (exact commands)
  - 🔧 Remediation steps (numbered checklist)
  - ✅ Fix guidance (developer-level code advice)
- **Remediation Priority Matrix** with effort level and timeline for every finding

> **How to save as PDF:** Click `📄 PDF Report` → Browser opens report in new tab → `Ctrl+P` / `Cmd+P` → **Save as PDF**

---

## 📊 Scan Modes

| Mode | Description |
|------|-------------|
| 🔍 **Recon** | Passive + active subdomain, DNS, port enumeration |
| 💉 **Vuln Scan** | Full vulnerability scan — Nuclei, SQLi, XSS, SSRF |
| 🗂️ **Fuzzing** | Directory, file, and parameter brute-force |
| 🌐 **OSINT** | Passive intelligence gathering only |
| 📡 **API Audit** | REST/SOAP/GraphQL security testing |
| ⚡ **God Mode** | All modules active simultaneously |

---

## ⚙️ Configuration Options

| Setting | Default | Description |
|---------|---------|-------------|
| Threads | 50 | Concurrent scan threads |
| Timeout | 10s | Request timeout per host |
| Rate | 150 req/s | HTTP request rate limit |
| Crawl Depth | 3 | Web crawler depth |
| Severity | All | Filter output by severity |
| Wordlist | raft-large | Fuzzing wordlist preset |
| HTTP Proxy | None | Route through Burp/ZAP |

---

## 🔒 Security Notes

> ⚠️ **For authorized security testing only.**

- All scan operations shown in this tool are **simulations** — no real network requests are made
- Payloads in the library are stored as **base64-encoded JSON** — they cannot execute within the tool itself
- All DOM manipulation uses `textContent` and `createElement` — zero `innerHTML` with untrusted data
- This tool is designed as a **reference and workflow aid** for security professionals

**Never use this tool against targets you do not have explicit written authorization to test.**  
Unauthorized security testing is illegal under laws including the CFAA (US), Computer Misuse Act (UK), and IT Act (India).

---

## 📁 Project Structure

```
AdiSecLab.html          ← Entire platform in one file
│
├── CSS                 ← Design system (CSS variables, components)
├── HTML                ← 9 pages (Scanner, Modules, Findings, Commands,
│                           Payloads, Tools, Notebook, Config, About)
└── JavaScript          ← IIFE module (navigation, scan engine, exports,
                            payload library, PDF generator, detail view)
```

**No build step. No framework. No dependencies.**  
Pure HTML + CSS + Vanilla JavaScript.

---

## 🗺️ Roadmap

- [ ] Real scan integration via API bridge (optional backend)
- [ ] Import external scan results (JSON/XML)
- [ ] Custom finding templates
- [ ] Dark/light theme toggle
- [ ] Workspace save/load (IndexedDB)
- [ ] Browser extension version
- [ ] Collaborative mode (shared findings)

---

## 🤝 Contributing

Contributions are welcome!

```bash
# Fork the repo, then:
git clone https://github.com/YOUR_USERNAME/adiseclab.git
cd adiseclab

# Make changes to AdiSecLab.html
# Test in browser
# Submit a pull request
```

**Ideas for contributions:**
- New payload categories
- Additional command references
- More tool entries
- UI improvements
- Bug fixes

---

## 📜 License

```
MIT License

Copyright (c) 2024 Aditya Bhosale

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND.
```

---

## 📬 Contact

<div align="center">

| Platform | Link |
|----------|------|
| 💼 LinkedIn | [linkedin.com/in/bhsoaleaditya](https://www.linkedin.com/in/bhsoaleaditya/) |
| 📧 Email | [adityabhosale212223@gmail.com](mailto:adityabhosale212223@gmail.com) |

**Open to:** Collaboration · Responsible Disclosure · Freelance Pentesting · Consulting

</div>

---

<div align="center">

**Built with ❤️ by [Aditya Bhosale](https://www.linkedin.com/in/bhsoaleaditya/)**  
*Making the internet more secure, one CVE at a time.*

⭐ **Star this repo if you find it useful!**

</div>
