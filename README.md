# Evolución de los trámites digitales en Mi Argentina

## Descripción
Este proyecto analiza la evolución de los trámites digitalizados en la plataforma *Mi Argentina*, aplicando herramientas de **análisis matemático y ciencia de datos**. Se estudia la evolución temporal de los trámites mediante **funciones, derivadas e integrales**, y se complementa con visualizaciones interactivas en Python y un dashboard en Power BI.

El objetivo principal es entender cómo se han incorporado los trámites digitales, evaluar la velocidad de crecimiento y la acumulación de servicios a lo largo del tiempo, y analizar brechas sociales en el acceso a la digitalización estatal.

---

## Objetivos

**Generales:**
- Modelar matemáticamente la evolución de los trámites digitales en el tiempo.
- Visualizar y comunicar resultados de manera clara y profesional.

**Específicos:**
- Calcular la **tasa de incorporación de trámites** usando derivadas.
- Estimar la **acumulación total de trámites** mediante integrales definidas.
- Generar gráficos interactivos y un dashboard para explorar la evolución.
- Analizar el impacto social y territorial de la digitalización.

---

## Tecnologías utilizadas
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

## Estructura del repositorio

```text
evolucion-tramites-digitales-ar/
├── data/
│   ├── raw/                # Dataset(s) originales
│   └── processed/          # Dataset(s) limpios y listos para análisis
├── notebooks/
│   └── 02_analisis_matematico.ipynb   # Notebook completo con preprocesamiento, modelado y visualizaciones
├── powerbi/
│   ├── dashboard.pbix       # Archivo de Power BI
│   └── capturas/            # Capturas de pantalla para README
├── report/
│   └── Informe_Tecnico.pdf  # Informe final en PDF
├── src/
│   └── funciones_auxiliares.py # Scripts de limpieza o preprocesamiento si aplican
└── README.md               # Presentación del proyecto


## 🔗 Recursos
- [Dashboard en Power BI](URL_AQUI)  
- [Informe técnico](report/Informe_Tecnico.pdf)  

## Autor
Isaias Emanuel Sudañez – Estudiante de Ciencias de Datos e IA  

Proyecto desarrollado en el marco del espacio curricular Análisis Matemático de la Tecnicatura Superior en Ciencia de Datos e Inteligencia Artificial.