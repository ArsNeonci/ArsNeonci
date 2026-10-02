# Chu Quang Linh

**Backend / Platform / Applied AI Engineer — Internship Candidate**

Final-year Information Technology student at **Thang Long University**, focused on building backend systems, microservices platforms, cloud infrastructure, and AI-enabled applications.

My strongest area is understanding a system end-to-end: from **architecture, service boundaries, data ownership, API/security contracts, and infrastructure** down to how each module is implemented and integrated.

I use AI coding agents as development tools, while keeping ownership of architecture, technical constraints, integration decisions, review, and debugging.

---

## What I can work on

### Backend Engineering
- Design microservices boundaries and service-owned data models.
- Build REST APIs with **Java/Spring Boot, Go/Gin, and Python/FastAPI**.
- Design authentication and authorization flows with **API Gateway, JWT/RS256, RBAC, and trusted service context**.
- Work with **PostgreSQL, MongoDB, RabbitMQ, migrations, transactions, idempotency, and asynchronous processing**.
- Integrate services without direct cross-service database coupling.

### Platform / Cloud / DevOps
- Containerize multi-service systems with **Docker and Docker Compose**.
- Define cloud infrastructure using **Terraform**.
- Deploy and organize workloads on **Kubernetes/k3s**.
- Work with **GCP, Traefik, Cloudflare Tunnel / Zero Trust, GitHub Actions, and Artifact Registry**.
- Build CI workflows for multi-language projects and service-specific image builds.

### Applied AI / AI Backend
- Integrate **LLMs, MCP tool execution, RAG, multimodal document processing, and face recognition** into business systems.
- Build AI services with **FastAPI, MongoDB, RabbitMQ, pgvector, HNSW, and Gemini Embeddings**.
- Design permission-aware AI tools, human approval for critical actions, and AI-to-backend trust boundaries.
- Build document pipelines for extraction, OCR, chunking, embeddings, hybrid retrieval, and grounded citations.

---

## Main Project — ERP ARS NeonCI

A personal ERP platform built to explore **microservices architecture, distributed backend systems, cloud deployment, and applied AI integration**.

### Project scale

| Area | Current implementation |
|---|---|
| Application services | **11** |
| ERP business domains | **6** |
| PostgreSQL logical databases | **10** |
| AI services | **3** |
| MCP tools | **176** |
| Kubernetes Deployments | **17** |
| Kubernetes Services | **16** |
| Active application Dockerfiles | **12** |
| Supported document extensions | **11** |

### Architecture focus

```text
Users
  |
  v
Next.js Frontend
  |
  v
API Gateway
  |
  +----------------------+----------------------+----------------------+
  |                      |                      |                      |
  v                      v                      v                      v
Identity            ERP Services           AI Services          Public APIs
                       |                      |
                       |                      +--> Orchestrator / MCP
                       |                      +--> Multimodal / RAG
                       |                      +--> Face Recognition
                       |
                       +--> CRM / Finance / HRM
                       +--> Inventory / Purchasing / Sales
  |
  v
PostgreSQL / MongoDB / RabbitMQ / pgvector
```

### Engineering decisions I focused on

- **Database-per-service:** each service owns its schema and persistence.
- **Gateway trust boundary:** external identity is validated at the edge; downstream services receive short-lived signed context.
- **Cross-service consistency:** REST, external IDs, transactional outbox, RabbitMQ events, and idempotent consumers instead of cross-database writes.
- **AI permission boundaries:** LLM tools are allowlisted, permission-filtered, risk-classified, and executed through the existing backend authorization path.
- **RAG isolation:** document lifecycle remains in MongoDB while semantic vectors are isolated in pgvector; async ingestion uses RabbitMQ workers and falls back to keyword retrieval when semantic retrieval is unavailable.
- **Infrastructure as code:** Docker, Kubernetes, Terraform, GCP, Traefik, and Cloudflare are used to describe and run the platform.

---

## Technology Stack

### Languages
`Java` `Go` `Python` `TypeScript`

### Backend
`Spring Boot` `Spring Cloud Gateway` `Gin` `FastAPI` `REST APIs`

### Data & Messaging
`PostgreSQL` `pgvector` `MongoDB` `RabbitMQ` `Flyway` `GORM`

### AI
`Gemini API` `Gemini Embeddings` `MCP` `RAG` `HNSW` `Tesseract OCR` `InsightFace` `ONNX Runtime`

### Frontend
`Next.js` `React` `TypeScript` `Tailwind CSS`

### Cloud & Infrastructure
`Docker` `Docker Compose` `Kubernetes` `k3s` `Terraform` `GCP` `GitHub Actions` `Traefik` `Cloudflare`

---

## How I approach engineering

I prefer working from system intent to implementation:

```text
Requirement
   ↓
Architecture
   ↓
Service / Data Boundaries
   ↓
API & Security Contracts
   ↓
Implementation Plan
   ↓
AI-assisted Development
   ↓
Integration Review
   ↓
Debugging / Refinement
   ↓
Deployment
```

I am most interested in roles where I can combine **backend engineering, system design, cloud/platform knowledge, and practical AI integration**.

---

## Roles I am interested in

- Backend Engineer Intern
- Software Engineer Intern
- AI Backend Engineer Intern
- AI Application Engineer Intern
- Platform / Cloud Engineer Intern
- DevOps Engineer Intern

My strongest overlap is currently:

**Backend Engineering + Platform / Cloud + Applied AI**

---

## Current learning focus

- Distributed systems and backend reliability
- Observability and tracing
- Production-grade CI/CD and deployment strategies
- RAG evaluation and AI system reliability
- Cloud-native architecture and Kubernetes operations

---

## Contact

- **GitHub:** https://github.com/ArsNeonci
- **Email:** quanglinh1286@gmail.com
- **Location:** Hanoi, Vietnam

If you are reviewing my profile for an internship opportunity, the ERP project is the best place to see how I approach architecture, backend integration, cloud infrastructure, and AI-enabled software systems.
