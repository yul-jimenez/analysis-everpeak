# EverPeak Retail Analysis – Sprint 6

Este repositorio contiene el análisis realizado durante el Sprint 6 del caso EverPeak–SilverBasket.

El dataset `everpeak_retail` incluye 2,000 órdenes de clientes con valores faltantes, sentinels, outliers y problemas de calidad diseñados para simular datos reales del retail. :contentReference[oaicite:2]{index=2}

## 📂 Contenido del repositorio

- `notebooks/everpeak_analysis.ipynb`
  → Notebook principal con limpieza, EDA, distribuciones, outliers y conclusiones.

## ▶ Cómo abrir el notebook en Google Colab

Haz clic en el siguiente botón:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](URL_DEL_NOTEBOOK_EN_GITHUB)

O:

1. Abre el archivo `.ipynb` en GitHub
2. Haz clic en **Open in Colab**

## 📘 Cómo reproducir el análisis

1. Abre `notebooks/everpeak_analysis.ipynb`
2. Ejecuta las celdas en orden
3. El notebook carga automáticamente el dataset desde `/data/` o desde un enlace público (según corresponda)

## 🧠 Objetivo del análisis

- Identificar problemas de calidad de datos
- Construir un pipeline de limpieza reproducible
- Analizar comportamientos, distribuciones y outliers
- Generar insights para el equipo de Estrategia e Integración de EverPeak

Google Colab 
https://colab.research.google.com/drive/1_3spf8pksENPsY0wnyhVr1eX1bWOMynH?usp=sharing

Objetivo del Proyecto

El objetivo de este proyecto es analizar el comportamiento de los clientes de ConnectaTel, identificando patrones de uso, segmentando usuarios según su consumo y edad, y generando insights que permitan optimizar la oferta de planes y mejorar la toma de decisiones del negocio.

Datasets Utilizados

Se utilizaron los siguientes datasets:

users: Información de los clientes
user_id, age, city, reg_date, plan, churn_date
usage: Información de uso de servicios
user_id, type (text/call), duration, length, date
plans: Información de los planes disponibles
plan_name, messages_included, minutes_included, usd_monthly_pay, etc.

Etapas del Análisis
1. Limpieza de datos
- Conversión de fechas
- Manejo de valores nulos
- Reemplazo de valores inválidos (ej: -999, '?')
- Identificación y análisis de outliers
2. Transformación de datos
- Creación de variables auxiliares (is_text, is_call)
- Agregación de métricas por usuario
- Unión de datasets (usage + users)
3. Análisis exploratorio
- Estadísticos descriptivos
- Distribución de variables numéricas
- Visualización por tipo de plan
4. Segmentación
- Clasificación por nivel de uso (Bajo, Medio, Alto)
- Clasificación por edad (Joven, Adulto, Adulto Mayor)
5. Visualización
- Histogramas
- Boxplots
- Gráficos de distribución por segmento
6. Insights y recomendaciones
- Identificación de patrones de comportamiento
- Evaluación de segmentos valiosos
- Propuestas de mejora en planes


Conclusión

El análisis muestra que el comportamiento de uso es el principal factor de segmentación, destacando oportunidades de negocio en usuarios de uso medio y alto. Esto permite diseñar estrategias de upselling y mejorar la oferta de planes.
