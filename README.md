# 🔄 Phoenix Reborn

<p align="center">
  <img src="https://img.shields.io/badge/Skill-Phoenix%20Reborn-111827?style=for-the-badge&logo=github" alt="Phoenix Reborn banner" />
</p>

<p align="center">
  <a href="./README.md"><img src="https://img.shields.io/badge/README-English-1f6feb?style=for-the-badge" alt="English"></a>
  <a href="./README.es.md"><img src="https://img.shields.io/badge/README-Español-c92a2a?style=for-the-badge" alt="Español"></a>
</p>

## Overview
Self-recovery engine with checkpoint restore and lightweight meta-learning retries.

## Purpose
Auto-resurrección y evolución: si el agente falla/crash/olvida contexto crítico, revive de backups locales + analiza logs de fallos para mutar su propio prompt base y skills (meta-learning ligero). Evita loops de muerte repetida en tareas largas.

## Installation
```bash
git clone https://github.com/smouj/Phoenix-Reborn.git
cd Phoenix-Reborn
cat SKILL.md
```

## Architecture (understanding)
```mermaid
flowchart LR
  A[Input] --> B[Validate scope]
  B --> C[Plan safe steps]
  C --> D[Execute]
  D --> E[Verify]
  E --> F[Report]
```

## Status
Initiating

## Difficulty
Alta
