# Selección de Regiones para la Expansión de Pozos Petrolíferos

## Descripción del proyecto

La empresa OilyGiant busca identificar la región más rentable para desarrollar 200 nuevos pozos petrolíferos. Para ello, se dispone de información geológica de tres regiones distintas y se requiere construir modelos predictivos que permitan estimar el volumen de reservas presentes en cada pozo.

El proyecto combina técnicas de Machine Learning y simulación estadística mediante Bootstrap para estimar beneficios potenciales y cuantificar el riesgo asociado a cada región antes de realizar una inversión millonaria.

## Objetivo

Seleccionar la región con la mejor relación entre rentabilidad esperada y riesgo financiero, utilizando modelos predictivos y análisis de incertidumbre.

## Datos

Se analizaron tres conjuntos de datos, cada uno correspondiente a una región potencial de exploración.

Cada dataset contiene:

- Identificador único del pozo.
- Tres variables geológicas predictoras.
- Volumen de reservas de petróleo (`product`).

## Tecnologías utilizadas

- Python
- Pandas
- NumPy
- Scikit-Learn
- SciPy
- Matplotlib
- Jupyter Notebook

## Metodología

### 1. Exploración y preparación de datos

- Carga de los tres datasets.
- Verificación de tipos de datos.
- Inspección de calidad de la información.
- Identificación de posibles inconsistencias.

### 2. Entrenamiento de modelos predictivos

Se entrenó un modelo de:

- Linear Regression

para cada una de las tres regiones.

Posteriormente se evaluó el desempeño utilizando:

- RMSE (Root Mean Squared Error)
- Reservas promedio predichas

### 3. Cálculo de rentabilidad

Se establecieron las condiciones económicas del proyecto:

- Presupuesto total de 100 millones de dólares.
- Selección de los 200 mejores pozos.
- Ingreso estimado por unidad de reserva extraída.

A partir de estas condiciones se calculó:

- Producción mínima necesaria para evitar pérdidas.
- Ganancia potencial por región.

### 4. Análisis de riesgo mediante Bootstrap

Para incorporar la incertidumbre del proyecto se aplicó:

- Muestreo Bootstrap con 1000 iteraciones.
- Selección de muestras aleatorias de pozos.
- Cálculo repetido de ganancias.

Con ello se estimaron:

- Ganancia promedio esperada.
- Intervalo de confianza del 95%.
- Probabilidad de pérdidas.

## Métricas utilizadas

### RMSE

Mide el error promedio de las predicciones realizadas por el modelo.

Un valor menor indica una mayor precisión predictiva.

### Ganancia esperada

Representa el beneficio económico promedio estimado para cada región.

### Riesgo de pérdidas

Porcentaje de simulaciones en las que el proyecto genera pérdidas económicas.

## Resultados principales

El análisis mostró diferencias importantes entre las regiones evaluadas.

La Región 1 presentó:

- El menor error de predicción.
- La mayor estabilidad en las simulaciones.
- El menor riesgo de pérdidas.
- Un intervalo de confianza completamente favorable.

Las demás regiones mostraron una probabilidad de pérdidas superior al límite de riesgo establecido por la compañía.

## Conclusiones

- La regresión lineal permitió estimar adecuadamente el volumen de reservas en cada región.
- El análisis Bootstrap proporcionó una evaluación más realista del riesgo financiero.
- La Región 1 presentó la mejor combinación entre rentabilidad esperada y seguridad de la inversión.
- Las Regiones 0 y 2 fueron descartadas debido a su mayor probabilidad de generar pérdidas.
- La Región 1 fue seleccionada como la alternativa más adecuada para el desarrollo de nuevos pozos petrolíferos.

## Habilidades demostradas

- Análisis exploratorio de datos.
- Modelos de regresión supervisada.
- Evaluación mediante RMSE.
- Simulación Monte Carlo y Bootstrap.
- Análisis de riesgo financiero.
- Cálculo de intervalos de confianza.
- Interpretación de métricas de negocio.
- Toma de decisiones basada en datos.

## Estructura del repositorio

```text
├── machine_learning_in_business.ipynb
├── README.md
├── data/
│   ├── geo_data_0.csv
│   ├── geo_data_1.csv
│   └── geo_data_2.csv
└── images/
```

## Autor

**Alejandro Cotes**  
Estudiante de Ciencia de Datos | Machine Learning | Analítica de Datos
