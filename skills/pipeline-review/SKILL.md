---
name: pipeline-review
description: Analiza la salud del pipeline comercial de Sisteco — prioriza deals, detecta riesgos y genera plan semanal de accion. Usar al hacer revision semanal de pipeline, decidir en que oportunidades enfocarse, detectar deals estancados, o auditar problemas de higiene. Marca: Sisteco.
argument-hint: "<segmento o ejecutivo> o pega el CSV/lista de deals"
---

# Pipeline Review — Sisteco

Analiza la salud del pipeline comercial, prioriza deals y entrega recomendaciones accionables sobre donde enfocarse esta semana.

## Uso

```
/pipeline-review [segmento o ejecutivo]
```

## Como funciona

STANDALONE (siempre funciona):
- Sube CSV exportado de tu CRM (Apollo, HubSpot, etc.)
- O pega / describe tus deals en formato libre
- Health check: detecta deals estancados y en riesgo
- Priorizacion: rankea deals por impacto y probabilidad de cierre
- Auditoria de higiene: datos faltantes, fechas malas, single-threaded
- Plan semanal de accion

SUPERCHARGED (con herramientas conectadas):
- CRM conectado: extrae pipeline automaticamente
- Email/calendario: reuniones pendientes por deal
- Historial de actividad para scoring de engagement

## Analisis que entrego

### 1. Health check
- Deals sin actividad +7 dias -> alerta amarilla / +14 dias -> alerta roja
- Deals con un solo contacto (single-threaded) -> riesgo alto
- Fechas de cierre en el pasado o sin fecha -> higiene
- Etapas atascadas (mismo estado +2 semanas)

### 2. Top 3 deals de la semana
Con justificacion: mayor impacto en revenue / mayor probabilidad de cierre rapido / deal en riesgo recuperable.

### 3. Plan de accion semanal
Tabla: deal | accion concreta | objetivo | responsable | fecha

### 4. Alerta de higiene
Lista de deals que necesitan limpieza en CRM antes del viernes.

## Contexto Sisteco

- Ciclo de venta: consultoria ICM a empresas medianas chilenas
- Tomadores de decision: gerentes generales, gerentes de operaciones, duenos
- Metodologia: diagnostico antes de propuesta — nunca venta directa de plataforma
- Nunca inventar ticket promedio u otras metricas no documentadas

## Formato de salida

Reporte ejecutivo en espanol, directo, sin relleno:
1. Estado del pipeline (3 lineas)
2. Top 3 deals de la semana
3. Alertas de riesgo
4. Plan de accion (tabla)
5. Limpieza de CRM pendiente
