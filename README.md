# Edgar Parra

**CS & Mathematics @ Northeastern University · Incoming SDE Intern @ AWS (Summer 2027) · SWE Co-Op @ IBM (Fall 2026)**

Boston, MA · [parra.ed@northeastern.edu](mailto:parra.ed@northeastern.edu) · [LinkedIn](https://www.linkedin.com/in/edgar-parra2028) · [GitHub](https://github.com/EdgarParra565)

---

## About Me

Junior at Northeastern's Khoury College of Computer Sciences studying CS and Mathematics. I build backend and data systems: database servers in Go, build infrastructure for mainframe software at IBM, production web apps, and data pipelines.

Incoming Software Development Engineer Intern at Amazon Web Services in New York (Summer 2027), and currently a Software Engineer Co-Op at IBM's Silicon Valley Lab.

---

## Experience

**Incoming SDE Intern** · Amazon Web Services · New York, NY · May 2027 – Jul 2027

**Software Engineer Co-Op** · IBM · Silicon Valley Lab, San Jose, CA · Sep 2026 – Dec 2026

Software engineer on the Db2 for z/OS team, working on IBM Dependency Based Build (DBB), the build platform replacing zBuild. Consolidating build metadata from static JSON and XML files into a relational database with a UI, and built a Java renderer, triggered through a Spring Boot endpoint, that regenerates and commits product-specific files whenever the metadata changes. Also porting CopySend into DBB as a Groovy job on our Jenkins pipeline, including APAR/PTF fix-driver support and a downlevel check so older load modules never overwrite newer ones.

**Painter / Web Developer** · Ed's Painting and Construction · Feb 2024 – Dec 2025

Built and deployed a full-stack Flask/PostgreSQL web app on Render that handles 30+ real customer inquiries a month. Implemented authentication, CSRF protection, rate limiting, instant cost estimation tools, automated email notifications, and a mobile-friendly UI.

---

## Projects

### [NBA Props Forecaster & Cross-Book Arbitrage System](https://github.com/EdgarParra565/player-performance-forecaster) · Python, TypeScript · Dec 2025 – Present

A pricing and measurement system for NBA player props. A trading-terminal-style React/TypeScript frontend (Vite, Tailwind, ECharts) sits over a read-only FastAPI service and a SQLite database with 90K+ player game logs, 8K+ team games, and 65K settled predictions.

An hourly, change-only ETL pipeline ingests lines from 10+ sportsbooks through browser automation, de-vigs posted odds into implied probabilities, and separates line shopping, middles, and true two-way arbitrage across books.

Forecasting uses Monte Carlo simulation, rolling features, and 8 distribution families (normal, Student-t, Poisson, binomial, negative binomial, lognormal, exponential, power law), with team-total priors and correlation-aware pricing for parlays. Forecasts are scored against historical outcomes with Brier scores, reliability tables, and closing line value. Code-splitting ECharts cut the initial bundle from 1.4 MB to 370 KB. 1,200+ tests across backend, API, and frontend.

### [Redis-Compatible Database Server](https://github.com/EdgarParra565/DataBaseRedisRecreation) · Go · May 2026 – Present

Concurrent TCP server in Go implementing the Redis Serialization Protocol (RESP) from scratch, compatible with `redis-cli`. Supports 18 commands, with each client handled in its own goroutine and read-write locks protecting the shared data stores.

Append-only file persistence with full startup replay including TTL restoration, plus lazy key expiration on access and a background cleanup goroutine. Also includes an MCP server built with the official Go SDK, exposing 13 tools so AI agents can store and query data, with a read-only mode and key-prefix allowlist for safe access. Covered by unit and concurrent stress tests.

### [NUFS: Userspace File System](https://github.com/EdgarParra565/FileSystemProject) · C, FUSE · March 2026 – April 2026

Persistent Unix-like file system built from scratch in C, exposed to the Linux kernel via FUSE. Supports `ls`, `mkdir`, `cat`, `echo`, `mv`, `rm`, and nested directories on a 1 MB disk image. Inode-based architecture with dual free-space bitmaps, an mmap'd disk image for persistence, and a layered storage design separating FUSE callbacks, storage, inode and directory logic, and block allocation.

### [ugit: Git Reimplementation](https://github.com/EdgarParra565/GitRecreation) · Python · May 2026

Core Git internals rebuilt from scratch: a content-addressed object store (blobs, trees, commits) with SHA-1 hashing, refs for branches and tags, and a JSON-backed staging index. DAG-based history traversal, three-way merge with conflict detection, and local fetch/push with remote ref tracking.

### [BasicShell](https://github.com/EdgarParra565/BasicShell) · C · Feb 2026 – April 2026

Unix shell in C supporting piped command chains, I/O redirection (`<`, `>`, `>>`), conditional operators (`&&`/`||`), background processes, and environment variable expansion. Built on `fork()`/`execvp()`/`waitpid()`/`pipe()` with a custom tokenizer.

### Java Game Development Suite · Java, JDK 21 · Feb 2025 – Dec 2025

Three games built from scratch using OOP and MVC: [Tetris](https://github.com/EdgarParra565/Tetris-Recreation), Klondike Solitaire, and a [custom card game](https://github.com/EdgarParra565/GameDemoOOD). AI opponents with strategy patterns, custom Swing/AWT components, and observer, strategy, and factory patterns.

---

## Skills

**Languages:** Java · Python · Go · C · JavaScript · SQL · HTML/CSS
**Frameworks & Libraries:** Spring Boot · Flask · SQLAlchemy · FastAPI · React · JUnit
**Tools:** Git · PostgreSQL · SQLite · Docker · Jenkins · Linux/Unix · Bash · Maven · Playwright · FUSE · IBM DBB · Db2 · z/OS
**Practices:** REST APIs · Database Design · Concurrency · Auth & Security · CI/CD · Statistical Modeling · Web Scraping · Model Context Protocol (MCP)

---

## Education

**Northeastern University** · B.S. Computer Science & Mathematics · Sep 2024 – May 2028 · GPA 3.6
Khoury College of Computer Sciences · Boston, MA

**Coursework:** Algorithms · Object Oriented Design · Computer Systems · Introduction to Databases · Discrete Structures · Logic & Computation · Probability & Statistics · Probability and Risk · Linear Algebra · Differential Equations · Group Theory · Calculus I–III

**Organizations:** NEU SHPE · NEU ALPFA · NEU Math Club

---

## Languages

English (Native) · Spanish (Native)
