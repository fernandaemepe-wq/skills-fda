---
name: handoff
description: Compacta la sesion actual en un documento de traspaso para que otra sesion/agente continue el trabajo. Usar al cerrar una sesion sustantiva, cuando el contexto se agota, o antes de traspasar trabajo a otro agente.
argument-hint: "¿Para que se usara la proxima sesion?"
---

# Handoff -- Marketing FDA

Escribe un documento de traspaso que resume la sesion actual para que otra sesion pueda continuar sin necesitar este contexto.

## Contenido del documento

1. **Estado**: que se completo, que quedo a medias, que esta bloqueado (y por que).
2. **Decisiones cerradas**: marcadas como CERRADO para que la proxima sesion no las reabra.
3. **Proximos pasos**: accionables, en orden, con el primero listo para ejecutar.
4. **Skills recomendadas**: que skills deberia usar el agente que retome.
5. **Referencias**: NO duplicar contenido que ya vive en otros archivos. Referenciarlos por ruta o URL.

Si el usuario paso argumentos, son la descripcion del foco de la proxima sesion. Adaptar el documento a eso.

**Siempre eliminar:** API keys, passwords, tokens y datos personales antes de guardar.

## Donde guardar

| Destino | Para quien | Que incluye |
|---|---|---|
| `Dropbox/Marketing-FDA/_handoffs/<proyecto>/` | Agente que retoma | Handoff completo, tecnico |
| Vault (cristalizaciones) | Agentes + busqueda semantica | Digest de aprendizaje |
| Notion (solo si tiene impacto en el negocio) | Fer | Avance + decisiones pendientes |

## Formato de salida

```markdown
# Handoff: [Proyecto/Tema]
Fecha: [Fecha]
Foco proxima sesion: [Argumentos del usuario]

---

## Estado

**Completado:**
- [accion completada]
- [accion completada]

**A medias:**
- [tarea incompleta] -- [estado actual]

**Bloqueado:**
- [bloqueo] -- [por que]

---

## Decisiones CERRADAS
- CERRADO: [decision 1-- no reabrir]
- CERRADO: [decision 2]

---

## Proximos pasos (en orden)
1. [Primer paso, listo para ejecutar]
2. [Segundo paso]
3. [Tercer paso]

---

## Skills recomendadas para la proxima sesion
- `[Skill 1]` -- [por que]
- `[Skill 2]` -- [por que]

---

## Referencias
- [Nombre del archivo]: [ruta o URL]
```

## Reglas duras

- NUNCA incluir API keys, passwords, ni datos de leads personales
- NO replicar contenido que ya existe en Dropbox/proyecto/-- solo referenciarlo
- Si no hay impacto de negocio -- no publicar a Notion
- El primer paso siempre tiene que estar listo para ejecutar sin preguntas
