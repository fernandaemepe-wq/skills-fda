# Skills FDA — Agentes IA para Marketing FDA, Sisteco y MicroSec

> Skills de producción lista para agentes IA (Claude Code, Composio, Antigravity) aplicadas a marketing de contenidos, ventas B2B y ciberseguridad en el mercado chileno.

Este repositorio es parte del ecosistema **Marketing FDA** — el estudio de Fernanda Martínez Poblete.

---

## Marcas cliente

- **Sisteco** — ventas agénticas B2B, metodología ICM, Chile
- **MicroSec** — ciberseguridad y formación

## Skills incluidas

| Skill | Marca | Descripción |
|---|---|---|
| [`brand-review`](skills/brand-review) | Sisteco / MicroSec / FDA | Revisa contenido contra el cerebro de la marca antes de publicar |
| [`pipeline-review`](skills/pipeline-review) | Sisteco | Analiza salud del pipeline comercial y genera plan semanal de acción |
| [`performance-report`](skills/performance-report) | Sisteco / MicroSec / FDA | Genera reporte de métricas con análisis, wins/misses y recomendaciones |

---

## Instalación en Claude Code

```bash
mkdir -p .claude/skills
cp -r skills/brand-review .claude/skills/
cp -r skills/pipeline-review .claude/skills/
cp -r skills/performance-report .claude/skills/
```

---

*Basado en el catálogo [Open Agentic Skills](https://github.com/FMC1d/open-agentic-skills) de FMC1d, adaptado para el mercado chileno. MIT License.*
