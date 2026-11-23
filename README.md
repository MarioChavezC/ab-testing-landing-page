# 📊 A/B Testing: Landing Page Experiment

## 📌 Descripción del proyecto

Análisis de un experimento A/B realizado en una página de inicio (Landing Page), cuyo objetivo es evaluar el desempeño de dos versiones (A y B) e identificar cuál genera mejores resultados de negocio.

Se utilizan técnicas de análisis exploratorio, pruebas de hipótesis y visualización de datos para determinar si existen diferencias estadísticamente significativas en las tasas de conversión y el gasto promedio de los usuarios convertidos.

El proyecto busca transformar los resultados estadísticos en recomendaciones estratégicas basadas en datos.

## 🎯 Objetivos

- Evaluar la calidad e integridad del conjunto de datos.
- Comparar el gasto promedio de los usuarios convertidos entre las versiones A y B.
- Analizar las diferencias en las tasas de conversión.
- Identificar la relación entre las fuentes de tráfico y las conversiones.
- Evaluar el comportamiento de usuarios nuevos y recurrentes.
- Comunicar los resultados mediante visualizaciones e insights ejecutivos.

## 🗂️ Dataset

**Archivo:** `landing_experiment.csv`

El conjunto de datos contiene 40,000 registros y 9 variables:

| Variable | Descripción |
|---|---|
| user_id | Identificador único del usuario |
| date | Fecha de exposición |
| landing | Versión de página (A/B) |
| region | Región geográfica |
| dispositivo | Tipo de dispositivo |
| traffic_source | Fuente de tráfico |
| user_type | Tipo de usuario |
| converted | Indicador de conversión (0/1) |
| gasto | Gasto realizado por el usuario |

## 🛠️ Tecnologías y herramientas

- Python
- Pandas – Manipulación y análisis de datos.
- Matplotlib – Visualización de datos.
- SciPy – Pruebas estadísticas.
- Statsmodels – Pruebas de proporciones.
- Jupyter Notebook – Desarrollo y documentación del análisis.

## 🔬 Metodología

### 1. Exploración y validación de datos
- Revisión de estructura y tipos de datos.
- Identificación de valores nulos y duplicados.
- Validación de identificadores únicos.
- Análisis de variables numéricas y categóricas.

### 2. Comparación del gasto promedio
- Prueba de Levene para evaluar igualdad de varianzas.
- Prueba t de Welch para comparar el gasto promedio de usuarios convertidos.

### 3. Comparación de tasas de conversión
- Prueba Z para comparar dos proporciones.
- Evaluación de significancia estadística.

### 4. Análisis de fuentes de tráfico
- Tablas de contingencia.
- Prueba Chi-cuadrado de independencia.
- Comparación de tasas y volúmenes de conversión.

### 5. Análisis por tipo de usuario
- Comparación entre usuarios nuevos y recurrentes.
- Prueba Chi-cuadrado de independencia.

### 6. Visualización de resultados
- Conversión por fuente de tráfico.
- Distribución de conversiones por tipo de usuario.
- Comparación de versiones A y B por segmento.

### 7. Insights ejecutivos
Interpretación de resultados y elaboración de recomendaciones para la toma de decisiones.

## 📈 Principales resultados

| Indicador | Landing A | Landing B |
|---|---:|---:|
| Usuarios | 19,982 | 20,018 |
| Conversiones | 2,512 | 3,194 |
| Tasa de conversión | 12.57% | 15.96% |
| Gasto promedio por comprador | $61.09 | $68.75 |

### Hallazgos estadísticos

**Tasa de conversión**
- Diferencia: +3.38 puntos porcentuales a favor de B.
- Mejora relativa: +26.92%.
- Prueba Z: p-value = 3.76 × 10⁻²².
- Resultado: diferencia estadísticamente significativa.

**Gasto promedio por comprador**
- Diferencia: +$7.66 a favor de B.
- Mejora relativa: +12.54%.
- Prueba t de Welch: p-value = 3.63 × 10⁻²¹.
- Resultado: diferencia estadísticamente significativa.

**Fuente de tráfico**
- Email presenta la mayor tasa de conversión (14.99%).
- Organic genera el mayor volumen de conversiones (2,480).
- Chi-cuadrado: p-value = 0.0341.

**Tipo de usuario**
- Usuarios nuevos: 14.36% de conversión.
- Usuarios recurrentes: 14.09%.
- Chi-cuadrado: p-value = 0.4736.
- No se encontró evidencia estadística suficiente de asociación.

## 💡 Recomendaciones de negocio

1. Implementar la versión B debido a sus mejores resultados en conversión y gasto promedio por comprador.
2. Monitorear el ingreso promedio por visitante, margen de contribución y rentabilidad.
3. Optimizar los canales de adquisición considerando tasas de conversión y costos.
4. Mantener una experiencia consistente para usuarios nuevos y recurrentes.
5. Diseñar nuevos experimentos A/B para identificar los elementos que impulsan el desempeño de la versión B.

## 🚀 Conclusión

La versión B presenta un desempeño superior al de la versión A tanto en tasa de conversión como en gasto promedio entre usuarios convertidos.

Los resultados proporcionan evidencia estadística para recomendar su implementación. Sin embargo, será necesario monitorear los indicadores económicos posteriores al lanzamiento para determinar su impacto real en los ingresos y la rentabilidad.

---

**Autor:** Mario Chávez

**Área:** Data Analytics | Business Intelligence | Statistical Analysis

**Proyecto:** A/B Testing – Landing Page Experiment