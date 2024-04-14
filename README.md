# Proyecto: Análisis de Homicidios por Siniestros Viales en CABA (2016 - 2021)

## Bienvenido al proyecto.
¡Hola! Soy David Marimón y soy el desarrollador de este repositorio. 

Quiero darte la bienvenida al trabajo realizado para este segundo proyecto individual dentro de la etapa de Labs de mis estudios con Henry. Para el desarrollo del proyecto, se tomó como base la [información](https://data.buenosaires.gob.ar/dataset/victimas-siniestros-viales) proporcionada por la Secretaría de Transporte del Gobierno de la Ciudad Autónoma de Buenos Aires respecto a los datos sobre homicidios por siniestros viales entre el año 2016 y el año 2021 ocurridos en la Ciudad Autónoma de Buenos Aires (CABA). El dataset incluye información sobre cada siniestro vial, como la fecha, la hora, la ubicación, los vehículos involucrados y las víctimas.

## Propósito:

Este proyecto tiene como objetivo analizar los datos sobre homicidios por siniestros viales en CABA entre los años 2016 y 2021, con el propósito de identificar patrones y tendencias que puedan ayudar a desarrollar estrategias para reducir el número de muertes por accidentes de tránsito. Con esto en mente, y tras la revisión de la información, se sugieren 3 KPIs (*Key Performance Indicators*, o "Medidor Clave de Rendimiento" por su nombre en español) para medir el éxito de las medidas que se implementen para reducir el número de homicidios por siniestros viales

## Composición del repositorio:

Encontrás que el repositorio está compuesto de la siguiente manera: 
- **[Data](https://github.com/DaAnMaGi/Proyecto_Data_Abril/tree/main/Data/Corregidos)**: Contiene las bases de datos procesadas para el análisis. Estos son: 
    - hechos.csv: Información sobre cada siniestro vial (fecha, hora, ubicación, vehículos, víctimas).
    - víctimas.csv: Información detallada sobre cada víctima (rol, edad, sexo, etc.).
- **[Exploración y revisión de las bases de datos](https://github.com/DaAnMaGi/Proyecto_Data_Abril/tree/main/Revisi%C3%B3n_Bases)**: Ubicado en la carpeta "Revisión_Bases". Contiene el notebook de exploración y revisión de las bases de datos.
- **[Análisis y graficación](https://github.com/DaAnMaGi/Proyecto_Data_Abril/tree/main/Dashboard)**: Ubicado en la carpeta "Dashboard". Contiene el archivo de Power BI con las visualizaciones utilizadas que tienen la función de proporcionar todos los insights trabajados para el análisis.

## Datos:

Los datos utilizados en este proyecto provienen del dataset "Víctimas de Siniestros Viales" proporcionado por la Secretaría de [Transporte del Gobierno de la Ciudad Autónoma de Buenos Aires](https://data.buenosaires.gob.ar/dataset/victimas-siniestros-viales). El dataset incluye información sobre cada siniestro vial, como la fecha, la hora, la ubicación, los vehículos involucrados y las víctimas.

## Metodología:

La exploración, limpieza, transformación y análisis de los datos se realizó utilizando las siguientes herramientas:

- **Python**: Lenguaje de programación a través del cual se realizó la extracción, limpieza y transformación de los datos.
- **Pandas**: Librería de Python, usada para el análisis y manipulación de los datos.
- **Matplotlib**: Librería de Python, usada justo a Seaborn para la visualización y exploración de los datos.
- **Seaborn**: Librería de Python. se utilizó para la visualización de datos.
- **Power BI Desktop**: Herramienta de inteligencia empresarial desarrollada por Microsoft. Se utilizó la versión de escritorio para la creación de las visualizaciones usadas para el análisis de los datos.

## Flujo de Trabajo:

- **Importación de datos**: Se descargaron los [datos originales](https://data.buenosaires.gob.ar/dataset/victimas-siniestros-viales) proporcionados por la Secretaría de Transporte del Gobierno de la Ciudad Autónoma de Buenos Aires.
- **Revisión y preparación de datos**: En [apertura_bases.ipynb](https://github.com/DaAnMaGi/Proyecto_Data_Abril/blob/main/Revisi%C3%B3n_Bases/apertura_bases.ipynb), se exploran los datos proporcionados por la Secretaría de Transporte, se revisa la base de datos para encontrar anomalías, se toman medidas para limpiar y preparar las bases de datos, y se grafican los datos para conocer la composición del dataset tras su transformación. Para ello, se utiliza Python haciendo uso de las librerías Pandas, Matplotlib y Seaborn.
- **Análisis y visualización**: En [Análisis.pbix](https://github.com/DaAnMaGi/Proyecto_Data_Abril/tree/main/Dashboard) se utiliza Power BI para crear las visualizaciones que proporcionen la información necesaria para realizar el análisis. El archivo está compuesto de las siguientes hojas:
    - **Intro**: Donde se aborda el contexto del problema, el propósito del análisis y los KPIs que se proponen para el análisis.
    - **Descripción**: Donde se observa la descripción de los hechos por homicidios en siniestros viales en CABA.
    - **Exploración - Víctimas**: Visualización sobre la composición de las víctimas. 
    - **Clasificación - Víctimas**: Profundización sobre la composición de las víctimas.
    - **Evolución - KPIs**: Visualización de la evolución de los KPIs sugeridos. 

## Algunos datos clave - Resultados:

De acuerdo con la exploración, visualización y análisis de los datos, me gustaría resaltar los siguientes puntos:

- Los motociclistas son el grupo de víctimas más vulnerable, seguido de los peatones y los ocupantes de automóviles:
    - Para los dos primeros grupos, en la mayoría de los accidentes se identifica como tipo de acusado a los autos, los pasajeros y vehículos de carga. 
    - Para el caso donde la víctima fue un auto, en la mayoría de los accidentes se identifica como tipo de acusado a otros autos, a objetos fijos, vehículos de carga y a los pasajeros.
- El mayor número de de accidentes es causado por autos, seguido de los pasajeros y vehículos de carga.
    - Para los autos, la mayoría de las víctimas son motos y peatones. 
    - Para los pasajeros, la mayoría de las víctimas son peatones. 
    - para los vehículos de carga, la mayoría de las víctimas son motos y peatones.
- Los grupos poblaciones donde más se registran víctimas son:
    - De acuerdo con su sexo, los hombres. 
    - De acuerdo con su grupo etario, primero por las personas entre los 21 y los 30 años, seguidos de las personas entre 31 - 40 años, donde la tercera y cuarta posición son ocupadas por las personas entre 41 - 50 años y 51 - 60 años, respectivamente.
- Los siniestros viales ocurren con mayor frecuencia durante el segundo semestre del año, donde el 4 trimestre (los meses de octubre, noviembre, diciembre) es el trimestre donde más se registran siniestros para toda la base. 
- Se presentan picos en el número de siniestros que ocurren para el fin de semana (viernes y sábado) y el inicio de semana (lunes).
- El mayor número de siniestros viales ocurren entre la franja horaria de la mañana, entre las 3 a.m. y las 12 del medio día. Donde el mayor número de siniestros ocurren entre las 6:00 y las 9 a.m.
- El mayor número de siniestros viales, por ubicación, ocurren en:
    - Por comunas, en orden descendente: 1, 4, 9 y 8.
    - Por tipo de calle, en las Avenidas y en las Calles.
    - Por tipo de vía (es o no es un cruce), en los cruces.

## KPIs:

Se proponen tres KPIs (Key Performance Indicators) para medir el éxito de las medidas que se implementen para reducir el número de homicidios por siniestros viales:

- Reducción en un 10% de la tasa de homicidios en siniestros viales de los últimos seis meses, en comparación con la tasa de homicidios en siniestros viales del semestre anterior (resumido como "KPI Tasa de Homicidios"). Se entiende a la tasa de homicidios en siniestros viales como número de víctimas fatales en accidentes de tránsito por cada 100,000 habitantes en un área geográfica durante un período de tiempo específico. Su fórmula es: (Número de homicidios en siniestros viales / Población total) * 100,000
- Reducir en un 7% la cantidad de accidentes mortales de motociclistas en el último año, en CABA, respecto al año anterior (resumido como "KPI Accidentes Motos"). Donde se define a la cantidad de accidentes mortales de motociclistas en siniestros viales como el número absoluto de accidentes fatales en los que estuvieron involucradas víctimas que viajaban en moto en un determinado periodo temporal.
- Reducir en un 10% la cantidad de accidentes mortales ocurridos en cruces, en CABA, respecto al año anterior (resumido como "KPI Accidentes Cruces"). Donde se define a la cantidad de accidentes mortales ocurridos en cruces como el número absoluto de accidentes fatales ocurridos en tipos de vías clasificadas como cruces en un determinado periodo temporal.

## Análisis de los KPIs:

Para los 3 KPIs, la fórmula utilizada para medir la evolución (o tasa de evolución) fue la siguiente: 
```
(([Indicador del periodo anterior] - [Indicador del periodo actual]) / [Indicador del periodo anterior]) * 100
```

Donde, para el último periodo registrado (segundo semestre del 2021), se tenía que:
- Se estaba cumpliendo la reducción establecida para "Tasa de Homicidios".
- No se estaba cumpliendo la reducción establecida para "Accidentes Motos".
- No se estaba cumpliendo la reducción establecida para "Accidentes Cruces".