![HenryLogo](https://d31uz8lwfmyn8g.cloudfront.net/Assets/logo-henry-white-lg.png)

# <h1 align="center">**`Proyecto Grupal XX`**

- - -

# <h1 align="center">**`Flujos Migratorios`**

<p align="center">
<img src="https://www.flippers.es/wp-content/uploads/2014/03/Flujos-migratorios-internacionales.jpg"   
>
</p>

## **Contexto**
Los procesos y flujos migratorios entre sociedades, aunque puedan parecer un fenómeno puramente actual, se han dado a lo largo de toda la historia de la humanidad. En este proyecto, lo que nos va a interesar, va a ser estudiar y analizar el porque de tales flujos migratorios (sobre todo en el contexto actual). La globalización y el avance en los medios de transporte han permitido generar flujos migratorios internacionales continuos y, en ocasiones, muy importantes, que dan forma y cambian constantemente la sociedad actual a un ritmo mucho mayor que hace siglos.    
     
   
La idea es plasmar como y, hasta cierto punto, porqué, estos cambios puedan estar sujetos a distintas problemáticas como el contexto socioeconómico de los países/regiones, conflictos bélicos, la calidad de vida, como muchos otros factores.
   


:earth_americas: 	:earth_africa: :earth_asia: **Rol a desarrollar:** El equipo/ consultora es contradado por una ONG internacional, con el fin de estudiar esos flujos migratorios, y como impactan en distintos aspectos de los países que se analicen. Para ello, deben crear toda una solución de datos (data pipeline, base de datos, data warehouse, dashboard, modelos predictivos, etc) para poder comunicar eficazmente la relación de las migraciones humanas con los distintos aspectos socieconómicos y geopolíticos.  

:airplane: :ship: :earth_africa: **Indicaciones:**
Deberán hacer un estudio pormenorizado de cada uno de los datasets utilizados y presentar lo siguiente:

- Análisis exploratorio de los datos (EDA): Reporte de calidad de datos (datos faltantes, outliers, valores nulos), criterio utilizado para su manejo, junto con un diccionario de datos.
- Data Pipeline para el ETL. [¿Qué es un ETL?](https://learn.microsoft.com/es-es/azure/architecture/data-guide/relational-data/etl)
- Proponer al menos 4 KPIs. [¿Qué es un KPI?](https://asana.com/es/resources/key-performance-indicator-kpi)
- Base de datos (DB), Datawarehouse (DW) con su Datalake, todo corriendo en local o bien en un proveedor de servicios en la nube (AWS, GCP, MS Azure, etc).
- Automatización del flujo de trabajo (Airflow, NiFi o similares). 
- Dashboard con los datos más relevantes para su storytelling.
- Uso de modelos de Machine Learning para predecir olas migratorias en los próximos años.
- Diagrama con la arquitectura de datos utilizada donde se visualice el nombre de las herramientas utilizadas. [Diagrama de ejemplo](https://learn.microsoft.com/en-us/azure/architecture/solution-ideas/articles/azure-databricks-modern-analytics-architecture)

Todo el trabajo debe incluirse en un repositorio de Github, donde crearán un archivo README que explique de manera resumida el trabajo realizado. Resulta menester aclarar que el README utilizado para su repositorio no debe ser el de las consignas del Proyecto Grupal. Todo además debe estar documentado en un archivo .doc o .pdf aparte, donde puedan desarrollar el avance de su proyecto semana a semana, explicando qué tecnologías utilizaron, quiénes son los miembros del equipo, cuáles son los productos a presentar, estimaciones de esfuerzos semana a semana y todo lo que deseen comunicar sobre su proyecto.


:airplane: :ship: :tram: **Alcance:** Como grupo tienen la libertad de elegir los países que quieran analizar. Pueden ser flujos globales, tener en cuenta solo determinados países o regiones (por ejemplo migraciones dentro de América Látina), balanza de migración de un país/ países en particular, migración intra estados/ provincial y su comparación con la inmigración/ emigración de ese mismo país (por ejemplo, estudiar como migran las personas dentro de Estados Unidos, y donde se asientan los inmigrantes que eligen a USA como su destino para vivir).   
Además, pueden seleccionar el período de tiempo que más les interese: hasta 2022, entre 2015 y 2022, 1970 a 2010, etc.
       
:house: :house_with_garden: :school: **Indicadores:** Los indicadores que pueden tomar en cuenta, son también de libre elección como el alcance del proyecto, y les van a servir para dar un mayor respaldo a los datos que recaben e intenten vender como consultora. Por ejemplo: económicos (PBI), de medición de calidad de vida, de esperanza de vida, de costo de vida en países (con cuantos dólares -o centavos de dólar- se puede vivir al día), de acceso a educación, de acceso a salud, efectos de los conflictos armados en los flujos migratorios, etc.



## **Datasets**
Del siguiente sitio web pueden tomar los archivos CSV como principal fuente para sus bases de datos. A su vez, deben complementarlo con al menos 3 fuentes de datos adicionales, para ello pueden utilizar información de otros sitios (datasets, APIs, etc) como las que están detalladas debajo o cualquiera que puedan encontrar en la web, relacionadas al tema. 
- Fuente principal: https://datos.bancomundial.org/indicator/SM.POP.NETM?end=2017&start=1962

### **Fuentes complementarias y material de apoyo**
La lista no es exhaustiva, y de ninguna manera deben restringirse a sólo utilizar estas fuentes, pueden utilizar cualquier otra fuente de datos que encuentren en Internet relacionada al tema y que quieran integrar al proyecto.

- https://ourworldindata.org/
- https://datacatalog.worldbank.org/
- https://www.migrationdataportal.org/es/international-data?i=stock_abs_&t=2020
- https://www.un.org/development/desa/pd/content/international-migrant-stock
- https://www.datos.gob.ar/dataset/interior-ingresos-egresos-personas-al-pais-residencias-otorgadas
- https://www.census.gov/data/tables/2019/demo/geographic-mobility/county-to-county-migration-2015-2019.html
- https://www.un.org/es/global-issues/migration#:~:text=En%202020%20el%20n%C3%BAmero%20de,164%20millones%20son%20trabajadores%20migrantes.
- https://worldmigrationreport.iom.int/wmr-2020-interactive/?lang=ES
- https://databank.worldbank.org/source/population-estimates-and-projections
- https://databank.worldbank.org/source/world-development-indicators
- https://databank.worldbank.org/source/global-bilateral-migration
   
*Recomendamos el uso de API's para obtener datos adicionales para este proyecto, como podrían ser de clima (mucho muy importante son las condiciones climáticas extremas, por ejemplo, en países que estén atravesando grandes sequías, relaciones entre temperatura promedio entre países que reciben migrantes o países desde donde migran, o las condiciones generales no favorezcan el desarrollo "pleno" para sus habitantes).  


## Disclaimer  
De parte del equipo de Henry se quiere aclarar y remarcar que los fines de los proyectos propuestos son exclusivamente pedagógicos, con el objetivo de realizar proyectos que simulen un entorno laboral, en el cual se trabajen diversas temáticas ajustadas a la realidad.
 No reflejan necesariamente la filosofía y valores de la organización. Además, Henry no alienta ni tampoco recomienda a los alumnos y/o cualquier persona leyendo los repositorios (y entregas de proyectos) que tomen acciones en base a los datos que pudieran o no haber recabado. Toda la información expuesta y resultados obtenidos en los proyectos, nunca deben ser tomados en cuenta para la toma real de decisiones (especialmente en la temática de finanzas, salud, política, etc.).
