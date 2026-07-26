# Descripción de los Datos

## Obtención de datos 

### Space-Track

Mediante el [script](../src/space_track_api.py) se obtuvieron los datos de [Space-Track.org](https://www.space-track.org/). Se crearon los archivos [satellites.json](../data/raw/satellites.json), [debris.json](../data/raw/debris.json), [rockets.json](../data/raw/rockets.json) y [unknown.json](../data/raw/unknown.json). Estos archivos corresponde con la informacion de satélites, debris espaciales, cohetes de lanzamiento y objetos no identicados. 

Las columnas de los archivos son: 

| **Columna**        | **Descripción** |
|--------------------|---------------|
| **OBJECT_ID**      | Identificador único asignado por [NORAD](https://www.norad.mil/). |
| **OBJECT_TYPE**    | Tipo de objeto (payload, debris, rocket body). |
| **SATNAME**        | Nombre del objeto o satélite. |
| **COUNTRY**        | País responsable del objeto. |
| **LAUNCH**         | Fecha de lanzamiento. |
| **SITE**           | Lugar de lanzamiento. |
| **DECAY**          | Fecha de reentrada en la atmósfera (si corresponde). |
| **PERIOD**         | Período orbital en minutos. |
| **INCLINATION**    | Inclinacion con respecto al ecuador en grados. |
| **APOGEE**         | Altitud máxima de la órbita en km. |
| **PERIGEE**        | Altitud mínima de la órbita en km. |
| **RCS_SIZE**       | Tamaño estimado del objeto. |
| **LAUNCH_YEAR**    | Año de lanzamiento. |
| **LAUNCH_NUM**     | Número de lanzamiento de ese año. |
| **LAUNCH_PIECE**   | Letra que identifica cada objeto dentro de un mismo lanzamiento. |
| **CURRENT**        | Estado actual del objeto. |  

### Union of Concerned Scientists

[Union of Concerned Scientists](https://www.ucs.org/) proporciona una base de datos, que ayuda a complementar los datos anteriores en el archivo [ucs-satellite-database.xlsx](../data/raw/ucs-satellite-database.xlsx). Para más información leer la [guía de usuario](../data/User+Guide+1-1-17+wAppendix.pdf).

Las columnas del archivo son: 

| **Columna**                           | **Descripción**                                                                 |
|---------------------------------------|---------------------------------------------------------------------------------|
| **NORAD Number**                      | Identificador único asignado por NORAD. |
| **Current Official Name of Satellite** | Nombre oficial del satélite. |
| **Country of Operator/Owner**         | País del operador o propietario del satélite. |
| **Operator/Owner**                    | Nombre del operador o propietario del satélite. |
| **Users**                             | Entidades o países que utilizan el satélite. |
| **Purpose**                           | Propósito general del satélite. |
| **Class of Orbit**                    | Órbita en la que se encuentra el satélite. |
| **Launch Mass (kg.)**                 | Masa del satélite en el momento del lanzamiento. |
| **Expected Lifetime (yrs.)**          | Vida útil esperada. |
| **Country of Contractor**             | País donde se encuentra el fabricante. |
| **Launch Site**                       | Sitio del lanzamiento. |
| **Launch Vehicle**                    | Lanzador. |  

El uso de estas dos fuentes de datos permite obtener información sobre:  
- Tamaño y masa de los satélites.  
- Órbita según el período orbital.  
- Propósito de cada satélite.  
- Vida útil esperada de los satélites.  

##
<p align="right">Siguiente | <b><a href="analisis_y_visualizacion.md">Análisis y Visualización</a></b>
<br/>
Atrás | <b><a href="intro_satelites.md">Introducción a los Satélites</a></p>

</b><p align="center"><sup> EnzoRg | </sup><a href="../README.md"><sup>Contenidos</sup></a></p>