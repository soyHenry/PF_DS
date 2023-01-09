# <b>Proyecto Grupal: Flujos migratorios</b>

![img](https://i.imgur.com/2gHG5uz.png)  

<hr>  

## <b>Descripción del problema</b> (Contexto y rol a desarrollar)  

### <b>Contexto</b>  

Los procesos y flujos migratorios entre sociedades, aunque puedan parecer un fenómeno
actual, se han dado a lo largo de toda la historia de la humanidad. La globalización y el avance en los medios de transporte han permitido generar flujos migratorios internacionales continuos y, en ocasiones, muy importantes, que dan forma y cambian constantemente la sociedad actual a un ritmo mucho mayor que hace siglos.
Este proyecto se centrará en estudiar y analizar el porqué de tales flujos migratorios en el contexto actual.

La idea principal es documentar cómo y por qué, estos cambios pueden estar sujetos a distintas problemáticas como el contexto socioeconómico de los países/regiones, conflictos bélicos, la calidad de vida, entre otros factores.

### <b>Rol a desarrollar</b>  

Tu equipo/consultora es contratado por una ONG internacional, con el fin de estudiar los
flujos migratorios y su impacto en diversos aspectos de los países afectados. Para ello, deben crear toda una solución de datos (data pipeline, bases de datos, data warehouse, dashboard, modelos predictivos, etc.) para poder comunicar eficazmente la relación de las migraciones humanas con los distintos aspectos socioeconómicos y geopolíticos.   

<hr>  

## <b>Indicaciones</b>  

Deberán realizar un estudio puntual de cada uno de los datasets utilizados y presentar lo siguiente:

- Análisis exploratorio de los datos (EDA). Reporte de calidad de datos (datos faltantes, outliers, valores nulos), el criterio utilizado para su manejo, además de un diccionario de datos.  

- Data Pipeline para el ETL  

- Proponer al menos 4 KPIs  

- Base de datos (DB), data warehouse (DW) y data lake. Debe estar corriendo de manera local o en un proveedor de servicios en la nube (AWS, GCP, Azure, etc).  

- Automatización del flujo de trabajo (Airflow, NiFi o similares).  

- Dashboard con los datos más relevantes para la creación de un storytelling.

- Uso de modelos de Machine Learning para predecir olas migratorias en los próximos años.  

- Diagrama con la arquitectura de datos utilizada donde se visualice el nombre de las herramientas utilizadas. Revisen el siguiente ejemplo de diagrama.

- Todo el trabajo debe incluirse en un repositorio de Github, donde crearan un archivo Readme que explique de manera resumida el trabajo realizado.  
<small><b>Nota</b>: el Readme utilizado para su repositorio no debe ser el de las consignas del Proyecto Grupal.</small>  

- El proyecto además debe estar documentado en un archivo .doc o .pdf, donde puedan desarrollar el avance de su proyecto semana a semana, explicando qué tecnologías utilizan, quiénes son los miembros del equipo, cuáles son los productos a presentar, estimaciones de esfuerzos semana a semana y todo lo que deseen comunicar sobre su proyecto.  

### <b>Alcance</b>  

Como grupo tienen la libertad de elegir los países que quieran analizar. Pueden ser flujos
globales, tener en cuenta sólo determinados países o regiones (por ejemplo, migraciones
dentro de América Latina), balanza de migración de un país/ países en particular, migración intra-estados/ provincial y su comparación con la inmigración/ emigración de ese mismo país (por ejemplo, estudiar cómo migran las personas dentro de Estados Unidos, y donde se asientan los inmigrantes que eligen a EUA como su destino para vivir).
El período de tiempo no tiene restricción alguna, sientanse libres de elegir el que más les interese.

### <b>Indicadores</b>  

Los indicadores que se pueden tomar en cuenta son de libre elección pero deben responder a las necesidades del proyecto. Estos les ayudarán para dar un mayor respaldo a los datos que recaben e intenten vender como consultora. Por ejemplo, económicos (PIB), calidad de vida, esperanza de vida, costo de vida en países (con cuántos dólares se puede vivir al día), acceso a educación, acceso a salud, efectos de los conflictos armados en los flujos migratorios, etc.  

<hr>  

## <b>Datasets</b>  

Del siguiente [sitio web](https://datos.bancomundial.org/indicator/SM.POP.NETM?end=2017&start=1962) pueden tomar los archivos CSV como principal fuente para sus bases de datos. A su vez, deben complementarlo con al menos tres fuentes de datos adicionales, para ello pueden utilizar información de otros sitios (datasets, APIs, etc.) como las que están detalladas abajo o cualquiera que puedan encontrar en internet relacionadas al tema.

### <b>Fuente principal</b>  

[Banco mundial](https://datos.bancomundial.org/indicator/SM.POP.NETM?end=2017&start=1962) 

### <b>Fuentes complementarias</b>  

- [Our world in data](https://ourworldindata.org/) 
- [The world bank](https://datacatalog.worldbank.org/) 
- [Portal de datos sobre migración](https://www.migrationdataportal.org/es/international-data?i=stock_abs_&t=2020)  
- [International Migrant Stock](https://www.un.org/development/desa/pd/content/international-migrant-stock)
- [Datos argentina](https://www.datos.gob.ar/dataset/interior-ingresos-egresos-personas-al-pais-residencias-otorgadas)
- [Instituto Nacional de Estadística y Geografía- Datos abiertos- México](https://en.www.inegi.org.mx/datosabiertos/)
- [County-to-County Migration Flows: 2015-2019 ACS](https://www.census.gov/data/tables/2019/demo/geographic-mobility/county-to-county-migration-2015-2019.html)
- [Migración - ONU](https://www.un.org/es/global-issues/migration#:~:text=En%202020%20el%20número%20de,164%20millones%20son%20trabajadores%20migrantes.)
- [Informe sobre las migraciones en el mundo 2020](https://worldmigrationreport.iom.int/wmr-2020-interactive/?lang=ES) 

La lista no es exhaustiva, y de ninguna manera deben restringirse a sólo utilizar estas fuentes, pueden utilizar cualquier otra fuente de datos relacionada al tema que sume positivamente al proyecto.

Te recomendamos el uso de APIs para obtener datos adicionales para este proyecto, como podrían ser de clima (dato muy importante son las condiciones climáticas extremas, por ejemplo, en países que estén atravesando grandes sequías, relaciones entre temperatura promedio entre países que reciben migrantes o países desde donde migran, o las condiciones generales no favorezcan el desarrollo "pleno" para sus habitantes).

<hr>

## <b>Lineamientos a evaluar</b>


[En este archivo se detalla lo que esperamos de ustedes semana tras semana](https://docs.google.com/document/d/13yU2EQ6eCFdESCwuP8pINDENgTCQCFEzSmVKqX98OL8/edit?usp=share_link)
<hr>  

## `Disclaimer`
De parte del equipo de Henry se aclara y remarca que el fin de los proyectos propuestos es exclusivamente pedagógico, con el objetivo de realizar simular un entorno laboral, en el cual se trabajan diversas temáticas ajustadas a la realidad. No reflejan necesariamente la filosofía y valores de la organización. Además, Henry no alienta ni tampoco recomienda a los alumnos y/o cualquier persona leyendo los repositorios (y entregas de proyectos) que tomen acciones con base a los datos que pudieran o no haber recabado. Toda la información expuesta y resultados obtenidos en los proyectos nunca deben ser tomados en cuenta para la toma real de decisiones (especialmente en la temática de finanzas, salud, política, etc.).
