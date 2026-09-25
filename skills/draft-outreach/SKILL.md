---
name: draft-outreach
description: Research a prospect then draft personalized outreach. Uses web research by default, supercharged with enrichment and CRM. Trigger with "draft outreach to [person/company]", "write cold email to [prospect]", "reach out to [name]".
---

# Draft Outreach

Research first, then draft. This skill never sends generic outreach - it always researches the prospect first to personalize the message. Works standalone with web search, supercharged when you connect your tools.

## Connectors (Optional)

| Connector | What It Adds |
|-----------|--------------|
| **Enrichment** | Verified email, phone, background details |
| **CRM** | Prior context, relationship history |
| **Email** | Create draft directly in inbox |

> **Sin connectors?** Web research funciona bien. Output texto del email para copiar.

---

## Ejecucion

### Paso 1: Investigar

Usar busqueda web para obtener:
- Quien es la persona (cargo, historial)
- Que hace la empresa
- Noticias recientes o trigger de contacto
- Hook de personalizacion

### Paso 2: Identificar Hook

Orden de prioridad:
1. Evento reciente (financiamiento, contratacion, noticia) -> mas oportuno
2. Conexion mutua
3. Contenido suyo (post, articulo, charla)
4. Iniciativa de la empresa
5. Pain point del rol

### Paso 3: Redactar

Estructura (AIDA):
```
SUBJECT: [personalizado, menos de 50 chars]

[Apertura: Hook personal basado en investigacion]

[Interes: Su problema/oportunidad en 1-2 oraciones]

[Prueba: Caso parecido en 1 oracion]

[CTA: pregunta clara y de bajo rozamiento]
```

Reglas de redaccion:
- Sin markdown (ni asteriscos ni negritas)
- Parrafos cortos (2-3 oraciones maximo)
- Espancl chileno, tuteo
- NO abrir con "Esperando que este email te encuentre bien" ni cliches
- NO fingir personalizacion generica ("Note que trabajas en [Empresa]" es obvio)

## Formato de salida

```
# Draft de Outreach: [Persona] en [Empresa]

Investigacion:
- Quien son: [Datos clave]
- Hook: [Razon de contacto hoy]
- Objetivo: [Que buscar]

---

SUBJECT: [Subject principal]

[Cuerpo del email]

Alternativas de asunto:
1. [Opcion 2]
2. [Opcion 3]

Mensaje LinkedIn (si no hay email):
[Mensaje de conexion <300 chars]
```
