# 📘 Dev Log

## 📅 2025-07-21 – GitHub Profile Setup

### ✅ What I did:

-   Created and published my personal GitHub profile README (`zrdt80/zrdt80`)
-   Added biography, contact links (email, LinkedIn, Discord), and badge-based tech stack
-   Included GitHub stats and project list section (Vault, BeeTrack, SkillMatch AI)
-   Set up profile visibility and pinned repositories

### 🧠 Notes:

-   Kept content consistent in English for professionalism and portability
-   Markdown rendering tested across light/dark themes

### 🛠 Tools used:

-   shields.io for tech badges
-   GitHub Stats API & Streak generator
-   Manual Markdown formatting in VS Code

### 🔜 Next step:

-   Initialize `dev-notes` repository and project structure

## 📅 2025-07-22

-   Created repository `dev-notes`
-   Defined folder structure and base files
-   Prepared to start project `Vault` tomorrow
-   Set up README, snippets and notes sections

## 📅 2025-07-23

### ✅ Milestones Completed:
- Created project `Vault` (secret manager) repo
- Implemented Flask backend with:
  - JWT Auth
  - SQLAlchemy ORM
  - CRUD for secrets
- Protected routes with decorators
- Encrypted secret values in DB
- Created unit tests:
  - Auth flow
  - CRUD (create, patch, delete)
  - Negative paths: auth required, owner-only, etc.
- Refactored tests for modularity
- Bootstrap README.md and all reference docs

---

### 🔧 Next Steps:
- Add Docker setup
- Setup Postgres instead of SQLite
- Optional: Add CLI / basic frontend
