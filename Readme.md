# EJERCICIO 2 #

>1.	**¿Qué es un servidor HTTP?**

Un programa servidor HTTP, conocido como servidor web, opera aplicaciones en el lado del servidor, estableciendo conexiones que pueden ser bidireccionales o unidireccionales, así como síncronas o asíncronas, con el cliente. Este servidor genera o proporciona respuestas en diversos lenguajes o aplicaciones del lado del cliente. El navegador web es responsable de renderizar el código recibido por el cliente. Estas comunicaciones suelen realizarse a través del protocolo HTTP, que forma parte de la capa de aplicación del modelo OSI. Además, el término "servidor web" también se refiere al equipo informático donde se llevan a cabo estas funciones.

>2.	**¿Qué son los verbos HTTP? Mencionar los más conocidos**

HTTP establece una serie de métodos de solicitud que especifican la acción que se desea ejecutar en un recurso específico. Aunque estos métodos pueden representarse como sustantivos, a menudo se les denomina "verbos HTTP".

Los verbos más conocidos son:

 GET:
Este método solicita una representación de un recurso específico. Las solicitudes GET solo recuperan datos.

 HEAD:
Pide una respuesta idéntica a la de una solicitud GET, pero sin el cuerpo de la respuesta.

 POST:
Envía datos para ser procesados por el recurso identificado en la URL de la línea de petición. Los datos se incluirán en el cuerpo de la solicitud. Se utiliza principalmente para crear un nuevo recurso, cuya naturaleza está especificada por la cabecera Content-Type.

 PUT:
Envía datos al servidor, pero a diferencia del método POST, la URI de la línea de petición no hace referencia al recurso que los procesará, sino que identifica a los propios datos.

 DELETE:
Borra un recurso específico.

 CONNECT:
Se utiliza para verificar si se tiene acceso a un host. No necesariamente la solicitud llega al servidor. Este método se utiliza principalmente para verificar si un proxy nos da acceso a un host bajo condiciones especiales, como por ejemplo "corrientes" de datos bidireccionales encriptadas.

 OPTIONS:
Devuelve los métodos HTTP que el servidor soporta para una URL específica. Esto puede ser utilizado para verificar la funcionalidad de un servidor web mediante la solicitud en lugar de un recurso específico.

 TRACE:
Realiza una prueba de bucle de retorno de mensaje a lo largo de la ruta al recurso de destino.

 PATCH:
Su función es similar a PUT, el cual sobrescribe completamente un recurso. Se utiliza para actualizar de manera parcial una o varias partes.


>3.	**¿Qué es un request y un response en una comunicación HTTP? ¿Qué son los headers?**

El proceso comienza con la solicitud, donde el cliente envía una petición al servidor web. Esta petición, conocida como **REQUEST**, es recibida y procesada por el servidor. Luego, el servidor genera una respuesta, denominada **RESPONSE**, después de realizar las acciones necesarias para cumplir con la solicitud. Estas acciones pueden incluir la ejecución de programas instalados, consultas a bases de datos u otras operaciones relacionadas con archivos y herramientas disponibles. Una vez que la información solicitada ha sido recopilada, se formatea según las especificaciones y se devuelve como respuesta al cliente.

El **ENCABEZADO** web, por otro lado, constituye la parte superior de un sitio web. Al ser lo primero que los usuarios visualizan al acceder al sitio, es crucial considerar dos aspectos importantes. En primer lugar, debe permitir que los usuarios naveguen fácilmente por el sitio, proporcionando una experiencia intuitiva de usuario. En segundo lugar, el encabezado debe ofrecer información relevante sobre la identidad del sitio, lo que ayuda a establecer una conexión rápida y significativa con los visitantes.

>4.	**¿Qué es un queryString? (En el contexto de una url)**

En el contexto de una URL, un queryString es una cadena de caracteres que sigue a la parte de la dirección web principal y contiene datos adicionales que se envían al servidor web. Estos datos se utilizan para realizar consultas específicas o para proporcionar información adicional sobre la solicitud al servidor. El queryString generalmente comienza con el símbolo "?" y consiste en una serie de pares clave-valor separados por el símbolo "&". 

>5.	**¿Qué es el responseCode? ¿Qué significado tiene los posibles valores devueltos?**

El responseCode, también conocido como código de respuesta HTTP, es un número de tres dígitos que indica el estado de una solicitud HTTP realizada por un cliente a un servidor web. Este código es devuelto por el servidor como parte de la respuesta a la solicitud del cliente y proporciona información sobre el resultado de la operación solicitada. Los códigos de respuesta HTTP se dividen en cinco clases principales, cada una de las cuales tiene un significado específico:

1-Informacionales (1xx): Indica que la solicitud ha sido recibida y el servidor está procesando la solicitud.

2- Éxito (2xx): Indica que la solicitud fue recibida, entendida y aceptada satisfactoriamente.

3- Redirección (3xx): Indica que se requiere que el cliente realice más acciones para completar la solicitud.

4- Error del cliente (4xx): Indica que la solicitud contiene errores por parte del cliente o no se pudo completar debido a circunstancias del cliente.

5- Error del servidor (5xx): Indica que el servidor no pudo completar la solicitud debido a un error interno.

6.	**¿Cómo se envía la data en un Get y cómo en un POST?**

En una solicitud GET, los datos se envían como parte de la URL en la línea de solicitud. Esto se hace agregando los parámetros de la solicitud directamente a la URL, separados por el símbolo de interrogación "?" y utilizando el formato clave=valor. 

En una solicitud POST, los datos se envían en el cuerpo de la solicitud HTTP en lugar de adjuntarse a la URL. Esto permite enviar una cantidad significativamente mayor de datos y también puede proporcionar una capa adicional de seguridad al ocultar los datos de la vista del usuario. Los datos se envían como pares clave=valor, pero no son visibles en la URL. En su lugar, se envían como parte del cuerpo de la solicitud HTTP y pueden ser de cualquier tipo MIME, como JSON o XML. Esta es la forma preferida de enviar datos sensibles o grandes, como formularios en línea.

>7.	**¿Qué verbo http utiliza el navegador cuando accedemos a una página?**

Cuando accedemos a una página web a través del navegador, se utiliza principalmente el verbo HTTP GET. Este verbo es el más comúnmente utilizado para recuperar recursos, como documentos HTML, imágenes, estilos CSS, scripts JavaScript, entre otros, desde un servidor web. El navegador envía una solicitud GET al servidor para recuperar la página web solicitada, y luego el servidor responde proporcionando los recursos solicitados, que luego son renderizados por el navegador para que el usuario los vea.

>8.	**Explicar brevemente qué son las estructuras de datos JSON y XML dando ejemplo de estructuras posibles.**

JSON y XML son dos formatos utilizados para representar y transmitir datos de manera estructurada y legible tanto por humanos como por máquinas. Ambos tienen sus propias características y usos particulares.

JSON
{
  "nombre": "Axel",
  "edad": 21,
  "ciudad": "Buenos Aires",
  "intereses": ["programación", "videojuegos", "Gym"]
}

XML
<persona>
  <nombre>Axel</nombre>
  <edad>21</edad>
  <ciudad>Buenos Aires</ciudad>
  <intereses>
    <interes>programación</interes>
    <interes>videojuegos</interes>
    <interes>gym</interes>
  </intereses>
</persona>

>9.	**Explicar brevemente el estándar SOAP**

SOAP es un estándar de comunicación basado en XML, diseñado para facilitar la interoperabilidad entre sistemas distribuidos en redes web. Permite el intercambio de mensajes estructurados de forma independiente del lenguaje de programación y la plataforma utilizada, promoviendo la integración de sistemas heterogéneos.

>10.	**Explicar brevemente el estándar REST Full**

REST es un estilo de arquitectura para sistemas distribuidos en la web. Los servicios RESTful exponen recursos que pueden ser accedidos y manipulados utilizando operaciones estándar de HTTP, como GET, POST, PUT y DELETE. Se caracteriza por ser sin estado, basado en recursos y utilizar una interfaz uniforme para acceder a dichos recursos.

>11.	**¿Qué son los headers en un request? ¿Para qué se utiliza el key Content-type en un header?**

Los encabezados (headers) en una solicitud HTTP son metadatos adicionales enviados junto con la solicitud que proporcionan información sobre la misma. Estos encabezados contienen detalles como el tipo de navegador del cliente, el tipo de contenido aceptado, la codificación de caracteres, las cookies, entre otros.

El encabezado "Content-Type" se utiliza para indicar el tipo de medio del contenido que se envía en el cuerpo de la solicitud o de la respuesta. Es decir, especifica el formato de los datos que se están enviando o recibiendo. Por ejemplo, si se está enviando un formulario HTML, el tipo de contenido puede ser "application/x-www-form-urlencoded". Si se está enviando un objeto JSON, el tipo de contenido puede ser "application/json". Esto permite al servidor entender cómo interpretar y procesar los datos recibidos de manera adecuada.

# EJERCICIO 3 #

>1.	Realizar un request GET a la URL: https://procontacto-reclutamiento-default-rtdb.firebaseio.com/contacts.json

![image](https://github.com/AxelColamarino/README/assets/153008108/e17a07f3-1924-4a41-bfbe-7dc5249ea23d)

>2.	Realizar un request POST a la URL anterior, y con body:

![image](https://github.com/AxelColamarino/README/assets/153008108/0e99ffff-1559-4ba4-a636-4060a0e48ac0)

>3.	Realizar nuevamente un request GET a la URL: https://procontacto-reclutamiento-default-rtdb.firebaseio.com/contacts.json

![image](https://github.com/AxelColamarino/README/assets/153008108/14d4a431-97ee-47e9-8091-d8b9e6a3de7d)

La diferencia que hay es que despues de hacer el ultimo GET mis datos figuran en el Servidor.

# EJERCICIO 4 #

[MODULOS DE TRAILHEAD](https://www.salesforce.com/trailblazer/v6r6hgwtxgz0siv2ir)

# EJERCICIO 5 #

>Lead (Prospecto):

Aquí se registran los posibles clientes interesados en los productos o servicios de la empresa. Los datos almacenados incluyen: Nombre completo, Nombre de la empresa, Ubicación, Dirección de correo electrónico, Estado del prospecto, Fecha de creación, Propietario asignado.

>Account (Cuenta):

Es el registro de las empresas con las que la empresa tiene una relación comercial. Los datos almacenados incluyen: Nombre de la empresa, Sitio web, Dirección de facturación, Número de teléfono, Tipo de empresa, Propietario asignado.

>Contact (Contacto):

Es el registro de los individuos que trabajan en las empresas con las que la empresa tiene relación. Los datos almacenados incluyen: Nombre completo, Nombre de la empresa, Cargo, Teléfono, Correo electrónico, Propietario asignado.

>Opportunity (Oportunidad):

Aquí se registran las posibles ventas que pueden convertirse en ingresos para la empresa. Los datos almacenados incluyen: Nombre de la oportunidad, Nombre de la empresa, Monto, Fecha estimada de cierre, Etapa del proceso, Propietario asignado de la oportunidad.

>Product (Producto):

Es el registro que contiene detalles específicos sobre los productos ofrecidos por la empresa. Los datos almacenados incluyen: Nombre del producto, Código del producto, Propietario asignado.

>PriceBook (Libro de precios):

Aquí se detallan los precios de los productos ofrecidos por la empresa. Los datos almacenados incluyen: Nombre del catálogo de precios, Descripción, Propietario asignado.

>Asset (Activo):

Es el registro que contiene información sobre un activo propiedad de la empresa. Los datos almacenados incluyen: Contacto asociado, Empresa asociada, Estado, Número de serie, Propietario del activo, Ubicación.

>Case (Caso):

Es donde se gestionan todos los problemas o consultas de los clientes que deben ser resueltos. Los datos almacenados incluyen: Número del caso, Nombre del contacto afectado, Asunto, Estado de prioridad, Fecha y hora de apertura, Propietario asignado del caso.

>Ejemplo de diagrama

![image](https://github.com/AxelColamarino/README/assets/153008108/ce51abf2-d021-4d4a-b3df-e01ddbd2a4b8)
