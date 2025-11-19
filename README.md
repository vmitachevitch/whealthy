# Whealthy

Whealthy is an open-source platform for personal and wealth management.

The project emphasizes modularity, transparency, and portability with a modern, multi-user, and extensible architecture.

---

## 🚀 Objectifs

- Centraliser les transactions, budgets, investissements et indicateurs patrimoniaux.
- Fournir un tableau de bord clair et personnalisable.
- Offrir une expérience multi-plateforme (Web, Desktop, Android).
- Proposer une base technique solide : API Python, PostgreSQL, Next.js, Docker.
- Permettre une gestion multi-utilisateurs avec rôles et règles de visibilité.
- Faciliter les imports (CSV, API bancaires, flux réguliers…).

---

## 🏗️ Architecture

### Backend
- **Python**
- **FastAPI**
- **PostgreSQL**

- `pg_trgm` for duplicate detection
- TimescaleDB (optional) for legacy time series
- Authentication:

- Local Auth
- JWT
- TOTP (2FA)
- REST API + Webhooks

### Frontend
- **Next.js (App Router)**
- **React Query**
- **TailwindCSS + shadcn/ui**
- **Nivo / ECharts** for data visualization
- Zustand (optional) for lightweight state management

### Documentation
- **MkDocs Material**
- Multi-language via the **i18n** plugin
- GitHub Pages deployment

### Containerization
- Docker + Docker Compose to simplify deployment

- Isolated images: frontend, backend, database

---

## 📦 Main Features

### 🔐 Authentication
- Account creation
- Access rights management (read/edit)
- Password reset via email
- Optional 2FA

### 📊 Dashboard
- Account balance
- Monthly balance
- Net worth trend
- Monthly summary
- Projected expenses and income
- Breakdown by category (pie chart)

### 💸 Transactions
- Filterable history
- Manual addition
- CSV import (multi-format)
- Import via banking APIs
- Duplicate detection
- Expense reports (with rules)

### 🎯 Budgets
- List of "piggy bank" type budgets
- Amount collected / remaining
- % progress
- Optional inflation
- Edit, delete

### 📈 Investments
- Recovery via Stock Market APIs
- Top 3
- Portfolio Pie Chart
- Invested/Current Value
- ROI
- Notifications (optional)

### ⚙️ Administration
- User Management
- Category Management
- Global Settings
- User Synchronization
- Home Assistant API (notifications)

---