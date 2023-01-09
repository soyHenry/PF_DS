# Proyecto Grupal: E-commerce Olist  

![img](https://epiprodux.com/blog/wp-content/uploads/2022/02/Ecommerce-managers-Role.jpg)  

## <b>Descripción del problema (Contexto y rol a desarrollar)</b>

### <b>Contexto</b>

En 2021, la venta minorista de productos a través de e-commerce significó un saldo aproximado de 5.2 trillones de dólares en todo el mundo y se infiere que dicha cifra aumentará un 56% en los próximos años, llegando a los 8.1 trillones en 2026.

Olist es una compañía brasileña prestadora de servicio e-commerce para PYMES que funciona como un marketplace, es decir, funciona como “tienda de tiendas” donde diferentes vendedores pueden ofrecer sus productos a consumidores finales.  

### <b>Rol a desarrollar</b>  

Con el objetivo primordial de seguir conectando a pequeñas empresas (PYMES) con mercados más grandes y mejorar la experiencia del usuario, Olist los contrata como consultores externos para encontrar soluciones innovadores que permitan a sus usuarios vender sus productos a un mayor número de clientes.  
Para lograrlo, les disponibiliza sus datos de 2016 a 2018 con lo que deberán entregar un MVP <i>(minimum viable product)</i>.  

## <b>Propuesta de trabajo</b> (indicaciones)  

- `Recopilar, depurar y disponibilizar la información`: 
    - Deben realizar un Análisis exploratorio de datos (EDA) y elaborar un reporte de calidad de datos (datos faltantes, outliers, valores nulos), el criterio utilizado para su manejo, además de un diccionario de datos.
    - Data Pipeline para el ETL
    - Creación de base de datos (DataWarehouse) de los diferentes csv provistos y las fuentes alternativas que fueren incorporadas por ustedes. Debe estar corriendo de manera local o en un proveedor de servicios en la nube (AWS, GCP, Azure, etc)
    - Automatización del flujo de trabajo (Airflow, NiFi o similares). 

- `Reporte y análisis significativos`: Un dashboard que brinde información concisa para la toma de decisiones de negocio brindando métricas y al menos 2 KPIs claves para el buen desempeño y mejora del e-commerce (ver ideas de analisis e implementacion).

- `Entrenamiento y puesta en producción de un modelo de machine learning`: Pueden implementar un modelo de recomendación de productos o un modelo de análisis de sentimiento sobre reviews.

## Ideas de analisis e implementación  

Solo a modo de disparadores, pueden divagar y proponer lo que se les ocurra, su mente es el límite!

- `Incorporación de Hubs`: Si se abrieran centros físicos para almacenar productos, cuáles serían los mejores lugares para emplazarlos? Qué productos se recomienda tener con constante stock debido a su venta?

- `Distribución geográfica del negocio`: en donde resulta más conveniente vender cada producto?

- `Optimización del DataWarehouse`: Existe un gran número de quejas de los sellers respecto a ordendes no completadas debido a la diferencia entre el stock real y productos publicados, ¿cómo se podria mejorar y brindarles herramientas de actualización del inventario individual? 

- `Marketing`: Identificar patrones en los marketing leads cerrados para mejorar estrategias de conversión de clientes (sellers)

## <b>Datasets y fuentes complementarias</b>  

### <b>Fuentes obligatorias</b>  

- [Dataset Olist](https://drive.google.com/file/d/1YiZqsF_F4OIdjLCq4sba2XXjPxU7LlgE/view?usp=sharing)

### <b>Fuente de datos alternativas</b>

- Pueden utilizar fuentes de datos complementarias que consideren pertinentes al proyecto.

## Material de apoyo  

- [ML for recommender systems](https://medium.com/recombee-blog/machine-learning-for-recommender-systems-part-1-algorithms-evaluation-and-cold-start-6f696683d0ed)

## `Disclaimer`
De parte del equipo de Henry se aclara y remarca que el fin de los proyectos propuestos es exclusivamente pedagógico, con el objetivo de realizar simular un entorno laboral, en el cual se trabajan diversas temáticas ajustadas a la realidad. No reflejan necesariamente la filosofía y valores de la organización. Además, Henry no alienta ni tampoco recomienda a los alumnos y/o cualquier persona leyendo los repositorios (y entregas de proyectos) que tomen acciones con base a los datos que pudieran o no haber recabado. Toda la información expuesta y resultados obtenidos en los proyectos nunca deben ser tomados en cuenta para la toma real de decisiones (especialmente en la temática de finanzas, salud, política, etc.).

