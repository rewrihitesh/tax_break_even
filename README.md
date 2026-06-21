# tax-agent

AI-assisted Indian Income Tax Filing Agent.

This repository is being shaped around a human-in-the-loop tax filing workflow
for resident individuals, starting from official tax documents and taxpayer
uploads, then using deterministic rules for eligibility, validation, and tax
calculation.

The highest-priority project document is [docs/PROJECT_SCOPE.md](docs/PROJECT_SCOPE.md).
Product, architecture, research, and implementation decisions should derive from
that scope.

## Current status

The project is in the scoping and research phase. The new project structure is
in place for:

- `agent/`
- `backend/`
- `frontend/`
- `tests/`
- `datasets/`
- `docs/`

The existing tax calculation utilities remain in their original folders for now
and can be folded into the backend later once research clarifies the deterministic
rule-engine design.

---

## Important notice

- **This repo is licensed under AGPL-3.0-or-later.** See the LICENSE file in
the repo root.

- **This repo is distributed in the hope that it will be useful, but WITHOUT
ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
FOR A PARTICULAR PURPOSE.**

- **NOBODY else but you, and ONLY you, are responsible for your ITR filing.**

- This is an auditable open-source repo. **Your use of this repo implies you
understand the code and you have nobody else to blame.**

- Please open PRs whenever you can so that the code improves for everyone.

---
