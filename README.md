# MEAP – Mini Enterprise Admin Platform

MEAP is a fullstack, production-style admin platform built with **ASP.NET Core**, **React + TypeScript**, **PostgreSQL**, and a fully self-hosted **Linux/DevOps infrastructure** (Docker, Nginx, Prometheus, Grafana, automated backups, CI/CD, and monitoring).

The goal is to demonstrate real-world experience in **system architecture**, **backend development**, **frontend development**, **DevOps**, **Linux server administration**, and **operational excellence** all inside a single cohesive project.

This repository is structured as an enterprise-like monorepo with clear separation between application code, infrastructure, and documentation.

---

## 🌐 Features (Planned + Implemented)

### 🟣 Authentication & Authorization
- JWT authentication  
- Refresh tokens  
- Role-based access (Admin, User, Auditor)  
- Claim-based permissions  
- Role-aware UI in React  

### 🟣 User & Role Management
- User CRUD  
- Role CRUD  
- Assign / unassign roles  
- Validations (client + server)  

### 🟣 Audit Logging
- Login attempts  
- User/role changes  
- System-level events  
- Export to CSV  
- Viewable in the UI  

### 🟣 System Health Dashboard
- CPU / Memory per container  
- API latency  
- Request rate & 5xx errors  
- Database status  
- Uptime  
- Prometheus metrics exposed via `/metrics`  

### 🟣 DevOps & Infrastructure
- Docker Compose (API + Web + DB + Monitoring stack)  
- Nginx reverse proxy with HTTPS (Let’s Encrypt)  
- CI/CD with GitHub Actions  
- Linux VPS hardening (SSH, firewall, fail2ban)  
- Automated PostgreSQL backups  
- Logging with Serilog  

### 🟣 Observability
- Prometheus  
- Grafana dashboards  
- Alert rules for CPU, memory, disk, and latency  

---

## 📁 Project Structure

backend/        # ASP.NET Core Web API
frontend/       # React + TypeScript application
infra/          # Docker, Nginx, Prometheus, Grafana, scripts
docs/           # Architecture, roadmap, diagrams

---

## 🚀 Deployment Model

MEAP is hosted on a self-managed Linux VPS (e.g., Hetzner) to demonstrate end-to-end control:

- Nginx reverse proxy
- Docker Compose orchestration
- SSL termination
- Monitoring stack
- Backup scripts
- Hardened OS configuration

This provides a **complete dev → deploy → operate** lifecycle, similar to how small companies run their systems.

---

## 🧭 Documentation

For a deeper explanation of the architecture, planned features, and DevOps pipeline, see:

- `/docs/architecture.md`
- `/docs/roadmap.md`

---

## 🔧 Development Status

This project is actively under construction.  
New features are being added through isolated feature branches and reviewed before merging into `main`.

---

## 📜 License

MIT License – free to use and learn from.