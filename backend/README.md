# MEAP Backend

ASP.NET Core 8 Web API that will provide enterprise-grade authentication, user management, audit logging, and system monitoring.
This document will be updated as the project evolves.

## Planned Tech Stack
- **ASP.NET Core 8** Web API
- **Entity Framework Core** + PostgreSQL
- **JWT** + Refresh Tokens (Argon2 password hashing)
- **Role/Claim-based** authorization
- **Serilog** structured JSON logging
- **Prometheus** metrics endpoint (`/metrics`)

## Planned Features
- 🔐 JWT authentication with refresh token rotation
- 👥 User & role management (Admin, User, Auditor)
- 📋 Comprehensive audit logging
- 📊 System health & diagnostics endpoints
- 🐳 Production-ready Docker deployment