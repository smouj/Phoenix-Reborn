# 🔄 Phoenix Reborn

<p align="center">
  <img src="https://img.shields.io/badge/Skill-Phoenix%20Reborn-111827?style=for-the-badge&logo=github" alt="Phoenix Reborn banner" />
</p>

<p align="center">
  <a href="./README.md"><img src="https://img.shields.io/badge/README-English-1f6feb?style=for-the-badge" alt="English"></a>
  <a href="./README.es.md"><img src="https://img.shields.io/badge/README-Español-c92a2a?style=for-the-badge" alt="Español"></a>
</p>

## Resumen
Auto-resurrección y evolución: si el agente falla/crash/olvida contexto crítico, revive de backups locales + analiza logs de fallos para mutar su propio prompt base y skills (meta-learning ligero). Evita loops de muerte repetida en tareas largas.

## Instalación
```bash
git clone https://github.com/smouj/Phoenix-Reborn.git
cd Phoenix-Reborn
cat SKILL.es.md
```

## Arquitectura de entendimiento
```mermaid
flowchart LR
  A[Entrada] --> B[Validar alcance]
  B --> C[Plan seguro]
  C --> D[Ejecutar]
  D --> E[Verificar]
  E --> F[Reportar]
```

## Estado
Iniciando

## Dificultad
Alta
