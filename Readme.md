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

![image](https://github.com/AxelColamarino/README/assets/153008108/a076c8b6-0ab4-43f9-8671-e8dec4de9016)

# EJERCICIO 6 #

- Soluciones de Salesforce

>¿Qué es Salesforce?

Salesforce es una **plataforma en la nube para la gestión de relaciones con los clientes** (CRM) que proporciona una vista unificada de los clientes en una plataforma integrada para todos los departamentos de una organización, incluyendo marketing, ventas, servicio al cliente y comercio electrónico.

>¿Qué es Sales Cloud?

Sales Cloud es una **herramienta CRM y de ventas completa** que ofrece las funciones necesarias de automatización de ventas en un solo lugar, simplificando el proceso de ventas y mejorando la eficiencia del equipo.

>¿Qué es Service Cloud?

Service Cloud es una **solución integral de atención al cliente** diseñada para brindar soporte a los clientes en cualquier momento y lugar a través de una variedad de canales, incluyendo teléfono, correo electrónico, redes sociales, chat y comunidades en línea.

>¿Qué es Health Cloud?

Health Cloud es una plataforma especializada en la **gestión clínica de pacientes en la nube**, que facilita una comunicación más personalizada entre pacientes, proveedores y prestadores de servicios de salud, adaptándose a los procesos y datos médicos de cada paciente.

>¿Qué es Marketing Cloud?

Marketing Cloud es un **módulo de Salesforce** que ofrece diversas herramientas para mejorar la **interacción de las marcas con sus clientes** a través de diversos canales, permitiendo una comunicación más efectiva y personalizada.

- Funcionalidades de Salesforce

>¿Qué es un RecordType?

Los **Record Types** en Salesforce nos permiten definir diferentes **Business Process, Pages Layouts y Picklist Values** en un determinado objeto. Así mismo, los **Record Types** nos ayudan a mostrar distintos tipos de información según el perfil del usuario.

>¿Qué es un ReportType?

Un **reporte** es una lista de registros que cumplen los criterios que define. Se muestra en Salesforce en filas y columnas, y se puede filtrar, agrupar o mostrar en un diagrama gráfico. Cada **reporte** se almacena en una carpeta.

>¿Qué es un Page Layout?

Los **diseños de página** controlan el diseño y la organización de botones, campos, s-controls, Visualforce, enlaces personalizados y listas relacionadas en páginas de registros de objetos.

>¿Qué es un Compact Layout?

Un **diseño compacto** muestra los campos clave de un registro de un vistazo en la aplicación móvil Salesforce, Lightning Experience y en las integraciones de Outlook y Gmail.

>¿Qué es un Perfil?

Los **perfiles** definen cómo acceden los usuarios a objetos y datos y qué pueden hacer en la aplicación.

>¿Qué es un Rol?

Los **roles** controlan el nivel de visibilidad que un usuario tiene sobre los datos de su organización. Usuarios en cualquier función dada pueden ver, editar, e informar sobre todos los datos para funciones por debajo de ellos en la jerarquía de roles.

>¿Qué es un Validation Rule?

Las **reglas de validación** verifican que los datos que un usuario introduce en un registro cumplen con las normas que especifica antes de que el usuario guarde el registro. Una **regla de validación** puede contener una fórmula o expresión que evalúa los datos en uno o más campos y ofrece un valor “Verdadero” o “Falso”.

>¿Qué diferencia hay entre una relación Master Detail y Lookup?

En las relaciones de búsqueda se usan cuando los objetos están relacionados solo en ciertos casos. Los objetos de las relaciones de búsqueda suelen funcionar como objetos independientes que tienen sus propias fichas en la interfaz de usuario. En las relaciones del tipo principal-detalle, el objeto de detalle no funciona de manera independiente. En realidad, este objeto depende del objeto principal. Por lo tanto, si se elimina un registro del objeto principal, también se eliminarán todos los registros relacionados del objeto de detalle. A la hora de crear relaciones principal-detalle, siempre se crea el campo de relación en el objeto de detalle.

>¿Qué es un Sandbox?

Un **Sandbox** es una copia de su organización en un entorno aislado que puede usar para distintos fines, como pruebas y capacitación. Los **sandbox** están completamente aislados de su organización de producción de Salesforce.

>¿Qué es un ChangeSet?

Un **conjunto de cambios entrantes** es un conjunto de cambios que se ha enviado desde otra organización de Salesforce a la organización en la que ha iniciado sesión. Un **conjunto de cambios** se debe implementar para que los cambios surtan efecto.

>¿Para qué sirve el import Wizard de Salesforce?

**Data Import Wizard** es una herramienta de carga de datos integrada en Salesforce para todas las ediciones.

>¿Para qué sirve la funcionalidad Web to Lead?

Puede utilizar los **formularios Web-to-Lead** para definir una campaña o fuente de clientes potenciales colocando valores dentro de los campos ocultos. Estos valores jugarán un papel clave en el respaldo de las acciones automatizadas una vez que los clientes potenciales lleguen a Salesforce.

>¿Para qué sirve la funcionalidad Web to Case?

Recopile las solicitudes de servicio de atención al cliente directamente del sitio web de su empresa y genere automáticamente casos nuevos con **Caso Web**.

>¿Para qué sirve la funcionalidad Omnichannel?

**Omni- canal** es una función personalizable y flexible que se puede configurar de forma declarativa en Salesforce, es decir, sin necesidad de escribir código. **OmniCanal** ayuda al enrutamiento automático de diferentes tipos de elementos de trabajo (como casos y clientes potenciales) a los agentes.

>¿Para qué sirve la funcionalidad Chatter?

**Chatter** es una aplicación de colaboración en tiempo real de Salesforce que permite a sus usuarios trabajar juntos, comunicarse y compartir información.

- Conceptos generales

>¿Qué significa SaaS?

El **software como servicio** (SaaS) es un modelo de entrega de software basado en la nube en el que el proveedor de la nube desarrolla y mantiene el software de las aplicaciones en la nube, proporciona actualizaciones automáticas del mismo y lo pone a disposición de sus clientes a través de Internet con un sistema de pago por uso.

>¿Salesforce es Saas?

No, Salesforce es una compañía de PaaS.

>¿Qué significa que una solución sea Cloud?

**Cloud computing** es la disponibilidad bajo demanda de recursos de computación como servicios a través de Internet. Esta tecnología evita que las empresas tengan que encargarse de aprovisionar, configurar o gestionar los recursos y permite que paguen únicamente por los que usen.

>¿Qué significa que una solución sea On-Premise?

El término **on-premises** se refiere al hecho de que los titulares de la licencia instalan el software en su propio entorno informático, sin recurrir a la nube o necesitar acceso a internet.

>¿Qué es un pipeline de ventas?

El **pipeline de ventas** se refiere a cada uno de los pasos de su proceso de ventas que sigue un representante de ventas para llevar una venta desde el principio hasta el final.

>¿Qué es un funnel de ventas?

El **embudo de ventas** es una forma de medir y conocer mucho mejor a tus clientes potenciales o buyer persona. Abarca todas las actividades, desde atraer nuevos visitantes hasta la generación de ventas con una estrategia de Inbound Marketing incrementando así la facturación mensual de tu negocio.

>¿Qué significa Customer Experience?

La **experiencia del cliente** es cómo se relaciona una empresa con sus clientes en todos los aspectos del recorrido de compra, desde el marketing hasta las ventas y el servicio al cliente pasando por cada punto intermedio. En gran parte, es la suma total de todas las interacciones que un cliente tiene con tu marca.

>¿Qué significa omnicanalidad?

La **omnicanalidad** es una estrategia de marketing que crea experiencias valiosas entre una empresa o negocio y sus clientes, a través de todos los medios de contacto que tiene vigentes, ya sean físicos o digitales.

>¿Qué significa que un negocio sea B2B? ¿Qué significa que un negocio sea B2C? ¿Qué es un KPI?

El **B2B (business to business)** es el modelo de negocio en el que se realizan transacciones comerciales entre empresas. En cambio, en el modelo **B2C (business to consumer)** esas transacciones se efectúan entre negocios y los consumidores.
El **KPI (Key Performance Indicator o, en Español, Indicador Clave de Rendimiento)** es un sistema de medición que, expresado normalmente en un porcentaje, nos dice el grado de progreso o cumplimiento de un objetivo de la empresa.

>¿Qué es una API y en qué se diferencia de una Rest API?

Por lo general, la **API** sigue el formato de aplicación a aplicación, mientras que **REST** sigue una estructura diferente: Cliente-Servidor. El cliente y el servidor están evolucionando de forma independiente, proporcionando más flexibilidad en el trabajo.

>¿Qué es un Proceso Batch?

El **modo de lotes** ejecuta una serie de procesos de Cargador de datos en un orden concreto utilizando un archivo por lotes. Puede volver a ejecutar la misma secuencia de procesos utilizando un archivo

>¿Qué es Kanban?

La metodología **Kanban** se implementa por medio de tableros Kanban. Se trata de un método visual de gestión de proyectos que permite a los equipos visualizar sus flujos de trabajo y la carga de trabajo. En un tablero **Kanban**, el trabajo se muestra en un proyecto en forma de tablero organizado por columnas.

>¿Qué es un ERP?

La **planificación de recursos empresariales**, también conocida como ERP, es un sistema que ayuda a automatizar y administrar los procesos empresariales de distintas áreas: finanzas, fabricación, venta al por menor, cadena de suministro, recursos humanos y operaciones.

>¿Salesforce es un ERP?

Salesforce es un CRM ya que se involucra en la gestión de las relaciones con los clientes, mientras que el **ERP** se ocupa de la planificación de los recursos empresariales.
