# Hi, I'm Ricardo 

BSc Computer Science graduate from the University of Sunderland, based in the UK.
I build Python tools that solve real problems, from data automation and database pipelines
to web scraping and collection management. I like projects that sit at the intersection
of clean engineering and something I actually care about.

---


##  What I Work With

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

---

##  Projects

### [DeckMaster](https://github.com/RiGraMa/deckMaster)
A Python toolkit for Magic: The Gathering players, built as a passion project that grew
into a multi-tool application demonstrating real software engineering practices.

**What it does:**
- Scrapes average Commander decklists from EDHREC
- Migrates ManaBox CSV exports into a SQLite collection database
- Cross-references any decklist against your personal collection
- Analyses the competitive metagame across multiple formats (Pauper, Modern, Vintage)
  by scraping MTGGoldfish, with local caching to avoid redundant downloads
- Flask web interface with Scryfall API integration to visually browse your decklists,
  showing owned and missing cards with card images loaded in real time

**Technical highlights:**
- Modular architecture — two independent programs sharing a common database layer
- SQLite migration from CSV with a dedicated one-time migration script
- Multi-format meta analyzer with a file-based caching system
- Scryfall API integration with rate-limit-aware lazy loading
- Clean separation of concerns across scraping, caching, analysis and presentation layers

---

### [GameScript — PDF to Game Inputs Converter](https://github.com/RiGraMa/GameScript-PDF-to-Game-Inputs-Converter)
Converts any text document into a deterministic sequence of game controller inputs,
then automates playback through a Lua script in the DeSmuME emulator.

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
- Modular design — each script has one clearly defined job

---

##  Get in Touch

- GitHub: [@RiGraMa](https://github.com/RiGraMa)
- Location: Sunderland, UK
- Open to: Graduate software developer and data roles
