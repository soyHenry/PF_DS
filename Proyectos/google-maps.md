![HenryLogo](https://d31uz8lwfmyn8g.cloudfront.net/Assets/logo-henry-white-lg.png)

# **PROYECTO GRUPAL Nº3**

- - -

# <h1 align="center">**`Google Maps REVIEWS AND RECOMMENDATIONS`**</h1>

<p align="center">
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/bd/Google_Maps_Logo_2020.svg/512px-Google_Maps_Logo_2020.svg.png"  height="200">
</p>


## **Contexto**

"Google posee una plataforma de reseñas de todo tipo de negocios, restaurantes, hoteles, servicios, entre otros. Los usuarios utilizan el servicio y luego suben su reseña según la experiencia vivida. Muchos usuarios leen las reseñas de los lugares a los que planean ir para tomar decisiones sobre dónde comprar, comer, dormir, reunirse, etc. Esta información es muy valiosa para las empresas, ya que les sirve para enterarse de la imagen que tienen los usuarios de los distintos locales de la empresa, siendo muy útil para medir el desempeño, utilidad del local, además de identificar los aspectos del servicio a mejorar. "


## **Rol a desarrollar**

"Como parte de una consultora de data, te han contratado para poder realizar un análisis del mercado estadounidense. El cliente es parte de un conglomerado de empresas de restaurantes y afines. Desean tener un análisis detallado de la opinión de los usuarios en Google Maps sobre hoteles, restaurantes y otros negocios afines al turismo y ocio. A partir del uso de análisis de sentimientos, predecir cuáles serán los rubros de los negocios que más crecerán (o decaerán). Además, desean saber dónde es conveniente establecer los nuevos locales de restaurantes y afines. Asimismo, desean poder tener un sistema de recomendación de restaurantes para los usuarios de Google para darle al usuario la posibilidad de poder conocer nuevos sabores a partir de sus experiencias previas. 
Nota: Pueden cambiar el tipo de comercio objetivo (no es necesario que sean restaurantes).
"

## **Propuesta de trabajo**

Recopilar, depurar y disponibilizar la información: Creación de una base de datos (DataWarehouse) de diferentes fuentes, tanto provistas por Henry como incorporadas por ustedes, corriendo en local o alojada en proveedores en la nube. La base de datos depurada deberá contemplar por lo menos dos tipos diferentes de extracción de datos, ejemplo: datos estáticos, llamadas a una API, scrapping, entre otros. 

Reporte y análisis significativos de la(s) línea(s) de investigación escogidas: El análisis debe contemplar las relaciones entre variables y concluir, si es que existe, una relación entre estas, y los posibles factores que causan dicha relación en la realidad. 

Entrenamiento y puesta en producción de un modelo de machine learning de clasificación no supervisado o supervisado: El modelo debe resolver un problema y conectar globalmente con los objetivos propuestos que se propongan como proyecto.
.

## **Ideas de análisis e implementación**


Mejoramiento de estrategias de marketing: campañas microsegmentadas

Sistemas de recomendación: Sobre algún lugar en particular, pueden ser comercios como restaurantes, hoteles, entre otros.

Datos adicionales a cruzar: Cotizaciones en bolsa, tendencias en redes sociales y medios de comunicación sobre comercios en expansíón.


- - -
## **Datasets y fuentes complementarias**


"Los datos son extraídos de la plataforma de reseñas de Google Maps en Estados Unidos. Tiene información sobre la ubicación de los comercios, su categoría, puntajes promedios, sobre los usuarios, las reseñas que hicieron, las respuestas que han recibido dichas reseñas entre otros. Se puede complementar el análisis con datasets adicionales que ofrezcan información que consideren pertinente al pedido (valores de acciones de las empresas, información geográfica adicional de los locales, etc). Recomendamos el uso de NLP para procesar la información de las reseñas. Tengan en cuenta que los datasets tienen un tamaño considerablemente grande, propongan una arquitectura de datos eficiente para su procesamiento."

### **Diccionario de datos**

El archivo donde se disponibiliza la metadata contiene información del comercio, incluyendo localización, atributos y categorías. Es un solo archivo 'all_meta.json.gz')

    // 'name': 'Walgreens Pharmacy', 
   
    // 'address': 'Walgreens Pharmacy, 124 E North St, Kendallville, IN 46755', 
  
    // 'gmap_id': '0x881614ce7c13acbb:0x5c7b18bbf6ec4f7e', 
 
    // 'description': 'Department of the Walgreens chain providing prescription medications & other health-related items.', 
  
    // 'latitude': 41.451859999999996, 
  
    // 'longitude': -85.2666757, 
  
    // 'category': ['Pharmacy'], 
  
    // 'avg_rating': 4.2, 
  
    // 'num_of_reviews': 5, 
  
    // 'price': '$$', 
  
    // 'hours': [['Thursday', '8AM–1:30PM'], ['Friday', '8AM–1:30PM'], ['Saturday', '9AM–1:30PM'], ['Sunday', '10AM–1:30PM'], ['Monday', '8AM–1:30PM'], ['Tuesday', '8AM–1:30PM'], ['Wednesday', '8AM–1:30PM']], 
  
    // 'MISC': {
    'Service options': ['Curbside pickup', 'Drive-through', 'In-store pickup', 'In-store shopping'], 
    'Health & safety': ['Mask required', 'Staff wear masks', 'Staff get temperature checks'], 
    'Accessibility': ['Wheelchair accessible entrance', 'Wheelchair accessible parking lot'], 
    'Planning': ['Quick visit'], 
    'Payments': ['Checks', 'Debit cards']
    }, 
  
    // 'state': 'Closes soon ⋅ 1:30PM ⋅ Reopens 2PM', 
  
    // 'relative_results': ['0x881614cd49e4fa33:0x2d507c24ff4f1c74', '0x8816145bf5141c89:0x535c1d605109f94b', '0x881614cda24cc591:0xca426e3a9b826432',    '0x88162894d98b91ef:0xd139b34de70d3e03', '0x881615400b5e57f9:0xc56d17dbe420a67f'], 
  
    // 'url': 'https://www.google.com/maps/place//data=!4m2!3m1!1s0x881614ce7c13acb
    b:0x5c7b18bbf6ec4f7e?authuser=-1&hl=en&gl=us'
    
Los archivos donde se disponibilizan las reviews de los usuarios (51 archivos, 1 por cada estado de USA) se conforman de la siguiente manera 
     
     // 'user_id': '101463350189962023774', 
     
     // 'name': 'Jordan Adams', 
    
     // 'time': 1627750414677, 
     
     // 'rating': 5, 
     
     // 'text': 'Cool place, great people, awesome dentist!', 
     
     // 'pics': [
     {
       'url': ['https://lh5.googleusercontent.com/p/AF1QipNq2nZC5TH4_M7h5xRAd
       61hoTgvY1o9lozABguI=w150-h150-k-no-p']
     }
     ], 
     
     // 'resp': {
       'time': 1628455067818, 
       'text': 'Thank you for your five-star review! -Dr. Blake'
     }, 
     
     // 'gmap_id': '0x87ec2394c2cd9d2d:0xd1119cfbee0da6f3'

   

Fuente de datos obligatoria: 
+  [Carpeta de Google Drive](https://drive.google.com/drive/folders/1Wf7YkxA0aHI3GpoHc9Nh8_scf5BbD4DA?usp=share_link), con metadata de los lugares y las reseñas de 51 estados de EE.UU.



## Disclaimer  
De parte del equipo de Henry se quiere aclarar y remarcar que los fines de los proyectos propuestos son exclusivamente pedagógicos, con el objetivo de realizar proyectos que simulen un entorno laboral, en el cual se trabajen diversas temáticas ajustadas a la realidad.
 No reflejan necesariamente la filosofía y valores de la organización. Además, Henry no alienta ni tampoco recomienda a los alumnos y/o cualquier persona leyendo los repositorios (y entregas de proyectos) que tomen acciones en base a los datos que pudieran o no haber recabado. Toda la información expuesta y resultados obtenidos en los proyectos, nunca deben ser tomados en cuenta para la toma real de decisiones (especialmente en la temática de finanzas, salud, política, etc.).
