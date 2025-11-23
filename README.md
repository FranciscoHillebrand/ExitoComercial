# 🛒 Retail Analytics: Descubriendo el Éxito Comercial

![Status](https://img.shields.io/badge/Status-Finalizado-success?style=for-the-badge)
![Tool](https://img.shields.io/badge/Google%20Sheets-Analytics-34A853?style=for-the-badge&logo=google-sheets&logoColor=white)

## 📖 Descripción del Proyecto

En el competitivo mundo del retail, anticiparse a la demanda es la clave de la rentabilidad. Este proyecto asume el rol de un **Data Analyst** encargado de modelar y analizar el histórico de ventas de una cadena minorista.

El objetivo principal fue transformar datos desconectados en un modelo de decisión capaz de predecir el impacto de **fechas especiales (Super Bowl, Navidad, Acción de Gracias)** y evaluar el rendimiento por departamento, utilizando exclusivamente **Google Sheets** para todo el ciclo de vida del dato.

---

## ⚙️ Metodología y Flujo de Trabajo

### 1. Ingeniería de Datos y ETL
Se procesaron tres fuentes de datos principales (`Stores`, `Sales`, `Features`) que contenían información histórica, datos macroeconómicos (CPI, Desempleo) y características de las tiendas.
* **Limpieza:** Tratamiento de valores nulos en columnas de "Markdowns" (descuentos promocionales).
* **Transformación:** Creación de variables temporales para aislar el impacto de las semanas festivas.

### 2. Modelado de Datos (DER)
Dado que los datos provenían de fuentes planas, fue necesario diseñar un modelo relacional para asegurar la integridad del análisis.
* Se normalizaron las tablas definiendo **Primary Keys** y relaciones lógicas entre las ventas fácticas y las dimensiones de tienda y otras features como el tiempo.

> 📄 **Documentación Técnica:**
> Puedes consultar el diseño detallado del Diagrama Entidad-Relación y el Modelo Relacional en el siguiente archivo:
> 👉 [**Ver PDF de Modelado de Datos**](./DER%20Y%20MODELO%20RELACIONAL.pdf)


## 💡 Insights Clave de Negocio

Tras un análisis exhaustivo utilizando tablas dinámicas y medidas de tendencia central robustas (mediana), se llegaron a las siguientes conclusiones:

### 🏢 Dinámica de las Tiendas
* **Tamaño vs. Ventas:** Existe una correlación positiva clara: las tiendas más grandes son las que generan mayor volumen de ventas.
* **Dominio del Tipo A:** Las tiendas "Tipo A" son las líderes en facturación. Aunque esto se explica parcialmente porque son mayoría en cantidad, también son las que ejecutan estrategias de promoción más agresivas.

### 🏷️ Estrategia de Promociones (Markdowns)
* **Correlación de Éxito:** Las tiendas con mayores ventas son, consistentemente, las que más facturan a través de "Markdowns", validando la efectividad de las campañas de descuento.
* **Top Performers:** Al desglosar por tipo de promoción, el **Markdown 1** demostró ser el más efectivo para generar ingresos, seguido de cerca por el **Markdown 5**.

### 📅 Temporalidad y Tendencias
* **La Caída del 2012:** Se detectó una contracción generalizada del negocio. Todas las tiendas vendieron menos en 2012 en comparación con 2011, un patrón sistémico confirmado por las líneas de tendencia individuales.
* **Estaciones Pico:** Contrario a lo esperado, la mediana de ventas indica que **Primavera y Verano** son las estaciones de mayor rendimiento comercial.
* **El Paradigma de los Feriados:** Al analizar la mediana de ventas (para evitar sesgos por outliers), se descubrió que en los días feriados se vende **aproximadamente la mitad** en comparación con días normales.

### 🌡️ Factores Externos (Macroeconomía)
* **Temperatura:** Se observa un leve aumento en las ventas a medida que la temperatura desciende, sugiriendo una oportunidad para productos estacionales de frío.
* **Impacto Económico Limitado:** Variables como el **CPI** (Índice de Precios), el precio del **Combustible** y la tasa de **Desempleo** mostraron correlaciones bajas o tendencias muy leves, indicando que las ventas de la cadena son relativamente resilientes a variaciones macroeconómicas moderadas.
---

## 📁 Estructura del Repositorio

* `WAREHOUSE.xlsx`: Archivos fuente con las tablas de hechos y dimensiones.
* `Informe.pdf`: Reporte narrativo del análisis.
* `DER Y MODELO RELACIONAL.pdf`: Diagramas de arquitectura de datos.

---
**Autor:** Francisco Javier Hillebrand
[LinkedIn](Tu_Link_Aquí) | [Portafolio](Tu_Link_Aquí)
