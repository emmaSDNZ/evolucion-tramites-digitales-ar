# Dashboard de Trámites Digitales: Evolución y Proyecciones

### 1. Descripción del Proyecto

Este proyecto consiste en la creación de un **dashboard interactivo en Power BI** diseñado para analizar la evolución temporal de los trámites digitales. El objetivo principal es apoyar la toma de decisiones estratégicas en la gestión pública, proporcionando una herramienta visual que permite identificar tendencias, estacionalidades y picos de demanda.

---

### 2. Objetivos del Dashboard

El dashboard fue desarrollado con los siguientes propósitos clave:

* **Visión General**: Proveer un panorama claro y conciso del volumen acumulado de trámites digitales.
* **Análisis de Evolución**: Analizar la evolución temporal de los trámites tanto a nivel mensual como interanual.
* **Detección de Patrones**: Identificar tendencias y patrones estacionales que influyen en la demanda.
* **Identificación de Picos**: Detectar y analizar picos destacados, a menudo asociados a eventos especiales como la pandemia o nuevas normativas.
* **Proyecciones**: Generar proyecciones de trámites futuros y modelar escenarios de planificación (optimista y pesimista) para una mejor gestión de recursos.

---

### 3. Beneficiarios

Esta herramienta es de gran valor para:

* **Responsables de Gestión Pública**: Para monitorear el avance de la digitalización y el impacto de las políticas públicas.
* **Ejecutivos y Decisores**: Para anticipar escenarios de demanda y planificar la asignación de recursos de manera proactiva.
* **Equipos de Innovación Tecnológica**: Para planificar la capacidad de los sistemas y detectar oportunidades de mejora en la infraestructura digital.

---

### 4. Estructura del Dashboard

El dashboard se organiza en tres páginas principales para una navegación intuitiva:

* **Página 1: Visión General**
    * **KPI 1**: Total de Trámites Acumulados
    * **KPI 2**: Evolución Mensual e Interanual
    * **KPI 3**: Variación Anual % y Mensual %

* **Página 2: Análisis de Tendencias y Patrones**
    * **KPI 4**: Crecimiento Mensual (%)
    * **KPI 5**: Estacionalidad Promedio por Mes
    * **KPI 6**: Picos Destacados

* **Página 3: Proyecciones y Escenarios**
    * **KPI 7**: Proyección de Trámites en los Próximos Meses (basada en un modelo de tendencia lineal)
    * **KPI 8**: Escenarios de Planificación (Optimista vs. Pesimista)

---

### 5. Dataset Utilizado

* **Fuente**: Dataset público oficial de trámites digitales.
* **Cobertura temporal**: 2016 – 2025.
* **Granularidad**: Trámites registrados por fecha de publicación.
* **Variables principales**: `id_tramite`, `fecha_publicacion_produccion`, `anio`, `mes`, entre otras.

---

### 6. Metodología

1.  **Ingesta y Transformación de Datos (Power Query)**:
    * Conexión al dataset y limpieza inicial de campos.

2.  **Modelado de Datos**:
    * Creación de una tabla `Calendario` con la función `ADDCOLUMNS`.
    * Establecimiento de relaciones entre la tabla de trámites y la tabla calendario.

3.  **Métricas DAX (Key Performance Indicators)**:
    * **Medidas Base**:
        * `Tramites Por Mes`: `COUNTROWS('lista-tramites-vigentes-total-procesado')`
        * `Tramites Acumulados`: `CALCULATE(COUNTROWS('lista-tramites-vigentes-total-procesado'), FILTER(ALL(Calendario), Calendario[Date] <= MAX(Calendario[Date])))`
    * **Medidas de Proyección**:
        * `Proyeccion Lineal`: Medida que calcula la línea de tendencia lineal.
        * `Proyeccion Diciembre 2025`: Medida de tarjeta que calcula el valor proyectado para una fecha específica.
        * `Escenario Optimista`: `[Proyeccion Lineal] * 1.2`
        * `Escenario Pesimista`: `[Proyeccion Lineal] * 0.8`

4.  **Visualización**:
    * **Gráficos de Líneas y Columnas**: Utilizados para la evolución temporal y estacionalidad.
    * **Tarjetas KPI**: Para mostrar valores clave como la proyección.
    * **Gráfico de Área**: Para visualizar la proyección y los escenarios de planificación.

---

### 7. Validación de Resultados

La consistencia y precisión de los datos se validó mediante:

* Verificación de los totales contra los registros originales.
* Revisión de la consistencia de las series de tiempo.
* Validación de las proyecciones observando la tendencia en los datos históricos.

---

### 8. Entregables

* Archivo **Power BI (.pbix)** con el dashboard interactivo.
* Dataset limpio en formato CSV/Excel.
* Este archivo **README.md** como documentación del proyecto.

---

### 9. Próximos Pasos

* Explorar modelos de *forecasting* más avanzados (ej. ARIMA o series de tiempo con Python/R) para obtener proyecciones más precisas, considerando la tendencia de la serie histórica.
* Incorporar segmentación por tipo de trámite y región para un análisis más granular.
* Automatizar la actualización del dataset para mantener el dashboard siempre al día con los datos más recientes.