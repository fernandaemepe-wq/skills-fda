---
name: performance-report
description: Genera reporte de metricas de marketing con analisis de tendencias, wins y misses, y recomendaciones priorizadas. Usar al cerrar un periodo (semanal, mensual) por marca, al preparar resumen para las marcas, o al traducir datos en resumen ejecutivo con prioridades para el siguiente periodo. Aplica a Sisteco, MicroSec y Marketing FDA.
argument-hint: "<periodo o marca> — ej: 'agosto Sisteco' o 'semana del 20 sep'"
---

# Performance Report — FDA

Genera reporte de desempeno de marketing con metricas clave, analisis de tendencias, insights y recomendaciones de optimizacion.

## Trigger

Fer pide reporte de metricas, revision de desempeno, resultados de periodo, o resumen de canales.

## Inputs

1. **Marca**: Sisteco, MicroSec, o FDA global
2. **Periodo**: ultima semana, ultimo mes, rango especifico
3. **Datos**: capturas de Instagram Insights / LinkedIn Analytics como texto, CSV, tabla, o numeros clave escritos directamente

## Reglas de analisis FDA

- Comparar solo contra si misma: Sisteco vs Sisteco periodo anterior, nunca Sisteco vs MicroSec.
- Con menos de 5 publicaciones, las conclusiones son provisorias (marcarlas como tales).
- Maximo 2 ajustes accionables por periodo.
- Si un aprendizaje se repite 2+ veces -> proponer linea exacta para el cerebro de la marca.

## Proceso

### 1. Registro de datos por pieza
Fecha / Canal / Formato / Pilar / Impresiones / Alcance / Interacciones / Guardados / Compartidos

### 2. Mejor y peor pieza del periodo (por marca)
- Mejor: metricas mas altas + hipotesis de por que (pilar, formato, gancho, horario)
- Peor: metricas mas bajas + hipotesis de por que

### 3. Tendencias
- Que formatos funcionan mejor?
- Que pilares generan mas engagement?
- Patrones de horario o dia?

### 4. Maxximo 2 recomendaciones
Priorizadas por impacto en el siguiente periodo.

### 5. Aprendizajes para el cerebro (si aplica)
Si algo se confirma 2+ veces -> linea lista para pegar en el cerebro de la marca.

### 6. Estado de experimentos activos
Evaluar metrica de exito: validado / descartado / sigue en curso.

## Formato de salida

**[MARCA] — Periodo: [FECHAS]**

Datos del periodo (tabla)
Mejor pieza + hipotesis
Peor pieza + hipotesis
Tendencias (2-3 observaciones)
2 ajustes para el proximo periodo
Aprendizaje para el cerebro (si aplica)
