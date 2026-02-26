---
name: phoenix-reborn
description: "🔄 Auto-resurrección y evolución post-fallo."
metadata:
  {
    "openclaw": {
      "emoji": "🔄",
      "version": "0.2.0",
      "author": "smouj",
      "lang_default": "en"
    }
  }
---

# 🔄 Phoenix Reborn

## Purpose
Sistema de auto-recuperación que detecta fallos en la ejecución de skills, analiza causas raíz mediante meta-learning ligero y ejecuta retries con estrategia mejorada.

## Tags
- security
- reliability
- automation
- openclaw-skill

## Execution contract
1. Validate request and constraints.
2. Generate minimal safe plan.
3. Execute in reversible steps.
4. Verify with explicit checks.
5. Return concise summary + next actions.

## Inputs expected
- Goal
- Constraints (time/cost/privacy)
- Optional files/URLs

## Outputs
- Plan
- Actions executed
- Verification results
- Rollback notes

## Guardrails
- Never expose secrets.
- No destructive operation without explicit confirmation.
- Fail safe with actionable diagnostics.

## Commands
```bash
# Placeholder entrypoint
printf "phoenix-reborn: validate -> execute -> verify\n"
```

## Test checklist
- [ ] Happy path
- [ ] Error handling
- [ ] Idempotency
- [ ] Guardrails respected
