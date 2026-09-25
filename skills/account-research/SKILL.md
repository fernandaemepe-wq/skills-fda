---
name: account-research
description: Investiga una empresa o persona y obtiene intel de ventas accionable. Funciona solo con busqueda web, mejora con enriquecimiento o CRM. Trigger: "investiga [empresa]", "intel de [prospecto]", "quien es [nombre] en [empresa]".
argument-hint: "<empresa o persona>"
---

# Account Research -- Sisteco

Obtiene la imagen completa de cualquier empresa o persona antes del contacto. Funciona siempre con busqueda web, mejora con enriquecimiento y CRM conectados.

## Como funciona

STANDALONE:
- Perfil de la empresa: que hacen, tamano, industria
- Noticias recientes: financiamiento, cambios de liderazg[o, anuncios
-Necesitars de contratacion: senales de crecimiento
- Personas clave: equipo directivo
- Producto/servicio: que venden, a quien atienden

SUPERCHARGED:
- Enriquecimiento: emails verificados, org chart, stack
- CRM: historial previo, contactos ya en sistema

## Desencadenantes

- "investiga [empresa]"
- "intel de [empresa]"
- "quien es [nombre]"
- "dime sobre [empresa]"
- "preparame para llamar a [empresa]"

## Formato de salida

```
# Investigacion: [Empresa o Persona]
Fecha: [Fecha] | Fuentes: Web [+ Enriquecimiento] [+ CRM]

---

## ResUmen rapido
[2-3 oraciones: quienes son, por que podrian necesitar Sisteco, mejor angulo de contacto]

---

## Perfil de la empresa

| Campo | Valor |
|-------|-------|
| Empresa | |
| Sitio web | |
| Industria | |
| Tamano | |
| Ubicacion | |
| Fundada | |

### Que hacen
[Descripcion en 1-2 oraciones]

### Noticias recientes
- **[Titulon]** - [Fecha] - [Por que importa para Sisteco]

### Senales de contratacion
[# de roles abiertos yc que indican]

### Personas clave
[Nombre] - [Cargo]
- LinkedIn: [URL]
- Background: [Historial]
- Punto de conversacion: [algo relevante]

---

## Historial en Sisteco (si CRM conectado)

| Campo | Valor |
|-------|-------|
| Estado | [Nuevo / prospecto anterior / cliente] |
| Ultimo contacto | |
| Oportunidades anteriores | |
| Contactos existentes | |

---

## Senales de calificacion

Positivas:
- [Senal con evidencia]

Posibles riesgos:
- [Risesgo a verificar]

---

## Enfoque recomendado
**Mejor punto de entrada:** [Persona y por que]
**Angulo de apertura:** [Que mencionar primero]
**Preguntas de descubrimiento:**
1. [Pregunta contextual]
2. [Pregunta de pain point]
3. [Pregunta de proceso]
```
