# Edgar Parra

**CS & Mathematics @ Northeastern University · Incoming IBM Co-Op · Fall 2026**

Boston, MA · [parra.ed@northeastern.edu](mailto:parra.ed@northeastern.edu) · [LinkedIn](https://www.linkedin.com/in/edgar-parra2028) · [GitHub](https://github.com/EdgarParra565)

---

## About Me

Sophomore at Northeastern's Khoury College of Computer Sciences studying CS and Mathematics. I build across the full stack — production web apps, probabilistic modeling systems, low-level systems software in C, and network servers in Go.

Incoming Forward Deploy Engineer Co-Op at IBM (Silicon Valley Lab, San Jose · Fall 2026).

**Seeking Summer 2027 software engineering internships.** Available May – December 2027.

---

## Experience

**Forward Deploy Engineer Co-Op** · IBM · Silicon Valley Lab, San Jose, CA · Sep 2026 – Dec 2026 *(incoming)*

**Painter / Web Developer** · Ed's Painting and Construction · Feb 2024 – Dec 2025
Built and deployed a full-stack Flask/PostgreSQL web app handling 30+ real customer inquiries monthly. Implemented authentication, CSRF protection, rate limiting, automated email notifications, and a mobile-friendly UI.

---

## Projects

### [NBA Props Forecaster & Cross-Book Arbitrage System](https://github.com/EdgarParra565/player-performance-forecaster) · Python, TypeScript · Dec 2025 – Present

Full-stack probabilistic sports analytics platform. Trading-terminal-style React/TypeScript frontend (Vite, Tailwind, ECharts) backed by a read-only FastAPI service, over a SQLite database spanning 90K+ player game-log rows and 8K+ team-game rows across three seasons.

The odds pipeline covers 20+ sportsbooks via Playwright CDP scraping and an 11-book aggregator parser, running hourly on a scheduled ETL with change-only ingestion and login-wall detection. De-vigs posted lines into implied probabilities and surfaces line-shopping, middle, and true-arbitrage signals across books.

Forecasting uses Monte Carlo simulation, rolling feature engineering, and 8 distribution families (normal, Poisson, negative binomial, Student-t, lognormal, power-law) with team-total priors and correlation-aware multivariate modeling for parlay legs. Code-splitting ECharts cut the initial bundle from 1.4 MB to 370 KB.

Production scaffold: Google/Microsoft OIDC sign-in, Stripe tiers with Customer Portal, HMAC-verified webhooks, per-IP rate limiting, and OWASP-compliant security headers. Validated with a paper-trading and calibration stack (Brier/reliability reports, CLV proxies, Kelly-capped slip export, z-tests against breakeven). 737 tests passing across backend, API, and frontend.

### [Redis-Like Database Server](https://github.com/EdgarParra565/DataBaseRedisRecreation) · Go · May 2026 – Jun 2026

Concurrent TCP server in Go implementing the Redis Serialization Protocol (RESP) from scratch, compatible with `redis-cli`. Supports 12 commands including SET, GET, DEL, INCR, EXPIRE, TTL, KEYS, HSET, and HGET across in-memory string and hash stores, with one goroutine per connection.

Append-only file persistence with full startup replay including TTL restoration, lazy key expiration on access, and a background cleanup goroutine scanning expirations every 100ms. Layered architecture separating RESP parsing, command dispatch, in-memory stores, expiration tracking, and AOF write/replay, with unit tests covering protocol output, handlers, persistence, expiration, and concurrent stress.

### [NUFS — Userspace File System](https://github.com/EdgarParra565/FileSystemProject) · C, FUSE · March 2026 – April 2026

Persistent Unix-like file system built from scratch in C, exposed to the Linux kernel via FUSE. Supports `ls`, `mkdir`, `cat`, `echo`, `mv`, `rm`, and nested directories on a 1 MB disk image. Inode-based architecture with dual free-space bitmaps and a layered storage abstraction (FUSE callbacks → storage → inode/directory → block allocator) with mmap'd disk image for persistence. Full read/write/create/delete/rename/truncate/utimens support with 48-byte dirent entries, permission bits, and stat(2) metadata.

### [ugit — Git Reimplementation](https://github.com/EdgarParra565/GitRecreation) · Python · May 2026

Core Git internals rebuilt from scratch: content-addressed object store (blobs, trees, commits) with SHA-1 hashing, a ref system for branches and tags, and a JSON-backed staging index. DAG-based commit history traversal, three-way merge with conflict detection, and local fetch/push with remote ref tracking. Layered architecture separating object I/O (`data.py`), repository logic (`base.py`), and CLI (`cli.py`) — mirroring Git's own plumbing/porcelain separation.

### [BasicShell](https://github.com/EdgarParra565/BasicShell) · C · Feb 2026 – April 2026

Unix shell in C supporting piped command chains, I/O redirection (`<`, `>`, `>>`), conditional operators (`&&`/`||`), background processes, and environment variable expansion. Built on `fork()`/`execvp()`/`waitpid()`/`pipe()` with a custom tokenizer and dynamic vector data structure.

### Java Game Development Suite · Java, JDK 21 · Feb 2025 – Dec 2025

Three games built from scratch using OOP principles and MVC architecture: [Tetris](https://github.com/EdgarParra565/Tetris-Recreation), Klondike Solitaire, and a [custom card game](https://github.com/EdgarParra565/GameDemoOOD). AI opponents with strategy patterns, custom Swing/AWT GUI components, and design patterns including observer, strategy, and factory.

---

## Skills

**Languages:** Java · Python · C · Go · TypeScript · JavaScript · HTML/CSS · OCaml · Kotlin
**Frameworks:** Flask · SQLAlchemy · Flask-WTF · FastAPI · React · Streamlit · Java Swing/AWT
**Tools:** Git · PostgreSQL · SQLite · Docker · Linux/Unix · Bash · FUSE · Playwright · Vite · Maven · JUnit
**Practices:** REST APIs · MVC · Database Design · Auth & Security · Concurrency · Statistical Modeling · Web Scraping · CI/CD
**Math:** Probability & Statistics · Linear Algebra · Differential Equations · Group Theory · Monte Carlo Methods

---

## Education

**Northeastern University** · B.S. Computer Science & Mathematics · Sep 2024 – May 2028 · GPA 3.6
Khoury College of Computer Sciences · Boston, MA

**Coursework:** Object Oriented Design · Computer Systems · Logic & Computation · Discrete Structures · Algorithms · Introduction to Databases · Probability & Statistics · Probability and Risk · Linear Algebra · Differential Equations · Group Theory · Calculus I–III

**Organizations:** NEU SHPE · NEU ALPFA · NEU Math Club

---

## Languages

English (Native) · Spanish (Native)
