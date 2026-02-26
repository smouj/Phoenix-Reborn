---
name: Phoenix Reborn
description: "🔄 Self-recovery engine with checkpoint restore and lightweight meta-learning retries."
when: "When a user request matches phoenix-reborn capabilities or requires this domain-specific workflow."
examples:
  - "Run Phoenix Reborn for this task"
  - "Apply Phoenix Reborn to solve this workflow"
metadata:
  openclaw:
    requires: ["fs_read", "fs_write", "shell_exec", "memory_search"]
  safety_level: high
  version: "1.0.0"
  author: "smouj"
  tags: ["phoenix-reborn", "automation", "openclaw-skill"]
---

# 🔄 Phoenix Reborn

## Propósito
Auto-resurrección y evolución: si el agente falla/crash/olvida contexto crítico, revive de backups locales + analiza logs de fallos para mutar su propio prompt base y skills (meta-learning ligero). Evita loops de muerte repetida en tareas largas.

## Cómo usar / Instrucciones núcleo
1. Primero piensa en alcance, riesgo y coste.
2. Luego valida inputs y dependencias mínimas.
3. Ejecuta en pasos pequeños y reversibles.
4. Verifica resultado con checks explícitos.
5. Si hay error, falla seguro y reporta causa + próximo paso.

## Security & Safety Guidelines
Nunca ejecutes código sospechoso sin sandbox. Reporta riesgos al usuario. No envíes datos sensibles fuera del entorno local.

## Herramientas requeridas
- fs_read
- fs_write
- shell_exec
- memory_search

## Flujos de ejemplo
- Entrada -> validación -> plan -> ejecución -> verificación -> reporte.
- Reintento controlado con rollback si falla.

## Casos límite y manejo de errores
- Input incompleto: pedir datos mínimos.
- Dependencia ausente: degradar en modo seguro.
- Error persistente: detener, registrar y escalar.
