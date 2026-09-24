# Análisis espacial del sistema sanitario de Madrid
## Descripción

<p style="text-align: justify;"> En esta parte del proyecto se amplía el análisis de los centros sanitarios de Madrid mediante el uso de PostgreSQL y PostGIS.</p>

<p style="text-align: justify;"> El objetivo es almacenar, consultar y analizar la información geográfica de los centros sanitarios y estudiar su relación espacial con los distritos de Madrid.</p>

## Objetivos

El análisis busca principalmente:

- Integrar los datos geográficos en una base de datos espacial.
- Realizar consultas SQL sobre los centros sanitarios.
- Analizar distancias y proximidad respecto a un punto de referencia.
- Relacionar espacialmente los centros sanitarios con los distritos de Madrid.
- Recuperar y visualizar los resultados mediante GeoPandas.
## Metodología
1. Importar las librerias 
2. Cargar el CSV
3. Crear el geodataframe con las coordenadas
4. Validar las geometrías
5. Conectar a la base de datos PostgreSQL
6. Cargar el GeoDataFrame en PostGIS
7. Comprobar que la tabla se ha creado correctamente
8. Comprobar índice espacial
9. Consulta SQL de los centros por tipo
10. Consulta espacial de los centros cercanos a un punto
11. Analisis de proximidad 
12. Relacionar los centros sanitarios con los distritos de Madrid
13. Recuperar los resultados con Geopandas (GeoDataFrame)
14. Comprobar los resultados obtenidos en un mapa
## Principales resultados

<p style="text-align: justify;">El análisis parte de 277 centros sanitarios, clasificados en 8 categorías diferentes, y 21 distritos de Madrid.</p>

<p style="text-align: justify;">La categoría más frecuente corresponde a los Centros de Salud, con 130 centros.</p>

<p style="text-align: justify;">Mediante el análisis de distancias se obtuvo una distancia mínima de aproximadamente 377 metros, una distancia media de 5,04 km y una distancia máxima de aproximadamente 13,71 km respecto al punto de referencia utilizado.</p>

<p style="text-align: justify;">Los centros se clasificaron además según diferentes rangos de proximidad:</p>

- 6 centros a menos de 1 km.
- 135 centros entre 1 y 5 km.
- 136 centros a más de 5 km.

<p style="text-align: justify;">Por otra parte, el análisis espacial mediante ST_Within permitió asignar los 277 centros sanitarios a los 21 distritos de Madrid, obteniendo el número de centros correspondiente a cada distrito.</p>

<p style="text-align: justify;">Finalmente, los resultados obtenidos mediante PostGIS se recuperaron con GeoPandas y se representaron cartográficamente, permitiendo visualizar conjuntamente los centros sanitarios y los límites de los distritos.</p>

## Tecnologías

<p style="text-align: justify;">Python · Pandas · GeoPandas · Matplotlib · PostgreSQL · PostGIS · SQLAlchemy · GeoAlchemy2 · Jupyter Notebook.</p>