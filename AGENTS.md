# AGENTS.md — Guidance for AI coding assistants (DSOLVE 2026)

DSOLVE 2026 **permits** AI coding assistants, generative models, and design tools
as development aids — but participants must be able to **explain, defend, and
justify** all code, architecture, and design choices. This file helps your AI
assistant produce code that is clean, explainable, and judge-friendly.

> Keep this file if you use AI during the hackathon. Delete it if you don't.

---

## Context

- **Repo purpose:** Hackathon submission template for **DSOLVE 2026**
  (DRISHTI, College of Engineering Trivandrum). Each team forks this repo and
  turns it into their product.
- **Event format:** 36-hour physical hackathon (Thu 6 PM → Sat 6 AM).
- **Submission:** Public GitHub repo + >30s pitch video + 3–5 min live demo
  + technical Q&A.

## Conventions every team must follow

1. **No secrets in code.** Never write real API keys, tokens, passwords, or
   connection strings into source or commit them. Use `.env` + `.env.example`.
2. **Explainable code.** Favor small, well-named functions over clever one-liners.
   Every critical piece (especially AI/ML) must be possible to explain in a Q&A.
3. **Repo hygiene.** Never commit dependency folders, build output, `.env`, or
   logs (see `.gitignore`). Keep commits clean and meaningful throughout the 36 hours —
   don't dump everything in one giant commit.
4. **Stack freedom.** Teams choose their own stack. Match the stack the team has
   chosen — check `backend/` and `frontend/` READMEs before generating code.
5. **Documentation first.** `README.md` §8 (Getting Started) must be accurate and
   reproducible from a fresh clone.

## What to do when a participant asks you to write code

1. Explore the existing repo structure first — don't invent unrelated structure.
2. If a frontend/backend stack exists, follow its conventions (framework, linting,
   file layout).
3. Prefer to add tests for non-trivial logic, and confirm lint/type-check commands
   actually exist before running them.
4. Do **not** add unrequested boilerplate, dependencies, or README sections.
5. When handling images/media (Problem 1, 4, 5), respect privacy/HIPAA-style
   sensitivity: never hardcode or log patient data.

## Commands

Commands are **not** listed here because each team picks its own stack. Once the
stack is chosen, document the real commands (install, run, test, lint, build) in
`backend/README.md` and `frontend/README.md`, and make sure the steps in
`README.md` §8 (Getting Started) can be run from a fresh clone. Before running any
test/lint/build command during development, confirm it actually exists for the
team's chosen stack.

## Submission-time AI checklist

- [ ] Every team member can explain each significant block of code.
- [ ] Architecture decisions documented in `docs/architecture.md`.
- [ ] Third-party AI models/APIs used are allowed (open-source or public).
- [ ] Nothing in the repo is pre-built from before the hackathon.