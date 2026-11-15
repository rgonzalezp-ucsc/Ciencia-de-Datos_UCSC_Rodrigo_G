Archivos correspondientes al Laboratorio 5 de Ciencia de Datos.
# Proyecto Analítico – Bike Sharing
### Ciencia de Datos · Advance UCSC · Semana 5

**Estudiante:** Rodrigo González Panes  
**Universidad:** Universidad Católica de la Santísima Concepción  
**Repositorio:** Ciencia-de-Datos_UCSC_Rodrigo_G

---

## 1. Descripción del proyecto

Este proyecto analiza los patrones de demanda diaria de bicicletas del sistema Capital Bikeshare de Washington D. C., utilizando el conjunto de datos *Bike Sharing Dataset*, publicado por UCI Machine Learning Repository.

El análisis considera información de los años 2011 y 2012, con 731 registros diarios y 16 variables originales.

**Pregunta analítica:**

¿Cómo varía la cantidad diaria de alquileres de bicicletas según las condiciones meteorológicas, la estación del año y las características del calendario durante 2011 y 2012?

## 2. Objetivos

- Analizar el comportamiento de la demanda de bicicletas.
- Identificar patrones temporales y estacionales.
- Evaluar la relación entre condiciones meteorológicas y cantidad de alquileres.
- Aplicar técnicas de minería de datos mediante segmentación K-Means.
- Detectar jornadas con comportamientos atípicos.
- Generar conclusiones y recomendaciones para la planificación operativa.

## 3. Fuente de datos

**Conjunto:** Bike Sharing Dataset – archivo diario `day.csv`.

**Fuente:** UCI Machine Learning Repository.

**DOI:** 10.24432/C5W894.

**Licencia:** Creative Commons Attribution 4.0 International (CC BY 4.0).

**Unidad de análisis:** Un día de operación del sistema de bicicletas compartidas.

## 4. Metodología

El proyecto se desarrolló progresivamente durante cinco semanas utilizando Python y Google Colab.

Las principales técnicas aplicadas fueron:

- Exploración y análisis descriptivo de datos.
- Limpieza y preparación de variables.
- Análisis temporal y estacional.
- Análisis de correlaciones.
- Segmentación mediante K-Means.
- Detección de anomalías.
- Validación de resultados y análisis de limitaciones.

Para la segmentación se utilizó K-Means con tres grupos (K=3), semilla aleatoria 20264 y preparación de variables mediante StandardScaler y OneHotEncoder.

## 5. Principales resultados

**Gráfico 1 – Demanda mensual**

Junio presenta el mayor promedio diario de alquileres, con 5.772,37 bicicletas, seguido de septiembre con 5.766,52.

**Gráfico 2 – Demanda según condiciones meteorológicas**

Los días despejados o parcialmente nublados registran un promedio de 4.876,79 alquileres diarios. En condiciones de lluvia o nieve ligera, el promedio disminuye a 1.803,29.

Estos resultados muestran asociaciones descriptivas entre la demanda, el calendario y las condiciones meteorológicas. No demuestran causalidad.

## 6. Herramientas y tecnologías

- Python 3.
- Google Colab.
- Jupyter Notebook.
- Pandas.
- NumPy.
- Matplotlib.
- Scikit-learn.
- GitHub.

## 7. Reproducibilidad

La segmentación principal utiliza la siguiente configuración:

| Parámetro | Valor |
|---|---|
| Algoritmo | K-Means |
| Número de grupos | 3 |
| Semilla aleatoria | 20264 |
| Inicializaciones | 20 |
| Unidad de análisis | Día de operación |

Para consultar las versiones exactas de las bibliotecas utilizadas, ejecutar en Google Colab:

```python
import sys
import pandas as pd
import numpy as np
import matplotlib
import sklearn

print("Python:", sys.version)
print("Pandas:", pd.__version__)
print("NumPy:", np.__version__)
print("Matplotlib:", matplotlib.__version__)
print("Scikit-learn:", sklearn.__version__)
```

## 8. Archivos del proyecto

La carpeta `Semana_5_Entregables` contiene:

| Archivo | Descripción |
|---|---|
| Ficha_Riesgo_Etico...docx | Ficha ético-legal actualizada y cerrada. |
| GRAFICO_1_RG.png | Visualización de demanda mensual. |
| GRAFICO_2_RG.png | Visualización de demanda según clima. |
| README.md | Documentación de los entregables. |

El notebook principal y los archivos de trabajo de las semanas anteriores se encuentran en el directorio principal del repositorio.

## 9. Limitaciones

Los datos corresponden exclusivamente al sistema Capital Bikeshare durante 2011 y 2012. Por lo tanto, los resultados representan un comportamiento histórico y no necesariamente reflejan la demanda actual.

La información está agregada por día, por lo que no permite analizar viajes individuales, horarios punta ni características demográficas de los usuarios.

Los resultados deben interpretarse como evidencia descriptiva y no como relaciones causales.

## 10. Autor

**Rodrigo I.González Panes**  
Estudiante de Ingeniería de ejecución en Informática  
Universidad Católica de la Santísima Concepción (UCSC).

Proyecto académico - Ciencia de Datos.

