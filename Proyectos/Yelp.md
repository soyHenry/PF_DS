![HenryLogo](https://d31uz8lwfmyn8g.cloudfront.net/Assets/logo-henry-white-lg.png)

# **PROYECTO GRUPAL Nº1**

- - -

# <h1 align="center">**`YELP REVIEWS AND RECOMMENDATIONS`**</h1>

<p align="center">
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/ad/Yelp_Logo.svg/2560px-Yelp_Logo.svg.png"  height="200">
</p>


## **Contexto**

"Yelp es una plataforma de reseñas de todo tipo de negocios, restaurantes, hoteles, servicios entre otros. Los usuarios utilizan el servicio y luego suben su reseña según la experiencia que han recibido. Esta información es muy valiosa para las empresas, ya que les sirve para enterarse de la imagen que tienen los usuarios de los distintos locales de la empresa, siendo útil para medir el desempeño, utilidad del local, además de saber en qué aspectos hay que mejorar el servicio. "


## **Propuesta de trabajo**

"Como parte de una consultora de data, nos han contratado para poder realizar un análisis del mercado estadounidense. Nuestro cliente es parte de un conglomerado de empresas de restaurantes y afines, y desean tener un análisis detallado de la opinión de los usuarios en Yelp sobre hoteles, restaurantes y otros negocios afines al turismo y ocio, utilizando análisis de sentimientos, predecir cuáles serán los rubros de los negocios que más crecerán (o decaerán). Además, desean saber dónde es conveniente emplazar los nuevos locales de restaurantes y afines, y desean poder tener un sistema de recomendación de restaurantes para los usuarios de Yelp para darle al usuario la posibilidad de poder conocer nuevos sabores basados en sus experiencias previas. Pueden cambiar el tipo de comercio (no es necesario que sean restaurantes).
"


- - -
## **Datasets y fuentes complementarias**

"Los datos son extraídos de la plataforma de reseñas Yelp. Tiene información sobre la ubicación de los comercios, su categoría, puntajes promedios, si están abiertos o no, sobre los usuarios, las reseñas que hicieron, cuántas reseñas hicieron, cuántos votos han recibido esas reseñas entre otros. Se puede complementar el análisis con datasets adicionales que ofrezcan información que consideren pertinente al pedido (valores de acciones de las empresas, información geográfica adicional de los locales, etc). Recomendamos fuertemente el uso de NLP para procesar la información de las reseñas."

### **Diccionario de datos**
business.pkl
Contiene información del comercio, incluyendo localización, atributos y categorías.

    // string, 22 caracteres id del negocio, refiere al negocio en   business.    json
    "business_id": "tnhfDv5Il8EaGSXZGiuQGg",

    // string, nombre del negocio
    "name": "Garaje",

    // string, direccion completa del negocio
    "address": "475 3rd St",

    // string, ciudad
    "city": "San Francisco",

    // string, codigo de 2 letras del Estado donde se ubica el negocio
    "state": "CA",

    // string, el codigo postal
    "postal code": "94107",

    // float, latitud
    "latitude": 37.7817529521,

    // float, longitud
    "longitude": -122.39612197,

    // float, rating en estrellas, redondeado a 0 o 0.5
    "stars": 4.5,

    // entero, numero de reseñas
    "review_count": 1198,

    // entero, 0 si esta cerrado, 1 si está abierto
    "is_open": 1,

    // objeto, atributos del negocio como valores. Algunos valores de atributos también puedne ser objetos. 
    "attributes": {
        "RestaurantsTakeOut": true,
        "BusinessParking": {
            "garage": false,
            "street": true,
            "validated": false,
            "lot": false,
            "valet": false
        },
    },

    // lista de categorias de los negocios
    "categories": [
        "Mexican",
        "Burgers",
        "Gastropubs"
    ],

    // objeto, de dia a hora, las horas son en 24hr
       "hours": {
        "Monday": "10:00-21:00",
        "Tuesday": "10:00-21:00",
        "Friday": "10:00-21:00",
        "Wednesday": "10:00-21:00",
        "Thursday": "10:00-21:00",
        "Sunday": "11:00-18:00",
        "Saturday": "10:00-21:00"
    

review.json
Contiene las reseñas completas, incluyendo el user_id que escribió el review y el business_id por el cual se escribe la reseña


    // string, 22 caracteres id de reseña
    "review_id": "zdSx_SD6obEhz9VrW9uAWA",

    // string, 22 caracteres id único de usuario, refiere al usuario en user.json
    "user_id": "Ha3iJu77CxlrFm-vQRs_8g",

    // string, 22 caracteres id del negocio, refiere al negocio en business.json
    "business_id": "tnhfDv5Il8EaGSXZGiuQGg",

    // entero, puntaje en estrellas de 1 al 5
    "stars": 4,

    // string, fecha formato YYYY-MM-DD
    "date": "2016-03-09",

    // string, la reseña en inglés
    "text": "Great place to hang out after work: the prices are decent, and the ambience is fun. It's a bit loud, but very lively. The staff is friendly, and the food is good. They have a good selection of drinks.",

    // entero, números de votos como reseña útil
    "useful": 0,

    // entero, número de votos como reseña graciosa
    "funny": 0,

    // entero, número de votos como reseña cool.
    "cool": 0

user.parquet
Data del usuario incluyendo referencias a otros usuarios amigos y a toda la metadata asociada al usuario.


    // string, 22 caracteres, id de usuario que refiere al usuario en user.json
    "user_id": "Ha3iJu77CxlrFm-vQRs_8g",

    // string, nombre del usuario
    "name": "Sebastien",

    // entero, numero de reseñas escritas
    "review_count": 56,

    // string, fecha de creacion del usuario en Yelp en formato YYYY-MM-DD
    "yelping_since": "2011-01-01",

    // lista con los id de usuarios que son amigos de ese usuario
    "friends": [
        "wqoXYLWmpkEH0YvTmHBsJQ",
        "KUXLLiJGrjtSsapmxmpvTA",
        "6e9rJKQC3n0RSKyHLViL-Q"
    ],

    // entero, numero de votos marcados como útiles por el usuario
    "useful": 21,

    // entero, numero de votos marcados como graciosospor el usuario
    "funny": 88,

    // entero, numero de votos marcados como cool por el usuario
    "cool": 15,

    // entero, numero de fans que tiene el usuario
    "fans": 1032,

    // lista de enteros, años en los que el usuario fue miembro elite
    "elite": [
        2012,
        2013
    ],

    // float, promedio del valor de las reseñas
    "average_stars": 4.31,

    // entero, total de cumplidos 'hot' recibidos por el usuario
    "compliment_hot": 339,

    // entero, total de cumplidos varios recibidos por el usuario
    "compliment_more": 668,

    // entero, total de cumplidos por el perfil recibidos por el usuario
    "compliment_profile": 42,

    // entero, total de cumplidos 'cute' recibidos por el usuario
    "compliment_cute": 62,

    // entero, total de listas de cumplidos recibidos por el usuario
    "compliment_list": 37,

    // entero, total de cumplidos como notas recibidos por el usuario
    "compliment_note": 356,

    // entero, total de cumplidos planos recibidos por el usuario
    "compliment_plain": 68,

    // entero, total de cumplidos 'cool' recibidos por el usuario
    "compliment_cool": 91,

    // entero, total de cumplidos graciosos recibidos por el usuario
    "compliment_funny": 99,

    // entero, número de complidos escritos recibidos por el usuario
    "compliment_writer": 95,

    // entero, número de cumplidos en foto recibidos por el usuario
    "compliment_photos": 50

checkin.json
Registros en el negocio.


    // string, 22 caracteres id del negocio que se refiere al negocio en business.json
    "business_id": "tnhfDv5Il8EaGSXZGiuQGg"

    // string que es una lista de fechas separados por coma, en formato YYYY-MM-DD HH:MM:SS
    "date": "2016-04-26 19:49:16, 2016-08-30 18:36:57, 2016-10-15 02:45:18, 2016-11-18 01:54:50, 2017-04-20 18:39:06, 2017-05-03 17:58:02"


tip.json
Tips (consejos) escritos por el usuario. Los tips son más cortas que las reseñas y tienden a dar sugerencias rápidas.


    // string, texto del tip
    "text": "Secret menu - fried chicken sando is da bombbbbbb Their zapatos are good too.",

    // string, fecha cuando se escribio el tip YYYY-MM-DD
    "date": "2013-09-20",

    // entero, cuantos cumplidos totales tiene
    "compliment_count": 172,

    // string, 22 caracteres, id del negocio que se refiere al negocio en business.json
    "business_id": "tnhfDv5Il8EaGSXZGiuQGg",

    // string, 22 caracteres de id de usuario, que se refieren al usuario en user.json
    "user_id": "49JhAJh8vSQ-vM4Aourl0g"

Fuentes de datos obligatorias:
+ https://drive.google.com/file/d/1QhtF1UAbVMJyAcqVJDucYwmib0hHCP1A/view?usp=sharing




<img src = "https://media0.giphy.com/media/3o6Mbp8ctWmQkXok5a/giphy.gif?cid=790b761128fb8043c46c89171eb1bd632b9fddae2ed68215&rid=giphy.gif&ct=g" height = 200>
  
  
## Disclaimer  
De parte del equipo de Henry se quiere aclarar y remarcar que los fines de los proyectos propuestos son exclusivamente pedagógicos, con el objetivo de realizar proyectos que simulen un entorno laboral, en el cual se trabajen diversas temáticas ajustadas a la realidad.
 No reflejan necesariamente la filosofía y valores de la organización. Además, Henry no alienta ni tampoco recomienda a los alumnos y/o cualquier persona leyendo los repositorios (y entregas de proyectos) que tomen acciones en base a los datos que pudieran o no haber recabado. Toda la información expuesta y resultados obtenidos en los proyectos, nunca deben ser tomados en cuenta para la toma real de decisiones (especialmente en la temática de finanzas, salud, política, etc.).




