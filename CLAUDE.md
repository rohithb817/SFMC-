# CLAUDE.md — AI Assistant Guide for SFMC-

## Project Overview

**Repository:** SFMC- (Salesforce Marketing Cloud)
**Status:** Initial setup — no source code yet, scaffolding only.

This project is related to Salesforce Marketing Cloud (SFMC). This document should be updated as the codebase evolves.

## Repository Structure

```
SFMC-/
├── CLAUDE.md          # This file — AI assistant guide
└── (no source code yet)
```

Update this section as directories and files are added (e.g., `src/`, `config/`, `tests/`, `docs/`).

## Technology Stack

To be documented once the project is initialized with a framework and dependencies. Likely candidates given the SFMC context:

- **SSJS (Server-Side JavaScript):** SFMC's native scripting language (older ECMAScript — avoid ES6+ without a transpiler)
- **AMPscript:** SFMC's proprietary scripting language for emails and landing pages
- **Node.js / Python:** Common choices for SFMC API integration tooling

## Development Setup

No build tooling or dependencies are configured yet. Update this section when `package.json` or equivalent is added.

## Build & Test Commands

No build or test commands defined yet. Update this section when scripts are added.

## Key Conventions

### Code Style

- Follow the project's linter and formatter configuration once established.
- Keep commits small and focused on a single change.
- Write descriptive commit messages in imperative mood (e.g., "Add email template parser").

### Branching Strategy

- Feature branches: `feature/<description>`
- Bug fix branches: `fix/<description>`
- Always create pull requests for review before merging to `main`.

### SFMC-Specific Guidelines

- **AMPscript:** Keep logic minimal and well-commented.
- **SSJS:** Uses an older ECMAScript version — avoid modern ES6+ syntax unless using a transpiler.
- **Data Extensions:** Document any Data Extension schemas used by the project.
- **API Integrations:** Store SFMC REST/SOAP API credentials in environment variables — never commit secrets.

## Environment Variables

No environment variables defined yet. When SFMC API integration is added, expect variables like:

| Variable | Description |
|----------|-------------|
| `SFMC_CLIENT_ID` | SFMC API client ID |
| `SFMC_CLIENT_SECRET` | SFMC API client secret |
| `SFMC_AUTH_URL` | SFMC authentication endpoint |
| `SFMC_SUBDOMAIN` | SFMC account subdomain |

Never commit actual secret values.

## AI Assistant Instructions

1. **Read before modifying** — Always read a file before making changes.
2. **Respect existing patterns** — Follow conventions already in the codebase.
3. **No secrets in code** — Use environment variables for all credentials.
4. **Test changes** — Run the test suite after changes. Note when tests should be added.
5. **Keep CLAUDE.md updated** — Update this file when adding features, directories, or changing workflows.
6. **Minimal changes** — Only make what's requested. Don't refactor unrelated code.
7. **Security first** — Validate inputs, sanitize outputs, use parameterized queries.

## Updating This File

Update CLAUDE.md when:
- The project is initialized with a framework or build tool
- New directories or major files are added
- Development workflows change (CI/CD, deployment, etc.)
- New conventions are established by the team
- Dependencies with special usage patterns are added
