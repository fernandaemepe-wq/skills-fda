---
id: meeting-to-actions
name: Meeting Notes to Action Items
version: 1.0.0
category: productivity
agent: workflow
trigger: "\\f meeting actions"
requires: [claude-api]
type: deterministic-text
description: Procesa transcripciones de reuniones y extrae informacion estructurada
---

# SOP: Meeting Notes to Action Items

## Objetivo
Transformar transcripciones de reuniones en informacion accionable estructurada.

## Entrada
- Transcripcion completa de una reunion (texto plano, .txt, .md, o pegado directo)
- Opcional: lista de participantes conocidos

## Proceso

### Paso 1: Identificar Participantes
- Extraer todos los nombres mencionados
- Asignar roles si son evidentes (cliente, proveedor, interno)

### Paso 2: Extraer Decisiones Tomadas
Buscar frases como: "decidimos", "acordamos", "vamos a", "queda definido"

### Paso 3: Extraer Tareas y Responsables
Para cada tarea:
- Descripcion
- Responsable (nombre asignado)
- Fecha limite (si se menciono)
- Prioridad (alta/media/baja, inferida del contexto)
- Dependencias

### Paso 4: Extraer Preguntas Abiertas
- Temas que quedaron sin resolver
- Items que requieren mas investigacion

### Paso 5: Extraer Datos de Contacto
- Telefonos, emails, URLs mencionados

### Paso 6: Generar Resumen Ejecutivo
- Resumen en 3-5 lineas
- Duracion estimada
- Proximo paso inmediato

## Formato de Salida

```json
{
  "meeting_summary": {
    "title": "string",
    "date": "ISO date si se menciona",
    "participants": ["nombre1", "nombre2"],
    "duration_estimate": "string",
    "executive_summary": "string"
  },
  "decisions": [{"description": "", "decided_by": "", "context": ""}],
  "action_items": [
    {
      "task": "string",
      "assignee": "string",
      "deadline": "ISO date o null",
      "priority": "alta|media|baja",
      "dependencies": []
    }
  ],
  "open_questions": [{"question": "", "raised_by": null, "context": ""}],
  "contact_info": [{"type": "phone|email|url", "value": "", "context": ""}],
  "next_steps": "string"
}
```

## Integraciones posibles

- Google Calendar: Crear evento si se detecto proxima reunion con fecha
- Todoist / Linear: Crear tarea por cada action item
- Email (Resend): Enviar resumen a participantes

## Reglas
- Si no se menciona fecha limite: dejar como null, no inventar
- Si no se puede determinar responsable: poner "Sin asignar"
- Inferir fechas relativas: "la proxima semana" > fecha concreta
- Distinguir compromisos firmes vs ideas sueltas
-NUNCA inventar informacion no presente en la transcripcion
