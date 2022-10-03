![HenryLogo](https://d31uz8lwfmyn8g.cloudfront.net/Assets/logo-henry-white-lg.png)

# **PROYECTO GRUPAL Nº2**

- - -


# <h1 align="center">**`AMAZON REVIEWS`**</h1>



<a href="https://www.freepnglogos.com/pics/amazon-png-logo-vector" title="Image from freepnglogos.com"><img src="https://www.freepnglogos.com/uploads/amazon-png-logo-vector/amazon-symbol-png-logo-vector-9.png" width="400" alt="amazon symbol png logo vector" /></a>


</center>



## **Contexto**

El portal de compras Amazon, uno de los más grandes e importantes del mundo (no miren a China) está estudiando nuevas estrategias para poder mejorar sus ventas y mantener su posición dominante en el mercado estadounidense. Para ello, ha decidido contratar los servicios de una empresa externa (a nosotros) para apostar por el talento nuevo con ideas frescas y así obtener resultados con pensamientos 'fuera de la caja'.



<center> <img src ="https://c.tenor.com/rGDa5cD4zV8AAAAC/simpsons-caja.gif" height = 200></center>



  Nuestro trabajo sería analizar toda la información de reseñas y metadata relacionadas de datos históricos que nos proveen para extraer insights para la empresa, con análisis de ventas y reseñas, además de crear un modelo de recomendaciones de productos para ofrecer a los usuarios que pueda ayudar a mejorar las ventas de la empresa.
 

  Un modelo o sistema de recomendación es una herramienta que establece un conjunto de criterios y valoraciones sobre los datos de los usuarios para realizar predicciones sobre recomendaciones de elementos que puedan ser de utilidad o valor para el usuario. Estos sistemas seleccionan datos proporcionados por el usuario de forma directa o indirecta, y procede a analizar y procesar información del historial del usuario para transformar estos datos en conocimiento de recomendación.
 

  Todo el proyecto debe ser realizado con una arquitectura de datos de diseño propio, con data pipelines que puedan ingestar datos nuevos a nuestra base de datos y un dashboard que muestre todos los datos relevantes a los ejecutivos de la empresa para poder tomar decisiones rápidamente, por lo que la infraestructura del proyecto debe ser muy eficiente al manejar grandes cantidades de datos.


  Se puede trabajar descargando los datos de las categorías que crean necesarias, pueden seccionarlo a su conveniencia, no es necesario trabajar con todo el dataset completo. 

- - -



## **Propuestas para este proyecto**

+ Analizar las reseñas de los clientes para extraer información útil a la empresa. (NLP o lo que consideren pertinente)
+ Generar un sistema de recomendación de compras futuras para los clientes (para ello hay reseñas, info sobre productos frecuentemente comprados juntos, puntajes, etc).
+ Pueden agregar cualquier otro producto al proyecto que consideren útil.
+ Es enorme la cantidad de datos disponible, sugerimos crear arquitecturas de datos escalables.

- - -

## **Datasets**


24 tablas (una por categoría de producto) con datos de puntaje, productos comprados juntos, reseñas, etc., sobre productos de Amazon, recolectados desde 1996 hasta 2014            (20gb de datos, se puede seccionar). Contiene 142.8 millones de reviews y 3.1gb de metadata (precios, marca, descripción, etc). 



### **Categoría y link de descarga**
Books http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Books_5.json.gz

Electronics http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Electronics_5.json.gz

Movies and TV http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Movies_and_TV_5.json.gz

CD and Vinyl http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_CDs_and_Vinyl_5.json.gz

Clothing, Shoes and Jewelry http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Clothing_Shoes_and_Jewelry_5.json.gz

Home and Kitchen http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Home_and_Kitchen_5.json.gz

Kindle Store http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Kindle_Store_5.json.gz

Sports and Outdoors http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Sports_and_Outdoors_5.json.gz

Cell Phones and Accesories http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Cell_Phones_and_Accessories_5.json.gz

Health and Personal Care http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Health_and_Personal_Care_5.json.gz

Toys and Games http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Toys_and_Games_5.json.gz

Video Games http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Video_Games_5.json.gz

Tools and Home Improvement http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Tools_and_Home_Improvement_5.json.gz

Beauty http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Beauty_5.json.gz

Apps for Android http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Apps_for_Android_5.json.gz

Office Products http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Office_Products_5.json.gz

Pet Supplies http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Pet_Supplies_5.json.gz

Automotive http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Automotive_5.json.gz

Grocery and Gourmet Food http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Grocery_and_Gourmet_Food_5.json.gz

Patio, Lawn and Garden http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Patio_Lawn_and_Garden_5.json.gz

Baby http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Baby_5.json.gz

Digital Music http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Digital_Music_5.json.gz

Musical Instruments http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Musical_Instruments_5.json.gz

Amazon Instant Video http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Amazon_Instant_Video_5.json.gz



### **Metadata**
http://snap.stanford.edu/data/amazon/productGraph/metadata.json.gz



- - -


## **Diccionario de datos:**


### **Reseñas**
reviewerID - ID del usuario, ejemplo: A2SUAM1J3GNN3B.

asin - ID del producto, ejemplo: 0000013714.

reviewerName - nombre del usuario.

helpful - Puntaje de utilidad de la reseña (votos externos), e.g. 2/3.

reviewText - Texto de la reseña.

overall - Puntaje dado al producto.

summary - Resumen de la reseña.

unixReviewTime - Fecha de la reseña (unix time).

reviewTime - Fecha de la reseña .

### **Metadata de productos**
asin - ID del producto, ejemplo: 0000031852.

title - Nombre del producto.

price - Precio en dólares.

imUrl - URL de la imagen del producto.

related - Productos relacionados (comprados juntos, también revisados, comprados por el mismo usuario, comprados luego de verlos).

salesRank - Información sobre cómo rankea en ventas.

brand - Nombre de la marca del producto.

categories - Lista de la categoría a la que pertenece el producto.


- - -

¡¡¡Éxitos!!!

<img src ="https://media0.giphy.com/media/4ml290TZ35zOM/giphy.gif?cid=ecf05e47rskqdw9el7s6yr0cduw3vhiihfcukzoddna6zl4p&rid=giphy.gif&ct=g)" height = 200>

