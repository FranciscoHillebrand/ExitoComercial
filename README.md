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

El análisis reveló patrones de consumo críticos para la planificación de inventario:

### 📅 El Impacto de la Estacionalidad (Fechas Especiales)
* **Picos Navideños:** Se identificó que las semanas previas a Navidad y Acción de Gracias representan los picos máximos de facturación anual, superando en un **X%** a una semana promedio.
    * *Acción:* El inventario debe reforzarse 4 semanas antes de estas fechas, no durante.
* **Super Bowl vs. Labor Day:** A diferencia de las festividades familiares, fechas como el Super Bowl muestran un impacto alto pero focalizado en departamentos específicos (probablemente Alimentos y Bebidas), mientras que otros departamentos no sufren variación.

### 🏢 Rendimiento por Tipo de Tienda
* **Tiendas Tipo A (Dominantes):** Representan el mayor volumen de ventas y son las más sensibles a las promociones (Markdowns).
* **Tiendas Tipo C:** Mantienen un flujo de ventas más estable pero con tickets promedio más bajos, sugiriendo una estrategia de "conveniencia" más que de "destino".

### 📉 Factores Externos
* Se observó que variables macroeconómicas como el **CPI (Índice de Precios al Consumidor)** o el precio del combustible tienen una correlación menor con las ventas inmediatas en comparación con los descuentos promocionales (Markdowns), lo que indica que el cliente responde más a ofertas directas que al contexto económico general en compras minoristas.

---

## 📁 Estructura del Repositorio

* `WAREHOUSE.xlsx`: Archivos fuente con las tablas de hechos y dimensiones.
* `Informe.pdf`: Reporte narrativo del análisis.
* `DER Y MODELO RELACIONAL.pdf`: Diagramas de arquitectura de datos.

---
**Autor:** Francisco Javier Hillebrand
[LinkedIn](Tu_Link_Aquí) | [Portafolio](Tu_Link_Aquí)
