## Yin y Yang de una aplicación: frontend y backend

![](https://edteam-media.s3.amazonaws.com/community/original/5c805a11-0c05-471a-b838-aadd16764c94.jpg)

![](https://static.platzi.com/media/user_upload/Backend%20y%20Fronend-d4fbe7b7-403c-4acb-ba58-70164f684e3c.jpg)

## Cómo se conecta el frontend con el backend: API y JSON

La unión entre el Frontend y el Backend se hace a través de una API: Application Programming Interface.

Una API es una sección del backend que permite que el frontend pueda comunicarse con él a través de mensajes bidireccionales (de ida y vuelta).

Tenemos dos grandes estándares para crear las APIs:

SOAP (Simple Objetct Access Protocol): Mueve la información a través de un lenguaje XML (Extensible Markup Language). Es similar al HTML, es un lenguaje demarcado. SOAP es un protocolo que ha quedado en el olvido.

![](https://static.platzi.com/media/user_upload/xml-9789f17e-f0df-4689-a076-b072130d3904.jpg)

Rest (Representational State Transfer): Utiliza otro lenguaje JSON (Javascript Objet Notation). Un JSON no es más que un diccionario de Python. Los diccionarios de Python son lo mismo que los objetos de JS.

![](https://static.platzi.com/media/user_upload/JSON-438f581a-f61e-4d76-a1ab-f3c7a9c44575.jpg)

## El lenguaje que habla Internet: HTTP

* https://developer.mozilla.org/es/docs/Web/HTTP/Status

![](https://plataforma.josedomingo.org/pledin/cursos/flask/curso/u01/img/dia2.png)
![](https://static.platzi.com/media/user_upload/Captura%20de%20pantalla%202021-10-15%20173709-c9329110-e601-4ec1-af80-1fed45b2cbbf.jpg)

![](https://i.imgur.com/8Ql7ST7.jpg)
![](https://static.platzi.com/media/user_upload/Screenshot%20from%202021-10-19%2022-23-06-7f84d301-f46c-4989-b7f4-827da71b349e.jpg)

## IaaS
Infraestructura como servicio. Es el tipo de servicio que nos permite indicarle al provdedor del servidor las especificaciones que requerimos en nuestro proyecto (RAM, SSD, CPU). Las más populares de este tipo son: AWS, Azure y Digital Ocean

## PaaS
Plataforma como servicio. Es el tipo de servicio que nos permite indicarle al provdedor del servidor que se encargue de realizar todas las actualizaciones que requerimos en nuestra app. Solo nos permite elegir que cosas particulares requere nuestro proyecto a nivel general a través de una interfaz. Las más populares de este tipo son: Firebase, Heroku y Google App Engine

## SaaS
Software como servicio. Esta opción nos permite utilizar una aplicación de un proveedor para hacer funcionar nuestro proyecto. Las más populares de este tipo son: Slack, Wordpress y Google Docs

## IaaS: Infrastructure as a service

AWS
Microsoft Azure
Digital Ocean

## PaaS

Firebase
Heroku
Google App Engine

## SaaS:
Software as a service

Slack
Workdpress
Google Docs

El servidor: Hogar de tu código
Es una computadora que contiene una aplicación y la distribuye mediante el protocolo HTTP.

La nube
Son servidores juntos que se encuentan en algún lugar del mundo funcionando y distribuyendo aplicaciones.

Estos se encuentran en un sitio llamado Data Centers

Data Centers
Son los lugares donde se encuentran los servidores, los cuales almacenan datos (como tu página web, o una aplicación como Facebook)

Hosting
Es el acto de guardar tu aplicación en un server.

Un espacio en un servidor, donde tu aplicación será guardada.

Existen diferentes tipos de hosting (formas de guardar aplicaciones):

IaaS: Infrastructure as a Service
PaaS: Platform as a Service
SaaS: Software as a Service
IaaS
Este servicio te da el control de las cosas importantes como

La cantidad de CPU
RAM
SSD
Para esto existen diferentes opciones:

AWS, Microsoft Azure, Digital Ocean.

Existen dos tipos de IaaS:

VPS (Virtual Private Server)

Servidor privado, recursos solo para tí.

Shared Hosting

Compartes los recursos con otras personas.

Investigar AWS, Azure.

PaaS
El servidor se asegura de actualizar las aplicaciones que hacen que viva tu aplicación:

Base de datos
Seguridad
Firewall ???
Qué es un Firewall?

Los firewall o cortafuegos en su traducción, son son programas de software o dispositivos de hardware que filtran y examinan la información que viaja a través de tu conexión a Internet. Representan la primera defensa porque pueden evitar que un programa malicioso o un atacante obtengan acceso a tu red y a tu información antes de que se produzca cualquier posible daño.

Las PaaS tienen una interfaz gráfica que te permite elegir lo que tu app necesita (como una DB o que tipo de Firewall). Creando así un nivel de abstracción donde no tienes que preocuparte de las especificaciones de los servers.

Los PaaS son Just Deploy

Existen diferentes:

Google APP Engine
Firebase
Heroku
SaaS
Es cuando necesitas un software ya hecho.

Es una aplicación que un provedor te presta para que hagas funcionar tu negocio.

No Code

Existen varias opciones:

Google Docs
Slack
WordPress

![](https://static.platzi.com/media/user_upload/server-1-6cb8513b-f495-44a1-84c5-004b1339a95f.jpg)

## Proyecto: diseño y bosquejo de una API

![](https://static.platzi.com/media/user_upload/api-03f678d4-9a58-4876-9436-220f9dcf519a.jpg)
* https://elbauldelprogramador.com/buenas-practicas-para-el-diseno-de-una-api-restful-pragmatica/
* https://www.freecodecamp.org/news/rest-api-best-practices-rest-endpoint-design-examples/

![](https://static.platzi.com/media/user_upload/api-a71b0e3c-d476-444d-986a-06aa8ecc1810.jpg)

## Endpoints para Tweets

(GET) /api/tweets => shows all tweets
(POST) /api/post => publish a tweet
(GET) /api/tweets/:id => shows a single tweet
(UPDATE) /api/tweets/:id => updates a tweet
(DELETE) /api/tweets/:id => deletes a tweet

## Endpoints para Usuarios

(GET) /api/users => shows all users
(POST) /api/signup => registers an user
(GET) /api/users/:userID => shows an user
(UPDATE) /api/users/:userID => updates an user
(DELETE) /api/users/:userID => deletes an user

![](https://static.platzi.com/media/user_upload/ejercicio_LI-24f0310b-f6f1-4fe9-9390-cdedea5fc9dd.jpg)
