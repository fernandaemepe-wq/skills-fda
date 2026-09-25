---
name: call-prep
description: Prepara para una llamada de ventas con contexto de la cuenta, investigacion de asistentes y agenda sugerida. Funciona solo con input del usuario y busqueda web, mejora con CRM. Trigger: "preparame para mi llamada con [empresa]", "call prep [empresa]". Marca: Sisteco.
argument-hint: "<empresa o contacto>"
---

# Call Prep -- Sisteco

Preparacion completa para llamadas comerciales de Sisteco.

## Como funciona

STANDALONE:
- Tu me dices: empresa, tipo de reunion, quienes asisten
- Buscada web: noticias recientes, liderazgo, movimientos
-Output: brief con agenda y preguntas

SUPERCHARGED (con herramientas conectadas):
- CRM: historial, contactos, oportunidades
- Email: hilos recientes, preguntas abiertas
- Calendario: auto-encontrar la reunion

## Que necesito

- Nombre de la empresa
- Tipo de reunion (descubrimiento, demo, propuesta, negociacion)
- Quien asiste (si lo sabes)
- Cualquier contexto relevante

## Output

```
# Prep Reunion: [Empresa]

Reunion: [Tipo] — [Fecha/hora si se sabe]
Asistentes: [Nombres con cargos]
Tu objetivo: [Que quieres lograr]

---

## Snapshot de la cuenta
| Campo | Valor |
|-------|-------|
| Empresa | [Nombre] |
| Industria | [Industria] |
| Tamano | [Empleados/indicadores tamano] |
| Estado | [Nuevo prospecto / activo / cliente] |
| Ultimo contacto | [Fecha y resumen] |

---

## Personas en la reunion
[Nombre] - [Cargo]
- Background: [Historial]
- Rol en toma de decision: [Decisor, champion, evaluador]
- Punto de conversacion: [algo personal/profesional para mencionar]

---

## Contexto e historial
- [Punto clave de interacciones anteriores]
- [Compromisos abiertos o acciones pendientes]
- Noticias recientes de [Empresa]: [noticia + por que importa]

---

## Agenda sugerida
1. [Inicio] - Referenciar ultima conversacion
2. [Tema 1] - [Pregunta de descubrimiento o valor]
3. [Tema 2] - [Abordar objecion o interes]
4. [Tema 3] - [Demo / propuesta / etc]
5. [Siguientes pasos] - Proponer seguimiento concreto

---

## Preguntas de descubrimiento
1. [Sobre situacion actual]
2. [Sobre pain points prioridades]
3. [Sobre proceso de toma de decision]
4. [Sobre criterios de exito]
5. [Sobre otros actores]

---

## Objeciones probables
| Objecion | Respuesta sugerida |
|----------|-------------------|
| [Objecion probable por etapa] | [Como abordarla] |

---

## Despues de la reunion
Correr *call-summary* para extraer acciones y redactar follow-up.
```

## Contexto Sisteco

- Metodologia ICM: diagnostico antes que propuesta
- Audiencia: empresas medianas chilenas
- Tomadores de decision: gerentes generales, directores de operaciones
- Nunca vender plataforma directamente: la conversacion parte del diagnostico
- Nunca inventar metricas no documentadas
- Cyclo de venta: consultoria ICM (6 semanas)
