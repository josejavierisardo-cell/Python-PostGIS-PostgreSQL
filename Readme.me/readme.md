# <h1 align="center">Análisis de datos y análisis geoespacial de los centros sanitarios de Madrid</h1>

## Descripción

<p style="text-align: justify;">Este proyecto analiza la oferta sanitaria de Madrid a partir de un conjunto de datos públicos, combinando análisis exploratorio, tratamiento de datos y técnicas de análisis geoespacial.</p>

<p style="text-align: justify;">El proyecto se desarrolla en tres fases, evolucionando desde el análisis inicial de los datos hasta el uso de PostgreSQL y PostGIS para realizar consultas y análisis espaciales.</p>

<p style="text-align: justify;">El objetivo es obtener una visión de la distribución y características de los centros sanitarios, así como analizar su relación con el territorio.</p>

## Objetivos
- Explorar y preparar los datos de los centros sanitarios.
- Analizar los diferentes tipos de centros existentes.
- Estudiar su distribución territorial por barrios.
- <p style="text-align: justify;">Analizar la disponibilidad de información sobre accesibilidad, horarios, equipamiento y transporte.</p>
- Incorporar información geográfica mediante GeoPandas.
- Analizar distancias y proximidad entre centros.
- Relacionar espacialmente los centros sanitarios con los distritos de Madrid.
- Integrar Python con una base de datos espacial PostgreSQL/PostGIS.

## Proyecto
*<u>1 · Análisis exploratorio</u>*

**Python · Pandas**

Se realiza la exploración, limpieza y preparación del conjunto de datos.

<p style="text-align: justify;">Se analizan los tipos de centros sanitarios, su distribución por barrios y la disponibilidad de información sobre diferentes características de los centros.</p>

277 centros sanitarios · 8 tipos · 116 barrios

*<u>2 · Análisis geoespacial</u>*

**GeoPandas · Matplotlib**

<p style="text-align: justify;">Se incorpora la componente geográfica al análisis mediante la transformación de las coordenadas de los centros en geometrías espaciales.</p>

<p style="text-align: justify;">Se validan las geometrías, se trabajan los sistemas de referencia y se generan representaciones cartográficas para estudiar la distribución espacial de los centros.</p>

*<u>3 · PostgreSQL + PostGIS</u>*

**PostgreSQL · PostGIS · SQLAlchemy · GeoAlchemy2**

Se crea una base de datos espacial para almacenar y analizar los centros sanitarios y los distritos de Madrid.

Se realizan consultas SQL y espaciales para:

- Analizar los tipos de centros.
- Calcular distancias y proximidades.
- Utilizar índices espaciales GiST.
- Relacionar centros y distritos mediante ST_Within.
- Recuperar los resultados con GeoPandas.
- Representar cartográficamente los resultados.

277 centros sanitarios · 21 distritos

## Conclusión

<p style="text-align: justify;">El proyecto muestra un flujo de trabajo completo aplicado al análisis de información sanitaria y geográfica: desde la exploración y preparación de los datos, pasando por su representación espacial, hasta su almacenamiento y análisis mediante una base de datos espacial.</p>

<p style="text-align: justify;">La combinación de Python, GeoPandas, PostgreSQL y PostGIS permite trabajar con los datos desde diferentes perspectivas y obtener resultados tanto analíticos como cartográficos.</p>