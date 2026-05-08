# **DYNAMICS FINANCIAL FORECASTING: MODELADO ESTRATÉGICO Y PROYECCIÓN 2026**
**Autor:** Julián Esteban León Ospina

![Status](https://img.shields.io/badge/Status-Finalizado-success)
![Stack](https://img.shields.io/badge/Stack-Python%20%7C%20Holt--Winters%20%7C%20Power%20BI-gold)

## **Descripción del Proyecto**
Este ecosistema de inteligencia financiera analiza el crecimiento histórico y proyecta el desempeño comercial hacia el cierre de 2026. Combina análisis de sensibilidad multivariable con **Machine Learning (Holt-Winters)** para transformar datos transaccionales en una hoja de ruta estratégica, facilitando la toma de decisiones basada en datos para la alta gerencia.

---

## **Estructura del Ecosistema Analítico**

### **1. Parte I: Diagnóstico Estratégico y Sensibilidad (EDA)**
* **Drivers de Negocio:** Validación estadística de variables clave: TRM, Tráfico Web, Tasas de Conversión y Precios de Competencia.
* **Correlación Macroeconómica:** Identificación de la sensibilidad de los ingresos frente a la volatilidad de la TRM en Colombia.
* **Análisis de Hipótesis:** Determinación de la elasticidad de los ingresos ante cambios en presupuestos de marketing y eficiencia operativa.

### **2. Parte II: Modelado Predictivo y Forecasting (ML)**
* **Algoritmo de Serie de Tiempo:** Implementación del modelo **Holt-Winters (Exponential Smoothing)** para capturar estacionalidad y tendencia.
* **Proyección 2026:** Generación de pronósticos mensuales con un enfoque de crecimiento orgánico estimado (7-8%).
* **Escenarios What-If:** Creación de medidas dinámicas para simular impactos económicos basados en variaciones de la conversión.

---

## **3. Parte III: Business Intelligence Deployment (Power BI)**
> **Ubicación:** `/dashboards/Financial_Forecasting.pbix`

#### **A. Análisis de Sensibilidad y Correlación TRM**
![Correlación Financiera](./images/image_6771b2.png)
* **Impacto Macroeconómico:** Análisis dinámico de la correlación entre la Tasa de Cambio (TRM) y el volumen de ventas.
* **Crecimiento Trimestral:** Visualización de la tasa de crecimiento por departamento, facilitando la detección de mercados regionales estrella.

#### **B. Proyección de Ventas y Modelado Holt-Winters**
![Pronóstico de Ventas](./images/image_67717a.png)
* **Forecasting 2026:** Implementación visual del modelo para proyectar el comportamiento comercial en los próximos ciclos fiscales.
* **Análisis de Estacionalidad:** Comparativa anual por mes que permite anticipar picos de demanda y optimizar la asignación de recursos.

---

## **4. Recorrido Visual: Dashboards e Insights Técnicos**
> **Ubicación de recursos:** `/images/` y `/dashboards/Financial_Forecasting.pbix`

A continuación, se presenta la secuencia lógica del ecosistema, recorriendo desde la validación de datos en Python hasta la toma de decisiones estratégica en Power BI.

### **Fase 1: Diagnóstico y Robustez de Datos (EDA)**
![Diagnóstico de Datos](images/image_722dbd.png)
> **Insight Técnico:** Iniciamos con un diagnóstico de **Data Quality**. Aquí validamos la no-normalidad de los activos mediante la **prueba de Jarque-Bera** y analizamos la matriz de correlación. Este paso es crítico para confirmar que los modelos lineales tradicionales son insuficientes y justificar un enfoque estocástico.

---

### **Fase 2: Modelado de Riesgo y Proyección Estocástica (ML)**

| Referencia | Visualización | Descripción y Valor Agregado |
| :--- | :--- | :--- |
| **Riesgo Extremo** | ![Monte Carlo VaR](images/image_7221ff.png) | **Simulación Monte Carlo:** Proyección de 10,000 escenarios posibles. Identificamos el **VaR (Value at Risk)** y el **CVaR**, detectando la 'Zona de Crisis' para proteger el capital ante eventos de baja probabilidad. |
| **Forecasting** | ![Proyección Estocástica](images/image_7222d8.jpg) | **Abanico de Probabilidades:** Más allá de una línea única, presentamos un abanico de confianza que muestra la tendencia central y la dispersión esperada, permitiendo una planificación basada en rangos. |
| **Explicabilidad** | ![SHAP Values](images/image_7225bb.png) | **IA Explicable (SHAP):** Desglose de la contribución de cada activo al rendimiento del modelo. Garantizamos transparencia (No "Black Box") para que la gerencia entienda los drivers de las proyecciones. |

---

### **Fase 3: Business Intelligence & Strategic Insights (Power BI)**

| Referencia | Visualización | Valor para la Alta Gerencia |
| :--- | :--- | :--- |
| **Estrategia** | ![Frontera Eficiente](images/image_722d78.png) | **Optimización de Markowitz:** Identificación del portafolio que maximiza el **Sharpe Ratio**. Es el entregable final: una combinación equilibrada ubicada en la frontera eficiente. |
| **Ejecución** | ![Ingresos y Proyección](images/dashboard1.png) | **KPIs Principales:** Monitor de Ingresos Totales ($22.4B) y Crecimiento Anual (34.36%) con comparativas dinámicas vs. metas proyectadas. |
| **Geografía** | ![Análisis Geográfico](images/dashboard2.png) | **Segmentación Regional:** Mapa de calor de ingresos y eficiencia por departamento, identificando territorios líderes (Cundinamarca) vs. regiones con brechas de ejecución. |
| **Operación** | ![Tablas Gerenciales](images/dashboard4.png) | **Auditoría y GAP:** Tablas de control detalladas para el cálculo de la **Brecha de Ejecución (GAP)** y variaciones porcentuales mensuales para ajuste táctico. |

---

## **Tecnologías Utilizadas**
* **Lenguaje:** Python (Pandas, Statsmodels, Scikit-Learn).
* **Modelado:** Holt-Winters para series temporales.
* **Visualización:** Power BI (Integración de modelos ML + DAX Avanzado).
* **Entorno:** Jupyter Notebooks para validación estadística.

## **Insights Principales**
1. **Dependencia de Conversión:** La optimización de la tasa de conversión tiene un impacto marginal en el ingreso significativamente mayor que el incremento en el tráfico web.
2. **Protección Cambiaria:** Se confirma una correlación positiva sólida con la TRM, sugiriendo que el modelo de negocio actúa como una cobertura natural ante la devaluación.
3. **Crecimiento Estable:** El pronóstico 2026 indica un crecimiento homogéneo, permitiendo a la organización enfocarse en la eficiencia operativa.


1- image_722dbd.png
2- image_722d9a.png
3- image_722d78.png
4 - image_722d3b.png
5- image_72261d.png
6- image_7225bb.png
7- image_7222d8.jpg
8- image_7221ff.png
9-
