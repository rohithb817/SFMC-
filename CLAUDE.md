# CLAUDE.md — AI Assistant Guide for SFMC-

## Project Overview

**Repository:** SFMC- (Salesforce Marketing Cloud)
**Status:** Initial setup — this is a new repository with no source code yet.

This project is related to Salesforce Marketing Cloud (SFMC). As the codebase evolves, this document should be updated to reflect the current architecture, conventions, and workflows.

## Repository Structure

```
SFMC-/
├── CLAUDE.md          # This file — AI assistant guide
└── (no source code yet)
```

> **Note:** Update this section as directories and files are added (e.g., `src/`, `config/`, `tests/`, `docs/`).

## Technology Stack

> To be documented once the project is initialized with a framework and dependencies.

<!-- Example entries to fill in:
- **Language:** TypeScript / JavaScript / Python / Java
- **Framework:** Node.js / React / Angular / SSJS (Server-Side JavaScript for SFMC)
- **Build Tool:** Webpack / Vite / Gradle
- **Package Manager:** npm / yarn / pnpm
- **Testing:** Jest / Mocha / Pytest
- **Linting:** ESLint / Prettier
-->

## Development Setup

### Prerequisites

> Document required tools, SDKs, and environment setup here once established.

### Installation

```bash
# To be documented once package.json or equivalent is added
```

### Running Locally

```bash
# To be documented
```

## Build & Test Commands

> Add commands here as they are defined in package.json or build scripts.

<!-- Example:
```bash
npm install          # Install dependencies
npm run build        # Production build
npm run dev          # Development server
npm test             # Run tests
npm run lint         # Run linter
npm run lint:fix     # Auto-fix lint issues
```
-->

## Key Conventions

### Code Style

- Follow the project's linter and formatter configuration once established.
- Keep commits small and focused on a single change.
- Write descriptive commit messages in imperative mood (e.g., "Add email template parser").

### Branching Strategy

- Feature branches should follow the pattern: `feature/<description>`
- Bug fix branches: `fix/<description>`
- Always create pull requests for review before merging to `main`.

### SFMC-Specific Guidelines

- **AMPscript:** If using AMPscript in email templates or landing pages, keep logic minimal and well-commented.
- **SSJS (Server-Side JavaScript):** Follow standard JavaScript conventions. Note that SFMC SSJS uses an older ECMAScript version — avoid modern ES6+ syntax unless using a transpiler.
- **Data Extensions:** Document any Data Extension schemas used by the project.
- **API Integrations:** When working with SFMC REST/SOAP APIs, store credentials in environment variables — never commit secrets.

## Architecture

> Document the high-level architecture, data flow, and key components here once the project takes shape.

## Environment Variables

> List required environment variables here. Never commit actual secrets.

<!-- Example:
| Variable | Description | Required |
|----------|-------------|----------|
| `SFMC_CLIENT_ID` | SFMC API client ID | Yes |
| `SFMC_CLIENT_SECRET` | SFMC API client secret | Yes |
| `SFMC_AUTH_URL` | SFMC authentication endpoint | Yes |
| `SFMC_SUBDOMAIN` | SFMC account subdomain | Yes |
-->

## AI Assistant Instructions

When working in this repository, AI assistants should:

1. **Read before modifying** — Always read a file before making changes. Understand context first.
2. **Respect existing patterns** — Follow the conventions already established in the codebase.
3. **No secrets in code** — Never hardcode API keys, passwords, or tokens. Use environment variables.
4. **Test changes** — Run the test suite after making changes. If no tests exist for the area you changed, note that tests should be added.
5. **Keep CLAUDE.md updated** — When adding significant new features, directories, or changing workflows, update this file.
6. **Minimal changes** — Make only the changes requested. Don't refactor surrounding code unless asked.
7. **Security first** — Be aware of OWASP top 10 vulnerabilities. Validate inputs, sanitize outputs, and use parameterized queries.

## Updating This File

This CLAUDE.md should be updated when:
- The project is initialized with a framework or build tool
- New directories or major files are added
- Development workflows change (CI/CD, deployment, etc.)
- New conventions are established by the team
- Dependencies with special usage patterns are added
