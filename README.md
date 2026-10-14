# Tanmay Patel

### Building useful software. Understanding the systems beneath it.

**Software Engineer · Backend · Full-Stack · Systems & Infrastructure**

I build software end to end, from the first conversation about a business problem to the system running in production. Most of my work sits in backend systems, databases, and infrastructure, with enough frontend and mobile to ship complete products.

[Explore my repositories](https://github.com/tanmay-73?tab=repositories) · [Experience](#experience) · [Selected public projects](#featured-projects) · [LinkedIn](https://www.linkedin.com/in/tanmay-patel-1644501a2/)

---

## About me

I like problems where data has to move reliably, systems have to stay up, and the software has to fit how a business actually works.

Over the past few years I have taken production platforms from an idea to live systems used daily by staff, clients, and field teams. That work covers architecture, data models, APIs, authentication and access control, containers, CI/CD, observability, backups, and the support that keeps it all running.

I want to understand the tradeoffs behind an architecture as well as how to implement it. Over time, I’m deepening my foundations in computer science, mathematics, physics, and systems engineering.

## Experience

### Independent Software Engineer · Self-employed
*Jul 2024 – Present*

I design and build software for clients end to end: requirements, architecture, implementation, deployment, and production support.

- **Operations platform for Vidhyut Electromech.** I'm the sole developer of a production platform used by about 50 staff and 350–400 contractors across sites to manage 80 MW of plant capacity. Its Flutter Android app replaced the diaries, paper records, and WhatsApp groups field staff used to rely on.
  - Full stack: TypeScript/Express API, React + Vite frontend, PostgreSQL, shipped through containerized CI/CD.
  - Authentication and authorization built from scratch: JWT access/refresh tokens, email-OTP MFA, roles plus direct permission grants, and access scoped to assigned project stages. Access is re-checked on every request, and every mutation is audit-logged.
  - Safe to run as multiple instances: atomic Redis rate limiting, Postgres advisory locks for migrations, readiness/liveness probes with graceful shutdown, and request tracing.
- **SimplifyRad, a medical-report insights app (client project).** A Flutter app (Android, iOS, web) and a Django/PostgreSQL API. Users upload a report as an image or PDF, the API runs OCR, and a generative AI model explains it in plain language. Includes email OTP verification, guest access, uploads with retry, Markdown-rendered summaries, and report history.

### Full Stack Engineer · Climate Detox Renewables
*Mar 2025 – Aug 2026*

I built the company's EPC and O&M business platform from scratch, from the initial idea to a live system used by about 100 internal and client users. It holds data for 180 MW of solar plants and 10M+ rows of SCADA data.

- Designed and built the entire stack (TypeScript/Express, PostgreSQL, Redis, React), covering purchase orders, design and statutory stages, invoicing, accounts, HRMS, asset management, and solar O&M.
- Implemented multi-organization access control for staff and client users: JWT auth and role-, page-, and client-level permissions.
- Integrated live plant data: a scheduled iSolarCloud worker whose runs are configured from the database without restarts, and a SCADA data service feeding live dashboards and energy reports.
- Owned production infrastructure: migrated hosting from E2E Networks to AWS and object storage to S3, running Dockerized services behind Nginx with GitHub Actions deployments and OpenTelemetry/SigNoz observability.
- Built data protection tooling: a Go service for scheduled `pg_dump` backups with WAL archiving for point-in-time recovery, and an incremental object-storage backup tool.
- Shipped a Flutter app for attendance and O&M dashboards, plus Excel/PDF exports, a queue-driven PDF report worker, WebSocket chat in procurement workflows, and scheduled compliance reminders.
- Interviewed and onboarded two new team members, then handed the platform over to the team.

### Associate Software Engineer · Casepoint
*May 2022 – Jun 2024 (Software Engineering Intern, Jan – Apr 2022)*

I did engineering work on an eDiscovery platform, spanning a Windows desktop migration tool, a backend file-transfer service, and the main web application.

- Built core capabilities of an internal tool that migrated database and filesystem data from on-premises infrastructure to Microsoft Azure, including logical database backup and restore wired into the end-to-end migration.
- Built the file-transfer microservice for migrations, with multithreaded concurrent transfers and pause/resume of in-progress jobs.
- Built the foundation of an Investigator Workbench that turns Elasticsearch-indexed data into interactive D3.js visualizations.
- Contributed to a workspace-to-workspace data transfer module that touched many of the platform's major modules and its data model.
- Received Casepoint's **Sprint Delivery Stud** award. Joined as an intern and converted to a full-time role.

## What I work with

- **Languages:** TypeScript, JavaScript, SQL, Go, Dart, Python.
- **Backend:** Node.js, Express.js, Bun, Django, REST API design, authentication and authorization, background workers and queues, WebSockets.
- **Frontend and mobile:** React, Vite, HTML5, CSS3, Flutter (Android, iOS, web).
- **Data:** PostgreSQL (including advisory locks, WAL archiving, and point-in-time recovery), Redis, Elasticsearch, SQL database design.
- **Infrastructure:** Docker, Docker Compose, Linux / Ubuntu Server, Nginx, SSH, reverse proxies, server deployment and administration.
- **Cloud and delivery:** AWS (EC2, S3), Microsoft Azure, Cloudflare, GitHub Actions, Git, GitHub.
- **Observability:** OpenTelemetry, SigNoz, request tracing, health probes.
- **Desktop and tooling:** Electron, cross-platform desktop applications, CLI tooling, development environments, and automation.

## Featured projects

Most of my work is in client and company codebases. These public repositories offer a look at my work with development environments, networking, and application logic.

### DiskGrove

A cross-platform Electron disk space analyzer with directory-tree analysis, treemap, pie and bar visualizations, large-file discovery, and duplicate-file detection.

**TypeScript · Electron**

### [Dotfiles](https://github.com/tanmay-73/Dotfiles)

A personal Linux environment configuration that brings window management, terminal, shell, and desktop utilities together.

**Shell · i3 · Polybar · Rofi · Alacritty · Zsh**

Combines application configuration with scripts for desktop tasks such as locking the session and launching the status bar. The repository credits the dotfiles it builds on.

### [NetworkTools](https://github.com/tanmay-73/NetworkTools)

An Android networking project that puts ping, port scanning, subnet discovery, and Wake-on-LAN behind a mobile interface.

**Java · Android · Gradle**

Connects diagnostic screens to a bundled networking library, making network operations accessible through a single application. The repository identifies it as a semester design-engineering project.

### [Chatbot](https://github.com/tanmay-73/Chatbot)

A desktop chatbot that maps text input to predefined intents and responses.

**Python · NLTK · TensorFlow / Keras · Tkinter**

Links tokenization and lemmatization to bag-of-words features, a dense neural-network classifier, and a desktop chat interface. Includes training code and a saved model.

## Engineering interests

- **Backend and distributed systems:** API boundaries, service communication, running services as multiple instances, architecture, and performance.
- **Databases and storage:** database internals, storage systems, backups, and recovery.
- **Developer tools and infrastructure:** CLI tools, Linux, networking, observability, self-hosting, and homelab environments.
- **Systems fundamentals:** operating systems, algorithms, data structures, and systems programming.

## Currently exploring

Going deeper with **Go** for services and tooling, studying **system design and performance**, and digging into **database and storage internals**. I’m interested in applying that learning to useful software products and developer tools.

---

## Connect

- **GitHub:** [@tanmay-73](https://github.com/tanmay-73)
- **LinkedIn:** [Tanmay Patel](https://www.linkedin.com/in/tanmay-patel-1644501a2/)
- **X:** [@pateltanmay73](https://x.com/pateltanmay73)

Based in Navsari, Gujarat, India.
