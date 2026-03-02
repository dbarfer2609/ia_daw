# Práctica IA (RA4 · b+c) — Big Data, análisis, rentabilidad y valoración IA

## 1) Caso y objetivo de negocio
- Empresa/sector: Plataforma de streaming digital (ej. Netflix).
- Problema a resolver: Alta tasa de cancelación de suscripciones (churn) y dificultad para mantener el interés del usuario.
- Objetivo de negocio (rentabilidad): Reducir cancelaciones y aumentar ingresos recurrentes mediante personalización.
## 2) Big Data: recogida masiva de datos
Describe por qué es Big Data (volumen, velocidad, variedad).
- Es Big Data porque cumple las 3V:
    Volumen: Millones de usuarios y miles de millones de eventos diarios.
    Velocidad: Datos generados en tiempo real (clics, pausas, búsquedas).
    Variedad: Datos estructurados y no estructurados.
- Fuente 1: Historial de visualización (qué ve cada usuario, cuánto tiempo, cuándo abandona).
- Fuente 2: Interacciones (búsquedas, clics, valoraciones).
- Fuente 3: Datos contextuales (dispositivo, ubicación aproximada, hora del día).
- Volumen/velocidad (estimación): Millones de eventos por minuto a nivel global.
- Formatos (texto, eventos, series temporales, imágenes, etc.): Eventos de clic, series temporales (tiempo de visualización), texto (búsquedas), metadatos de contenido.

## 3) Tratamiento/análisis: pipeline de datos
Explica el flujo de forma ordenada:
- Ingesta (captura/eventos): Los eventos de usuario se capturan en tiempo real cada vez que alguien interactúa con la plataforma.
- Limpieza/normalización: Eliminación de datos duplicados, corrección de errores y estandarización de formatos.
- Almacenamiento (data lake/warehouse): Data Lake para datos en bruto.
                                        Data Warehouse para datos estructurados listos para análisis.
- Preparación de variables (features):
      Tiempo medio de visualización.
      Géneros preferidos.
      Frecuencia de uso semanal.
      Tasa de abandono de episodios.
- Análisis/BI (opcional): Dashboards para analizar tendencias de consumo y segmentación de usuarios.

## 4) IA aplicada: modelo y decisión
- Tipo de IA/técnica (clasificación, predicción, recomendación, anomalías, NLP...): Sistema de recomendación (machine learning predictivo + filtrado colaborativo).
- Entrada del modelo (qué datos usa): Historial de consumo, gustos similares de otros usuarios, tiempo de visualización.
- Salida del modelo (qué produce): Lista personalizada de contenidos recomendados.
- Decisión que habilita (qué hace la empresa con esa salida): Mostrar recomendaciones personalizadas en la pantalla principal para aumentar el tiempo de uso y evitar cancelaciones.

## 5) Rentabilidad: KPIs antes/después (mínimo 3)
KPI 1 (ingresos/coste/eficiencia): 1,5 horas/día
- Antes: 8% mensual
- Después: 5% mensual
- Por qué mejora la rentabilidad: Más usuarios activos → más ingresos recurrentes.

KPI 2:
- Antes: 1,5 horas/día
- Después: 2,3 horas/día
- Por qué mejora la rentabilidad: Mayor engagement → menor probabilidad de baja.

KPI 3:
- Antes: 11 €/mes
- Después: 13 €/mes
- Por qué mejora la rentabilidad: Mayor retención y posibilidad de upselling (planes premium).

## 6) Diagrama del pipeline (ASCII o Mermaid)
```
+------------------+
|     USUARIOS     |
+------------------+
          |
          v
+------------------------------+
| Captura de eventos           |
| (clics, búsquedas, tiempo)   |
+------------------------------+
          |
          v
+------------------------------+
| Limpieza y normalización     |
| (errores, duplicados,        |
|  formatos estándar)          |
+------------------------------+
          |
          v
+------------------------------+
| Data Lake (datos en bruto)   |
+------------------------------+
          |
          v
+------------------------------+
| Feature Engineering          |
| (géneros, frecuencia,        |
|  tiempo medio, abandono)     |
+------------------------------+
          |
          v
+------------------------------+
| Modelo IA de recomendación   |
| (ML / filtrado colaborativo) |
+------------------------------+
          |
          v
+------------------------------+
| Recomendaciones              |
| personalizadas               |
+------------------------------+
          |
          v
+------------------------------+
| Mayor retención              |
| y rentabilidad               |
+------------------------------+
```

## 7) Riesgos y mitigación
Riesgo 1: Sesgo en recomendaciones
- Mitigación: Auditorías periódicas del modelo y diversidad forzada en sugerencias.

Riesgo 2: Problemas de privacidad
- Mitigación: Anonimización de datos y cumplimiento de normativa (RGPD).
## 8) Valoración (criterio c): importancia presente y futura de la IA (10–15 líneas)
- Importancia actual:
La IA es clave en plataformas de streaming porque permite personalizar la experiencia del usuario en un mercado altamente competitivo. Sin sistemas de recomendación, los usuarios tardarían más en encontrar contenido relevante, reduciendo su satisfacción y aumentando la probabilidad de cancelación.

- Importancia futura (3–5 años):
La IA evolucionará hacia recomendaciones más contextuales y predictivas, anticipando qué contenido querrá ver el usuario incluso antes de buscarlo. También se usará para optimizar la producción de contenido original basándose en patrones de consumo.

- Condiciones/limitaciones:
La calidad depende de la cantidad y calidad de los datos. Existen costes elevados de infraestructura, riesgos de privacidad y posibles sesgos algorítmicos.

- Conclusión razonada:
La IA no es solo una herramienta de mejora, sino un factor estratégico fundamental para la rentabilidad y sostenibilidad futura de plataformas como Netflix.

## 9) Fuentes oficiales (mín. 2)
- Big Data/analítica (enlace oficial): IBM – What is Big Data? https://www.ibm.com/topics/big-data
- IA/técnica/modelo (enlace oficial): Google Developers – Recommendation Systems https://developers.google.com/machine-learning/recommendation
