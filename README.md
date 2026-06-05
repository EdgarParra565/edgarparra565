# Edgar Parra
**CS & Mathematics @ Northeastern University · Incoming IBM Co-Op · Fall 2026**

Boston, MA · [parra.ed@northeastern.edu](mailto:parra.ed@northeastern.edu) · [LinkedIn](https://linkedin.com/in/edgar-parra2028) · [GitHub](https://github.com/EdgarParra565)

---

## About Me

Sophomore at Northeastern's Khoury College of Computer Science studying CS and Mathematics (GPA 3.6). I build across the full stack — production web apps, probabilistic modeling systems, low-level systems software in C, and network servers in Go.

Incoming **Forward Deploy Engineer Co-Op at IBM** (Silicon Valley Lab, San Jose · Fall 2026).

---

## Experience

**Forward Deploy Engineer Co-Op** · IBM · Silicon Valley Lab, San Jose, CA · Sep 2026 – Dec 2026 *(incoming)*

**Painter / Web Developer** · Ed's Painting and Construction · 2024 – 2025
Built and deployed a full-stack Flask/PostgreSQL web app handling 30+ real customer inquiries monthly. Implemented authentication, CSRF protection, rate limiting, automated email notifications, and a mobile-friendly UI.

---

## Projects

### [NBA Props Forecaster & Cross-Book Arbitrage System](https://github.com/EdgarParra565/player-performance-forecaster) · Python · *Jan 2025 – Present*
Full-stack probabilistic sports analytics platform with a Streamlit web app, FastAPI webhook server, and SQLite database spanning 90K+ player game log rows and 8K+ team-game rows across 3 seasons. Implements Monte Carlo simulation, rolling feature engineering, and multiple distribution families (normal, Poisson, Student-t, lognormal, power-law) with correlation-aware multivariate modeling for parlay legs.

Cross-book arbitrage pipeline ingests odds from 9 active sportsbooks (PrizePicks, DraftKings, BetMGM, Caesars, Bovada, and others) via Playwright CDP scraping, strips vig to extract implied probabilities, and surfaces cross-market discrepancies as value signals. Production-ready auth and billing scaffold with Google/Microsoft OIDC, Stripe Free/Premium tier gating, FastAPI webhook with HMAC verification, per-IP rate limiting, and OWASP-compliant HTTP security headers. Evaluated with Brier score, Sharpe ratio, Wilson confidence intervals, CLV proxies, and z-tests against breakeven. **182/182 tests passing.**

### [Redis-Like Database Server](https://github.com/EdgarParra565) · Go · *May 2026 – Present*
TCP server in Go implementing the RESP protocol from scratch. Supports SET, GET, HSET, HGET, and PING with in-memory string and hash storage. Layered architecture separating RESP parsing and marshaling, command dispatch, in-memory stores, and an append-only file helper for persistence. Compatible with redis-cli.

### [NUFS — Userspace File System](https://github.com/EdgarParra565) · C · *March 2026 – April 2026*
Persistent Unix-like file system built from scratch in C, exposed to the Linux kernel via FUSE. Supports `ls`, `mkdir`, `cat`, `echo`, `mv`, `rm`, and nested directories on a 1 MB disk image. Inode-based architecture with dual free-space bitmaps and a layered storage abstraction (FUSE callbacks → storage → inode/directory → block allocator) with mmap'd disk image for persistence. Full `read`/`write`/`create`/`delete`/`rename`/`truncate`/`utimens` support with permission bits and `stat(2)` metadata.

### [ugit — Git Reimplementation](https://github.com/EdgarParra565) · Python · *May 2026*
Core Git internals rebuilt from scratch: content-addressed object store (blobs, trees, commits) with SHA-1 hashing, a ref system for branches and tags, and a JSON-backed staging index. DAG-based commit history traversal, three-way merge with conflict detection, and local fetch/push with remote ref tracking. Layered architecture separating object I/O (`data.py`), repository logic (`base.py`), and CLI (`cli.py`) — mirroring Git's own plumbing/porcelain separation.

### [Java Game Development Suite](https://github.com/EdgarParra565/SolitaireGame) · Java · *Feb 2025 – Dec 2025*
Tetris, Klondike Solitaire, and a custom card game built from scratch using OOP principles and MVC architecture. AI opponents with strategy patterns, custom Swing/AWT GUI components, and design patterns including observer, strategy, and factory.

### [BasicShell](https://github.com/EdgarParra565/BasicShell) · C · *Sep 2025 – Nov 2025*
Unix shell in C supporting piped command chains, I/O redirection (`<`, `>`, `>>`), conditional operators (`&&`/`||`), background processes, and environment variable expansion. Built on `fork()`/`execvp()`/`waitpid()`/`pipe()` with a custom tokenizer and dynamic vector data structure.

---

## Skills

**Languages:** Java · Python · C · Go · JavaScript · HTML/CSS · OCaml · Kotlin
**Frameworks:** Flask · SQLAlchemy · Flask-WTF · FastAPI · Streamlit · Java Swing/AWT
**Tools:** Git · PostgreSQL · SQLite · Docker · Linux/Unix · Bash · FUSE · Playwright · Maven · JUnit
**Practices:** REST APIs · MVC · Database Design · Auth & Security · Statistical Modeling · Web Scraping · CI/CD
**Math:** Probability & Statistics · Linear Algebra · Differential Equations · Group Theory · Monte Carlo Methods

---

## Education

**Northeastern University** · B.S. Computer Science & Mathematics · Sep 2024 – May 2028 · GPA 3.6
Khoury College of Computer Science · Boston, MA

**Coursework:** Object Oriented Design · Computer Systems · Logic & Computation · Discrete Structures · Probability & Statistics · Linear Algebra · Differential Equations · Group Theory · Algorithms · Calculus I–III · Probability and Risk

**Organizations:** NEU SHPE · NEU ALPFA · NEU Math Club

---

## Languages

English (Native) · Spanish (Native)
