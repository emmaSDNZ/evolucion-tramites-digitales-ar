# Evolución de los trámites digitales en Mi Argentina

## 📌 Descripción
Este proyecto analiza la evolución de los trámites digitalizados en la plataforma *Mi Argentina*, aplicando herramientas de **análisis matemático y ciencia de datos**. Se estudia la evolución temporal de los trámites mediante **funciones, derivadas e integrales**, y se complementa con visualizaciones interactivas en Python y un dashboard en Power BI.

El objetivo principal es entender cómo se han incorporado los trámites digitales, evaluar la velocidad de crecimiento y la acumulación de servicios a lo largo del tiempo, y analizar brechas sociales en el acceso a la digitalización estatal.

---

## 🎯 Objetivos

**Generales:**
- Modelar matemáticamente la evolución de los trámites digitales en el tiempo.
- Visualizar y comunicar resultados de manera clara y profesional.

**Específicos:**
- Calcular la **tasa de incorporación de trámites** usando derivadas.
- Estimar la **acumulación total de trámites** mediante integrales definidas.
- Generar gráficos interactivos y un dashboard para explorar la evolución.
- Analizar el impacto social y territorial de la digitalización.

---

## 🛠️ Tecnologías utilizadas
- **Python:** Pandas, Numpy, Matplotlib, Plotly, Scipy
- **Power BI:** Dashboard interactivo
- **Google Forms / Typeform:** Encuestas complementarias sobre percepción ciudadana

---

## 📊 Resultados principales

1. **Serie temporal de trámites acumulados**  
   Representa la función creciente \( F(t) \) de trámites digitalizados desde 2016.

2. **Tasa de crecimiento diaria**  
   La derivada \( F'(t) \) muestra cuántos trámites se incorporaron cada día.

3. **Estimaciones por integral definida**  
   La integral definida de \( F(t) \) permite calcular el total de trámites incorporados en intervalos específicos.

4. **Visualizaciones interactivas**  
   - Evolución acumulada de trámites (gráfico de línea)
   - Tasa de crecimiento diaria (gráfico de barras)
   - Comparaciones sociales y territoriales en Power BI

---

## 📈 Conexión con el Negocio y Proyecciones

Para trasladar este análisis de la teoría a la práctica, los modelos matemáticos se visualizan en un **dashboard de Power BI**, diseñado específicamente para la toma de decisiones ejecutivas. Este enfoque permite:

* **Identificar patrones de negocio**: La derivada **$F'(t)$** (tasa de crecimiento diaria) se traduce en la detección de picos y caídas de trámites. Esto ayuda a los equipos a entender el impacto de eventos como lanzamientos de nuevos servicios o cambios en la normativa.
* **Evaluar la estacionalidad**: El análisis de la función **$F(t)$** por mes permite identificar patrones estacionales, como meses de alta o baja demanda. Esta información es crucial para la planificación de recursos humanos y tecnológicos.
* **Proyectar el futuro**: Basándose en los datos históricos, se implementa un modelo de proyección lineal (y se puede considerar un modelo polinómico para mayor precisión) con el fin de anticipar el volumen de trámites futuros.
* **Planificación estratégica**: Se definen escenarios de planificación (optimista y pesimista) directamente en el dashboard, proporcionando un rango de posibles resultados para mitigar la incertidumbre en la toma de decisiones.

---

## 📂 Estructura del repositorio

```text
evolucion-tramites-digitales-ar/
├── data/
│   ├── raw/                # Dataset(s) originales
│   └── processed/          # Dataset(s) limpios y listos para análisis
├── notebooks/
│   └── 02_analisis_matematico.ipynb   # Notebook completo con preprocesamiento, modelado y visualizaciones
├── powerbi/
│   ├── avolucion-tramites-digitales-argentina.pbix       # Archivo de Power BI
│   └── capturas/            # Capturas de pantalla para README
├── report/
│   └── Informe_Tecnico.pdf  # Informe final en PDF
├── src/
│   └── funciones_auxiliares.py # Scripts de limpieza o preprocesamiento si aplican
└── README.md               # Presentación del proyecto


## Autores 
Isaias Emanuel Sudañez,   
Luciana Goldraij 
Baigorria Sol Milagros, 
Luciano Castillo.


Proyecto desarrollado en el marco del espacio curricular Análisis Matemático de la Tecnicatura Superior en Ciencia de Datos e Inteligencia Artificial del ISPC.