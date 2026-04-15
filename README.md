# Análisis de Tarifas Aéreas vs. Precios del Combustible (2019–2026)

**Autor:** Franco Agustín Marani

**Curso:**  Curso de Herramientas basicas para el Analisis de Datos

**Cohorte:** 2026  

---

## Descripción del proyecto

Este proyecto analiza el modo en que los distintos procesos geopolíticos impactaron en los precios globales del combustible, y como consecuencia de ello en las tarifas aéreas de 33 aerolíneas durante el período enero 2019 – marzo 2026. 
El análisis integra Python, Power BI y GitHub en un flujo de trabajo end to end de análisis de datos.

---

## Pregunta de investigación

**Principal:** ¿Cómo evolucionaron las tarifas aéreas promedio entre 2019 y 2026 en relación al precio del combustible de aviación, y qué fases geopolíticas explican los mayores incrementos y caídas?

**Subpregunta:** ¿Qué tipo de aerolínea (Flag Carrier o Low Cost) trasladó proporcionalmente más el costo del combustible al pasajero a través del recargo por combustible durante cada fase de crisis?

---

## Dataset

- **Nombre:** Airline Ticket Prices vs Oil & Fuel Costs
- **Fuente:** [Kaggle] ([https://www.kaggle.com/datasets/zkskhurram/airline-ticket-prices-vs-oil-and-fuel-cost]
- **Formato:** CSV | 14.355 filas | 18 columnas
- **Período:** Enero 2019 – Marzo 2026
- **Archivo:** [airline_ticket_prices.csv](data/raw/airline_ticket_prices.csv)

---

## Pasos realizados

### 1. Ingesta y limpieza (Python)
- Carga del dataset con pandas
- Auditoría de tipos, nulos, duplicados y outliers
- Eliminación de columnas redundantes (`iata_code`)
- Estandarización de fechas y categorías
- Traducción de fases geopolíticas

### 2. Exploración y visualización (Python)
- Gráfico de evolución temporal de tarifas y combustible
- Gráfico de tarifa promedio por fase y tipo de aerolínea
- Scatter plot de correlación Jet Fuel vs. Tarifa Total
- Heatmap de correlaciones entre variables financieras

### 3. Dashboard interactivo (Power BI)
- 2 KPIs: Tarifa promedio, Recargo combustible,
- 5 visualizaciones distribuidas en 2 páginas

---

## Principales hallazgos

- La correlación entre jet fuel y tarifa final es de apenas 0,28,  indicando que el combustible explica solo el 28% de la variación
  en los precios. 
- Flag Carriers y Low Cost convergieron hacia tarifas similares en todas las fases de crisis, sugiriendo que el modelo de negocio
  pierde relevancia como diferenciador de precios ante shocks globales.
- La fase US-Iran War Conflict (2026) generó los mayores recargos por combustible históricos, superando USD 120 promedio por pasaje.
- Asia registró la tarifa promedio más alta por región (USD 1.239),  mientras que Europa presentó los valores más bajos (USD 1.026).

---

## Estructura del repositorio
