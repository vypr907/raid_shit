---
tags: [dev-project, software]
---

# raid_roster — Software Side-Project Status

This is a **software project**, not RAID game knowledge — it's a personal Flask web app for tracking your champion roster, referenced across several of the migrated ChatGPT conversations. Kept separate from [[../05 History/Historical Knowledge Archive|Historical Knowledge Archive]] so game strategy and dev-project history don't get tangled together.

## Original plan (Sept 2025 conversations)
Decided **Flask over Streamlit**, explicitly to build DevOps portfolio value. Scoped an ambitious architecture:
- **DB:** SQLAlchemy ORM over **AWS RDS PostgreSQL**, with **Flask-Migrate/Alembic** for schema versioning
- **Champion schema:** `id, name, image, faction, rarity, affinity, level, rank, ascension, perfect, role, is_favourite, stat_HP, stat_ATK, stat_DEF, stat_SPD, stat_CCR, stat_CDMG, stat_RES, stat_ACC, stat_IGNDEF` plus a `Team` model (many-to-many via `teams`/`team_champions`/`champions`)
- **Manual CLI seeding** (`python run.py seed`) rather than an HTTP `/seed` route, for security
- **Full AWS stack planned:** Docker, ECR, ECS/Fargate (favored over Elastic Beanstalk), S3 for assets, Lambda/API Gateway for an AI layer, Secrets Manager, VPC/security groups, CloudWatch, GitHub → CodePipeline → CodeBuild CI/CD
- An RDS PostgreSQL instance was actually created (`raidcoach-db.concauk0gml1.us-east-1.rds.amazonaws.com`), and Flask-Migrate/Alembic was adopted in principle. A local `raid_roster/` connection to that RDS instance had at least one failed attempt (timeout on port 5432 — likely a security-group/public-access issue, never resolved in the conversations).

## What's actually in the repo today
The current code is a **much simpler, local-only rebuild** — it doesn't match the plan above:
- Plain **`sqlite3`** (no SQLAlchemy, no Postgres/RDS connection, no Flask-Migrate) — DB file is `roster.db`
- Simpler schema: `id, name, role, affinity, level, notes, rarity, affiliation, rank, awoken, perfect` (no `image`, `ascension`, `is_favourite`, or any `stat_*` fields; `affiliation` where the plan said `faction`; adds `notes` and `awoken`)
- Three tables: `champions`, `tags`, `champion_tags` (many-to-many tagging, matching the original "tag a champion for squads/events/dungeons" requirement)
- Three routes: `/` (list + add form), `/add`, `/tags` (manage tags), plus delete routes for both
- Latest git commit message ("adding Flask-Migrate...") describes intent that isn't reflected in `app.py` yet — Flask-Migrate isn't imported or configured anywhere in the current code

**This looks like the project was restarted at a smaller scope** (a working local tracker first) rather than abandoned — the many-to-many tagging idea from the original plan survived, but the AWS/PostgreSQL portfolio ambitions haven't been carried over yet.

## Bug found & fixed (Sept 2, 2026)
`init_db()`'s `tags` table had a trailing comma after `name TEXT UNIQUE,` before the closing paren — invalid SQLite syntax that would throw `sqlite3.OperationalError` the first time the app ran and tried to create tables. Also fixed a stray `awoken iNTEGER` casing typo (harmless — SQLite type names are case-insensitive — but cleaned up for readability). Both are fixed in `app.py` as of this note; verified by running the three `CREATE TABLE` statements against a test database successfully.

## Open questions for next time
- Is the AWS/RDS/SQLAlchemy direction still the goal (for the DevOps portfolio value), or has the scope intentionally settled on local SQLite for now?
- `static/boostrap.min.css` is an empty file (0 bytes) — the HTML templates reference Bootstrap via CDN link instead, so this may be a leftover/unused file.
- No masteries or blessings fields exist in the schema at all — flagged as unresolved in the original design conversation too.
