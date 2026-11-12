# Hi, I'm Ricardo 👋
 
BSc (Hons) Computer Science graduate from the University of Sunderland, based in Sunderland, UK.
 
I build Python tools and cloud infrastructure that solve real problems, from web apps and database pipelines to AWS deployments and self-hosted monitoring. I like projects that go all the way from design through to a live, working deployment.
 
---
 
## 🛠 What I Work With
 
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
 
---
 
## 🚀 Projects
 
### [AWS Cloud Infrastructure & Observability](https://github.com/RiGraMa) — Live `rochasbirthday.xyz`
A self-hosted monitoring stack deployed and secured on AWS from the ground up.
 
**What it does:**
- Static site served from S3 behind CloudFront as a global CDN over HTTPS
- ACM TLS certificate provisioned with DNS validation; custom domain configured (ALIAS, CNAME records)
- Prometheus, Node Exporter and Grafana running as systemd services on EC2, live at `metrics.rochasbirthday.xyz`
- Nginx reverse proxy in front of Grafana with a Let's Encrypt certificate
**Technical highlights:**
- EC2 security groups locked down to trusted IPs only, with IAM least-privilege applied throughout
- Elastic IP allocated for a stable public address
- Fully documented build process, including troubleshooting notes
---
 
### [DeckMaster](https://github.com/RiGraMa/deckMaster)

A Python/Flask toolkit for Magic: The Gathering players. I built it to compare Commander decklists against my own card collection, and it grew into a small multi-tool project.

**What it does:**

- Scrapes average Commander decklists from EDHREC
- Imports ManaBox CSV exports into a SQLite collection database
- Cross-references any decklist against your collection to show owned and missing cards
- Flask web interface with Scryfall API integration to browse decks with live card images
- Copy/download buttons for decklists in Moxfield/ManaBox-compatible text format

**Technical highlights:**

- Modular Flask blueprint structure with a shared database layer
- EDHREC changed its JSON format twice, so I extracted a single shared parser (`parse_edhrec_deck()`) that handles both formats and is the only place to update next time
- Rate-limit-aware Scryfall API integration
- Containerised with Docker, docker-compose and Gunicorn, with a GitHub Actions CI pipeline
- A metagame analysis tool for other formats is parked: the original source blocked scraping, and my rewrite is unfinished
 
### [Active Directory Home Lab](https://github.com/RiGraMa)
A hands-on enterprise infrastructure environment built from scratch.
 
**What it does:**
- Windows Server 2022 domain controller running Active Directory Domain Services
- Ubuntu Server with Apache and secure SSH access
- Internal virtual network with static IP addressing and DNS
**Technical highlights:**
- Users, groups, OUs and Group Policy Objects created and managed
- Security policies implemented, including account lockout and access restrictions
---
 
### [GameScript — PDF to Game Inputs Converter](https://github.com/RiGraMa/GameScript-PDF-to-Game-Inputs-Converter)
Converts any text document into a deterministic sequence of game controller inputs, then automates playback through a Lua script in the DeSmuME emulator.
 
In other words: the Portuguese Constitution can play Pokémon. For 47 hours straight.
 
**What it does:**
- Extracts text from PDF or plain text files
- Maps every character to a button press via a deterministic character table
- Generates a Lua automation script for DeSmuME with frame-accurate timing
- Supports Nintendo DS and Game Boy/GBA button mappings
- Full pipeline runs from a single command
**Technical highlights:**
- Three-stage pipeline: PDF → JSON → Lua, each stage independently usable via CLI
- Master orchestration script coordinates the full pipeline with subprocess isolation
- Frame-by-frame timing synchronisation at 60 FPS (9 frames per input)
- argparse CLI with sensible defaults and flexible overrides
---
 
## 📫 Get in Touch
 
- GitHub: [@RiGraMa](https://github.com/RiGraMa)
- LinkedIn: [ricardo-martins-b573101b1](https://www.linkedin.com/in/ricardo-martins-b573101b1/)
- Location: Sunderland, UK
- Open to: Graduate DevOps, cloud and software engineering roles
 
