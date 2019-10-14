# Configuración básica

Una vez que tengas CONSUL funcionando en el servidor, hay algunas opciones básicas de configuración que probablemente quieras definir para poder empezar a usarlo.

Para ello deberás acceder a tu instalación de CONSUL a través de cualquier navegador de internet e identificarte con el usuario de administración (inicialmente es el usuario `admin@consul.dev` con la contraseña `12345678`). Una vez identificado verás en la parte superior derecha de la pantalla el enlace "Admin" que te llevará a la interfaz de administración. Desde esta interfaz recomendamos configurar las principales opciones básicas a través del asistente de instalación, y una vez configurado recorrer el resto de posibles funcionalidades que se pueden desear accediendo a la sección Configuración desde el submenú de Administración.

## Asistente de instalación
Para acceder al Asistente de instalación, en el menú lateral encontrarás la opción "Configuración" y posteriormente el submenú "Asistentes", donde podremos acceder al "Asistente de instalación".

#### Paso 1 - Bienvenida al Asistente de Instalación
En este asistente realizaremos paso a paso toda la configuración necesaria para poder personalizar la aplicación a las necesidades de su Institución. Si no dispone de alguna información solicitada en el asistente podrá obviarlos y modificarlo en un futuro en la Sección de Configuración relacionada o desde este mismo Asistente.

#### Paso 2 - Configuración Global
En este paso podrá actualizar algunas de las Configuraciones Globales de la aplicación más importantes. En caso de querer modificar alguna una vez realizado el Asistente podrá acceder a la sección "Configuración > Configuración Global" o volviendo a ejecutar el Asistente de Instalación.

- Nombre del sitio. Este nombre aparecerá en el asunto de emails, páginas de ayuda...
- Edad mínima para participar. Si utilizas un sistema de verificación de usuarios esta será la edad mínima que se exigirá a los usuarios. Sobre el sistema de verificación de usuarios se ha incluido un nuevo asistente para poder configurarlo, que será explicado al final de esta sección.

#### Paso 3 - Procesos de participación
En este paso podrán activar/desactivar los procesos de participación que decida utilizar cada Institución. En caso de querer modificar alguna una vez realizado el Asistente podrá acceder a la sección "Configuración > Procesos de Participación" o volviendo a ejecutar el Asistente de Instalación.
- Debates: El espacio de debates ciudadanos está dirigido a que cualquier persona pueda exponer temas que le preocupan y sobre los que quiera compartir puntos de vista con otras personas.
- Propuestas: Las propuestas ciudadanas son una oportunidad para que los vecinos y colectivos decidan directamente cómo quieren que sea su sociedad, después de conseguir los apoyos suficientes y de someterse a votación ciudadana.
- Número de apoyos necesarios para aprobar una Propuesta: Cuando una propuesta alcance este número de apoyos ya no podrá recibir más y se considera exitosa.
- Votaciones: Las votaciones ciudadanas son un mecanismo de participación por el que la ciudadanía con derecho a voto puede tomar decisiones de forma directa.
- Presupuestos participativos: Con los presupuestos participativos la ciudadanía decide a qué proyectos presentados por los vecinos y vecinas va destinada una parte del presupuesto.

#### Paso 4 - Configuración del Mapa
En este paso podrán activar/desactivar la geolocalización de las propuestas y proyectos de gasto, y personalizar la manera en que se muestra el mapa a los usuarios. En caso de querer modificar alguna una vez realizado el Asistente podrá acceder a la sección "Configuración > Configuración del mapa" o volviendo a ejecutar el Asistente de Instalación.
- Geolocalización de propuestas y proyectos de gasto: Permite activar la geolocalización en la aplicación.
- Latitud: Latitud para mostrar la posición del mapa
- Longitud: Longitud para mostrar la posición del mapa
- Zoom: Zoom para mostrar la posición del mapa. Puedes probar con un valor inicial y luego cambiarlo más adelante.

#### Paso 5 - Conexión SMTP
En este paso podrán configurar la conexión SMTP para poder enviar correos desde la aplicación En caso de querer modificar alguna una vez realizado el Asistente podrá acceder a la sección "Configuración > Conexión SMTP" o volviendo a ejecutar el Asistente de Instalación.
- Configuración SMTP: Activa esta funcionalidad para permitir utilizar la configuración SMTP definida en esta sección y poder enviar emails desde la aplicación.
- Host SMTP: Configura el host del servidor SMTP. Ejemplo: 'smtp.example.com'.
- Puerto SMTP: Configura el puerto del servidor SMTP. Ejemplo: 587.
- Dominio: Configura el dominio del servidor SMTP. Ejemplo: 'example.com'.
- Usuario SMTP: Configura el usuario del servidor SMTP. Ejemplo: 'username'.
- Contraseña SMTP: Configura la contraseña del servidor SMTP. Ejemplo: 'password'.
- Autenticación SMTP: Configura el mecanismo de autenticación del servidor SMTP. Ejemplo: 'plain'.
- Activar TLS para SMTP.

#### Paso 6 - Idiomas y Zona horaria
En este paso podrán configurar el idioma por defecto de la aplicación, los idiomas disponibles y la zona horaria en la que se encuentra. En caso de querer modificar alguna una vez realizado el Asistente podrá acceder a la sección "Configuración > Regional Settings" o volviendo a ejecutar el Asistente de Instalación.

- Idioma por defecto: Definir el idioma por defecto de la aplicación mediante el selector que ofrece todos los idiomas disponibles en la aplicación.
- Idiomas disponibles de la aplicación:  Podrá ver todo el listado de idiomas disponibles en la aplicación y habilitar/deshabilitar los que considere oportunos.
- Zona horaria: Permite seleccionar la zona horaria en la que queremos utilizar la aplicación.

#### Paso 7 - Finalización del Asistente
En caso de querer modificar cualquier dato una vez realizado el Asistente podrá modificarlo en la sección Configuración o volviendo a ejecutar el Asistente de Instalación.

Al finalizar el asistente nos redirigirá a la pantalla de Configuración donde podremos modificar tanto los valores introducidos como configurar nuevas funcionalidades y características de la aplicación no contempladas en este Asistente de instalación explicadas en los siguientes apartados.

## Parámetros de la configuración global
En el menú lateral encontrarás la opción "Configuración" y posteriormente el submenú "Configuración global". Aquí encontrarás muchos parámetros interesantes, pero por el momento te recomendamos definir algunos de los más básicos. Más adelante cuando estés más familiarizado con la herramienta podrás volver a configurar otros parámetros:

- Nombre del sitio. Este nombre aparecerá en el asunto de emails, páginas de ayuda...
- Nombre email remitente. Este nombre aparecerá como nombre del remitente en los emails enviados desde la aplicación. Como por ejemplo el email que los usuarios reciben para confirmar que han creado su cuenta.
- Dirección email remitente. Esta dirección de email aparecerá en los emails enviados desde la aplicación.
- URL general de la web. URL principal de tu web.
- Edad mínima para participar. Si utilizas un sistema de verificación de usuarios esta será la edad mínima que se exigirá a los usuarios. Sobre el sistema de verificación de usuarios hablaremos en más detalle más adelante.
- Número de apoyos necesarios para aprobar una Propuesta. Si utilizas la sección de propuestas ciudadanas, puedes definir un mínimo de apoyos que necesitan las propuestas para ser consideradas. Cualquier usuario podrá crear propuestas pero solo las que lleguen a ese valor serán tenidas en cuenta.
- Cargos públicos de nivel x. CONSUL permite que algunas cuentas de usuario se marquen como "cuentas oficiales" apareciendo más resaltadas sus intervenciones en la plataforma. Esto por ejemplo se usa en una ciudad si se quieren definir cuentas para el Alcalde, los Concejales, etc. Esta opción de cargos públicos te permitirá definir la etiqueta oficial que aparece al lado de los nombres de usuario de estas cuentas de mayor importancia (nivel 1) a menor (nivel 5).

## Categorías de las propuestas
Cuando los usuarios crean propuestas en la plataforma se sugieren unas categorías generales, para ayudar a organizar las propuestas. Para definir estas categorías puedes entrar en el menú "Configuración global" y luego en el submenú "Temas de propuestas". En la parte superior puedes escribir temas y crearlos con el botón que aparece a continuación.

##  Definición de geozonas
Las geozonas son áreas territoriales más pequeñas que la zona en la que usas CONSUL (por ejemplo los distritos en una ciudad en la que se use CONSUL). Si las activas permitirá por ejemplo que las propuestas ciudadanas se asignen a una zona concreta, o que las votaciones estén restringidas a la gente que viva en alguna zona.

En el menú lateral encontrarás la opción "Configuración" y posteriormente el submenú "Gestionar distritos". A la derecha el botón "Crear distrito" te permitirá crear nuevas geozonas. Solo el nombre es necesario para definirlas, pero podrás agregar otros datos que son útiles en ciertas secciones. Inicialmente te recomendamos que empieces definiendo sólo los nombres de las zonas.

Una vez definidas si creas una propuesta ciudadana verás como una de las opciones en el formulario de creación te permite elegir si tu propuesta se refiere a una geozona concreta.

Si activas las geozonas puedes también mostrar una imagen que represente el área con las zonas. Esta imagen puedes cambiarla en el menú "Configuración global" en el submenú "Personalizar imágenes". La imagen por defecto que podrás cambiar es la titulada "map".

##  Mapa para geolocalizar propuestas
Puedes permitir que al crear propuestas los usuarios puedan situarlas en un mapa. Para ello tienes que definir qué mapa quieres mostrar.

Accede en primer lugar al menú  "Configuración" y posteriormente al submenú "Configuración global". Allí encontrarás tres parámetros que tendrás que rellenar:

- Latitud. Latitud para mostrar la posición del mapa
- Longitud. Longitud para mostrar la posición del mapa
- Zoom. Zoom para mostrar la posición del mapa. Puedes probar con un valor inicial y luego cambiarlo más adelante.

En la parte superior de esta página encontrarás tres pestañas: "Configuración Global", "Funcionalidades" y "Configuración del Mapa". Accede ahora a la segunda pestaña "Funcionalidades".

En esta página encontrarás una de las funcionalidades titulada como "Geolocalización de propuestas y proyectos de gasto". Deberá aparecer el mensaje "Funcionalidad activada" a su derecha. Si no es así haz click en el botón "Activar".

A continuación, en la parte superior de esta página accede a la pestaña "Configuración del Mapa". Si todo ha sido configurado correctamente verás aquí el mapa centrado en la latitud y longitud que introdujiste antes. Puedes centrar correctamente el mapa y cambiar el nivel de zoom directamente sobre el mapa, pulsando luego el botón "Actualizar" que hay debajo de él.

##  Emails a usuarios
CONSUL envía por defecto una serie de correos electrónicos a los usuarios. Por ejemplo al crear una cuenta de usuario, al intentar recuperar la contraseña, al recibir un mensaje de otro usuario, etc.

Todos los correos que se envían puedes visualizarlos en el menú "Mensajes a usuarios" en el submenú "Emails del sistema". Ahí podrás previsualizar cada correo electrónico y ver el archivo donde está el contenido del correo por si quieres cambiarlo.

## Páginas básicas de información
CONSUL cuenta con una serie de páginas básicas de información que se mostrarán a los usuarios. Por ejemplo "Política de Privacidad", "Preguntas Frecuentes", "Felicidades acabas de crear tu cuenta de usuario", etc.

Puedes ver las páginas que existen por defecto y modificarlas en el menú "Contenido del sitio" en el submenú "Personalizar Páginas".

## Página principal del sitio
Al acceder a tu instalación de CONSUL los usuarios verán la página principal de la plataforma. Esta página es totalmente configurable, para que muestres el contenido que te parezca más relevante. Puedes modificarla desde el menú "Contenido del sitio" en el submenú "Homepage".

Prueba a crear "Encabezados" y "Tarjetas" y a activar las diferentes funcionalidades que encontrarás debajo para ver el efecto que producen en tu página principal.

## Textos de la plataforma
Si accedes al menú "Contenido del sitio" y al submenú "Personalizar textos" verás diferentes pestañas con una serie de textos. Estos son todos los textos que se muestran en la plataforma. Por defecto puedes utilizar los que existen, pero en cualquier momento puedes acceder a esta sección para modificar cualquiera de los textos.

Para tener más información sobre cómo añadir nuevas traducciones a tu versión de CONSUL accede a la sección "Textos y traducciones" de esta documentación.

## Canales de participación
Por defecto encontrarás en CONSUL diferentes formas de participación para los usuarios. Para empezar y familiarizarte con la plataforma te recomendamos tenerlos todos activados, pero puedes desactivar todos los que no te parezcan necesarios. Para ello accede al menú "Configuración" y posteriormente al submenú "Configuración global". En la parte superior de esta página encontrarás tres pestañas: "Configuración Global", "Funcionalidades" y "Configuración del Mapa". Accede a la segunda pestaña "Funcionalidades".

Encontrarás diversas funcionalidades con los nombres de los diferentes canales de participación "Debates", "Propuestas", "Votaciones", "Legislación Colaborativa" y "Presupuestos Participativos". Puedes desactivar cualquiera de las funcionalidades y dejará de mostrarse en tu instalación de CONSUL.

###  Más información y documentación detallada
Estas opciones anteriores te permitirán tener una versión básica de CONSUL que empezar a usar. Te recomendamos acceder a la sección [Documentación y guías sobre CONSUL](../getting_started/consul_guides.md) donde podrás encontrar más documentación detallada.
