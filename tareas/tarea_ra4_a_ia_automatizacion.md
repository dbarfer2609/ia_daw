# Práctica IA (RA4 · a) — Automatización y optimización

## 1) Proceso elegido
- Nombre del proceso: Predicción de abandono de carrito
- Contexto (empresa/servicio web/IT): Plataforma de e-commerce
- Rol/es implicados: 1. Cliente, 2. Sistema web, 3. Departamentos de marketing y  4. Analisis de datos

## 2) ANTES (sin IA)
- Pasos (5–7):
  1. El cliente navega por la web
  2. Añade productos al carrito
  3. El sistema espera a que complete la compra
  4. Si abandona, se registra el carrito como "no completado"
  5. Marketing envía campañas generales de recordatorio
  6. Se analizan métricas globales al final del mes
- Tiempo aproximado por caso: El análisis se realiza mensualmente.
- Problemas / cuellos de botella: 1. No se detecta el abandono en tiempo real y 2. Baja tasa de recuperación.

## 3) DESPUÉS (con IA)
- ¿Qué automatiza la IA?
.- Predicción en tiempo real de la probabilidad de abandono.
.- Activación automática de acciones (descuento, notificación push, email personalizado).
.- Segmentación inteligente de usuarios según comportamiento.
- ¿Qué queda para humanos?
.- Definir estrategias de marketing.
.- Supervisar resultados.
.- Ajustar promociones y políticas comerciales
- Datos necesarios (tipos de datos, sin datos personales):
.- Tiempo en la página
.- Número de productos añadidos.
.- Historial de compras.
.- Dispositivo utilizado.
.- Número de visitas previas.
.- Tiempo de inactividad antes de salir.
- Modelo/técnica (NLP, clasificación, recomendación, visión, etc.):
.- Machine Learning supervisado.
.- Clasificación binaria.
.- Modelos como Gradient Boosting o redes neuronales.
.- Análisis de comportamiento.

## 4) Optimización (mejora medible)
Define 3 métricas con valores antes/después:
- Tiempo:  Antes: 2000€ mensuales en campañas masivas poco efectivas.
           Después: 1.200€ mensuales en campañas personalizadas optimizadas.
- Coste:   Antes: 2000€ mensuales en campañas masivos poco efectivas.
           Después: 1.200€ mensuales en campañas personalizadas optimizadas.
- Calidad: Antes: tasa de recuperación de carritos del 8%.
           Después: tasa de recuperación del 18%.
           Incremento del 10% en conversión.

## 5) Diagrama del flujo (ASCII o Mermaid)
flowchart TD
A[Usuario añade producto al carrito] --> B[IA analiza comportamiento]
B --> C[Calcula probabilidad de abandono]
C -->|Probabilidad baja| D[Proceso normal]
C -->|Probabilidad alta| E[Activa incentivo personalizado]
E --> F[Usuario completa compra]
D --> G[Compra o abandono]

## 6) Riesgos y mitigación
- Riesgo 1: Ofrecer descuentos innecesarios a clientes que comprarían igualmente.
- Mitigación 1: Ajustar el umbral de activación del incentivo y evaluar ROI continuamente.
- Riesgo 2: Modelo poco preciso por datos insuficientes.
- Mitigación 2: Reentrenamiento periódico y validación cruzada del modelo.

## 7) Fuente oficial
- Enlace: Personalización y sistemas predictivos en Amazon
https://www.aboutamazon.com/
