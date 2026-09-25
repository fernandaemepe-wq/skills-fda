---
id: content-repurposer
name: Content Repurposer
version: 1.0.0
category: marketing
agent: marketing
trigger: "\\f repurpose content"
requires: [claude-api, twitter-api, linkedin-api]
type: code-assisted
description: Transforma contenido largo en multiples formatos para distribucion multicanal
---

# SOP: Content Repurposer

## Objetivo
Tomar contenido largo (transcripcion de video, podcast, articulo) y generar en paralelo: hilo de Twitter/X, post de LinkedIn y borrador de newsletter.

## Entrada
- Transcripcion o texto largo (minimo 500 palabras)
- Fuente original (URL del video, titulo del podcast, etc.)
- Opcional: audiencia objetivo
- Opcional: CTA deseado por canal

## Proceso

### Paso 1: Analizar Contenido Fuente
- Identificar tema principal y subtemas
- Extraer 5-7 puntos clave / insights
- Identificar citas memorables o datos impactantes
- Determinar el "hot take" o angulo unico del autor

### Paso 2: Generar Hilo de Twitter/X
Estructura del hilo (7-12 tweets):

- Tweet 1 (Hook): declaracion provocativa, max 200 chars, terminar con "Hilo:"
- Tweets 2-N: un punto clave por tweet, max 280 chars
- Tweet final: resumen + CTA

### Paso 3: Generar Post de LinkedIn
- Primera linea: hook impactante
- Cuerpo: 5-8 parrafos cortos con saltos generosos
- Incluir anecdota personal
- Cierre: pregunta abierta para engagement
- 3-5 hashtags al final
- Largo ideal: 1200-1500 caracteres

### Paso 4: Generar Borrador de Newsletter
- 3 variantes de subject line
- Preview text 40-90 chars
- Intro personal + 3 secciones con headers
- CTA al contenido original
- Largo ideal: 600-900 palabras

## Reglas FDA
- NUNCA inventar citas o datos que no esten en el contenido original
- Adaptar tono a cada plataforma (Twitter = directo, LinkedIn = profesional, Newsletter = editorial)
- Por defecto en espanol (es-CL)
- LinkedIn optimo: 1300 chars (visible sin "ver mas")
- Si el original es en ingles, preguntar si traducir o mantener
- Verificar que no hay mezcla de voces entre Sisteco y MicroSec

## Formato de Salida

Json structurado con:
- source: titulo, url, word_count
- outputs.twitter_thread: array de tweets
- outputs.linkedin_post: texto + hashtags
- outputs.newsletter: subjects, preview, body

## Referencias
- Incluye script.js con arquitectura de sub-agentes para n8n
