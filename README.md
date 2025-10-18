
---

## 🎯 CP5 2025

**🛞 CP5 — Locadora de Carros: Reservas, Pagamentos e Observabilidade (ASP.NET Core 8 + Clean Architecture)**

**Integrantes do Grupo:**  
**Paulo André Carminati RM557881**  
**Turma: 2-TDSPZ**

**Repositório no GitHub**: [CP5 - Locadora de Carros: Reservas, Pagamentos e Observabilidade](https://github.com/carmipa/Advanced_Business_Development_with.NET_CP_1SEM/tree/main/cp5)

---

### 📌 Objetivo
Evoluir a API da locadora construída nos CPs anteriores adicionando **reserva em tempo real**, **pagamentos**, **observabilidade completa** (logs estruturados, métricas e traces) e **boas práticas de arquitetura** (Clean Architecture + CQRS/Validation).

---

### 🧩 Principais Funcionalidades
- **Reservas em tempo real** com *hold* temporário do veículo (TTL)  
- **Pagamentos** (simulação) com estados: `Pending → Authorized → Captured → Refunded`  
- **Cancelamento e reembolso** com regras de negócio e janelas de tempo  
- **Disponibilidade** por período (datas/horários) e filial  
- **Observabilidade**: Serilog (JSON), OpenTelemetry (traces/metrics/logs), Swagger/OpenAPI  
- **Segurança**: JWT (Bearer), perfis `admin` e `user`  
- **Validações** robustas (FluentValidation) e notificações de domínio  

---

### 🏗️ Arquitetura (Clean Architecture)
- **Domain** → Entidades, Value Objects, eventos de domínio  
- **Application** → Casos de uso (CQRS com MediatR), DTOs, validações  
- **Infrastructure** → EF Core, Repositórios, Migrations, Serilog, OTel exporters  
- **WebApi** → Endpoints (Minimal API/Controllers), Auth, Swagger  

---

### 🛠️ Tecnologias
`.NET 8`, `ASP.NET Core`, `EF Core 8`, `PostgreSQL/SQL Server`, `Medi