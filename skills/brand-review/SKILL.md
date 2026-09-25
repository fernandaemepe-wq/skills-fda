---
name: brand-review
description: Revisa contenido contra la guia de voz y los pilares de la marca antes de publicar — detecta desviaciones por severidad con correcciones especificas antes/despues. Usar al revisar un borrador antes de que salga, al auditar copy para consistencia de voz y terminologia, o al detectar claims sin respaldo. Aplica a Sisteco, MicroSec y Marketing FDA.
argument-hint: "<contenido a revisar> [marca: Sisteco | MicroSec | FDA]"
---

# Brand Review — FDA

Revisa contenido de marketing contra la guia de voz, pilares de contenido y estandares de mensajeria de la marca. Detecta desviaciones y entrega sugerencias de mejora especificas.

## Trigger

El usuario pide revisar, chequear o dar el visto bueno a una pieza de Sisteco, MicroSec o FDA.

## Marca

Identificar por contexto o preguntar:
- **Sisteco** → revisar contra cerebro-sisteco.md
- **MicroSec** → revisar contra cerebro-microsec.md
- **FDA** → revisar contra manifiesto-fda.md

Si la marca no es obvia → preguntar antes de revisar.

## Dimensiones de evaluacion

### Voz y tono
- Coincide con los atributos de voz del cerebro de la marca?
- El tono es apropiado para el tipo de contenido y audiencia?
- Hay cambios de voz inconsistentes?

### Terminologia y vocabulario
- Se usan correctamente los terminos propios de la marca?
- Aparece alguna palabra prohibida?
- El nivel de jerga es apropiado? (DUA: claro sin perder profundidad)

### Claims y metricas
- Toda cifra o promesa tiene respaldo en el cerebro de la marca?
- Claims sin fuente documentada = BLOQUEANTE siempre.

### Mezcla de voces
- Lo que suena a Sisteco podria confundirse con MicroSec? Si si -> rehacer.
- La pieza tiene identidad clara de marca o es generica?

## Formato de salida

**Veredicto:** PUBLICABLE / PUBLICABLE CON AJUSTES / REHACER

**Hallazgos:**

BLOQUEANTE (no publicar hasta resolver):
- [problema + correccion exacta]

RECOMENDADO (mejorar si hay tiempo):
- [problema + sugerencia]

NOTA (no bloquea):
- [observacion menor]

**Resumen:** una linea con el veredicto y el ajuste mas urgente.

## Reglas duras

- Claim sin fuente en el cerebro -> siempre BLOQUEANTE
- Voz que podria ser de cualquier marca -> siempre REHACER
- No dar elogios de relleno — veredicto directo
