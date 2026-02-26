---
name: phoenix-reborn
description: "Auto-resurrección y evolución post-fallo."
metadata:
  {
    "openclaw": {
      "emoji": "🔄",
      "version": "0.1.0",
      "author": "smouj"
    }
  }
---

# Phoenix Reborn

## Purpose
Sistema de auto-recuperación que detecta fallos en la ejecución de skills, analiza causas raíz mediante meta-learning ligero y propone/ejecuta retries con estrategia mejorada.

## Scope
- Execute this skill when tasks match this domain.
- Keep actions measurable and reversible.
- Prefer local-first execution and minimal permissions.

## Inputs expected
- Goal/intention in plain language
- Optional constraints (time/cost/privacy)
- Optional files/URLs needed for context

## Outputs
- Brief execution plan
- Step-by-step actions performed
- Verification checks
- Rollback/recovery notes

## Standard workflow
1. Validate scope and constraints.
2. Build a minimal execution plan.
3. Execute in small safe steps.
4. Verify results with explicit checks.
5. Summarize outcome + next steps.

## Commands (reference)
```bash
# validation stub
printf "running phoenix-reborn checks...
"

# add project-specific command here
# ./scripts/phoenix-reborn.sh
```

## Guardrails
- Never expose secrets in logs or outputs.
- Avoid destructive actions without explicit confirmation.
- Fail safely and report actionable diagnostics.

## Installation notes
- No external dependency is required for the documentation skeleton.
- Add dependencies in this section when implementation starts.

## Test checklist
- [ ] Happy path validated
- [ ] Error path validated
- [ ] Idempotency checked
- [ ] Security constraints verified

## Changelog
- 0.1.0: Initial structure, purpose, workflow and guardrails.
