<!-- 
.. title: documentación
.. slug: documentation
.. date: 2016-10-03 04:59:39 UTC-05:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. type: text
-->

¡Peligro!
---------

Estás leyendo un documento generado para una aplicación en estado de
desarrollo. La intención de este manual es clarificar algunos detalles
sobre el funcionamiento del programa. Ten en cuenta que al ser
activamente desarrollado, el software puede cambiar parte de esta
documentación en un futuro relativamente cercano, así que es
recomendable dar un vistazo de vez en cuando para no perderte demasiado.

Si quieres ver lo que ha cambiado con respecto a la versión anterior,
[lee la lista de novedades aquí.](changes.html)

Introducción {#introduccion}
------------

TWBlue es una aplicación para utilizar twitter de manera sencilla,
rápida, y evitando en la medida de las posibilidades, consumir
demasiados recursos del equipo donde se ejecute. Con la aplicación
podrás hacer acciones en twitter tales como:

-   Crear, responder, reenviar y eliminar Tuits,
-   Marcar como favorito, eliminar de tus favoritos un tuit,
-   Enviar y eliminar mensajes directos,
-   Ver tus amigos y seguidores,
-   Seguir, dejar de seguir, reportar como spam y bloquear a un usuario,
-   Abrir una línea temporal para un usuario, lo que permite obtener
    todos los Tuits de ese usuario únicamente,
-   Abrir direcciones URL cuando vayan en un tuit o mensaje directo,
-   Reproducir varios tipos de archivos o direcciones que contengan
    audio,
-   Y más.

Uso
---

Twitter es una red social que te permite crear actualizaciones de estado
sobre tus actividades en un máximo de 140 caracteres. Twitter es una
manera para mantenerte conectado con tus amigos, familiares y compañeros
de trabajo a través del intercambio de mensajes breves. Puedes
restringir tus actualizaciones para que solo las vean tus amigos, o
permitir que cualquiera pueda verlas. Esta segunda opción es el
comportamiento por defecto de Twitter.

Puedes ver las actualizaciones de estado de tus amigos, familia y
compañeros de trabajo (lo que se conoce como seguir a alguien), y ellos
a su vez pueden ver las actualizaciones que tú publicas (lo que se
conoce como seguidores). Las actualizaciones se denominan Tuits. Los
tuits se publican en tu perfil en Twitter y pueden verse en blogs u
otras páginas web.

Para utilizar TWBlue, primero debes haber creado una cuenta en el sitio
web de Twitter. El proceso de registro en Twitter es muy accesible. Al
registrarte, tendrás que elegir un nombre de usuario. Esto sirve para
dos propósitos. A través de tu nombre de usuario la gente se comunicará
contigo, pero lo más importante, es que se necesitará de tu nombre de
usuario y una contraseña para dar permiso a TWBlue de usar tu cuenta. Te
sugerimos que escojas un nombre de usuario que resulte fácil de recordar
para ti y para tus futuros seguidores.

Para esta guía se asumirá que tienes una cuenta de Twitter y su
contraseña correspondiente.

### Autorizando la aplicación {#autorizando-la-aplicacion}

Antes de nada, lo primero que se necesita es autorizar al programa para
que este pueda acceder a tu cuenta de Twitter, y desde ella realizar lo
que le pidas. El proceso de autorización es bastante sencillo, y en
ningún momento el programa podrá tener acceso a tus datos como usuario y
contraseña. Para autorizar la aplicación, solo tienes que abrir el
archivo principal del programa, llamado TWBlue.exe (en algunos PC, solo
se muestra como TWBlue si el explorador de Windows no está configurado
para mostrar las extensiones de archivos). Si usas una versión portable,
te sugerimos crear un acceso directo en el escritorio para acceder al
programa más rápida y cómodamente.

Puedes iniciar sesión con varias cuentas de Twitter de forma simultánea.
El programa se refiere a cada cuenta que tienes configurada como
"sesión". Si es la primera vez que abres TWBlue, o si no has configurado
antes una sesión, verás el gestor de sesiones. Este diálogo te permite
autorizar todas las cuentas que desees. Si presionas sobre el botón
"Nueva cuenta", un mensaje te informará que tu navegador será abierto
para autorizar la aplicación. Presiona "sí" para iniciar el proceso.

A continuación, tu navegador predeterminado se abrirá con la página de
Twitter solicitándote autorizar la aplicación. Escribe, si no estás
autenticado ya, tu nombre de usuario y contraseña, luego busca el botón
autorizar, y presiónalo.

Una vez que hayas autorizado tu cuenta de Twitter, Twitter te redirigirá
a una página que te notificará que TWBlue ha sido correctamente
autorizado. Ahora puedes cerrar el navegador y regresar al gestor de
sesiones. En la lista de sesiones, podrás ver un nuevo elemento llamado
temporalmente "Cuenta autorizada x", donde x es un número. El nombre
cambiará una vez que inicies esa sesión.

Para iniciar TWBlue, presiona el botón aceptar en el gestor de sesiones.
De forma predeterminada, TWBlue inicia todas las sesiones configuradas
automáticamente, sin embargo, puedes modificar este comportamiento más
adelante.

Si todo ha salido bien, la aplicación empezará a reproducir un grupo de
sonidos en señal que se están actualizando tus datos.

Cuando termine, el programa reproducirá otro sonido, y el lector de
pantalla dirá "listo" (esto puede ser configurado desde las opciones
globales).

conceptos generales
-------------------

Antes de profundizar en el uso de TWBlue, es necesario explicar algunos
conceptos que serán usados extensivamente a lo largo de esta guía.

### Buffer

Un Buffer es una lista de elementos para manejar la información que
proviene de Twitter, después de ser procesada por la aplicación. Cuando
configuras e inicias una sesión en TWBlue, este crea algunos buffers.
Cada uno de ellos puede contener elementos con los que trabaja el
programa: Tuits, mensajes directos, usuarios, tendencias o eventos.
Dependiendo del buffer en el que te encuentres, serás capaz de realizar
distintas acciones con sus elementos.

A continuación está una descripción para cada buffer y los diferentes
tipos de elementos que pueden contener.

-   Principal: Aquí van todos los Tuits que se muestran en la
    línea principal. Estos son los Tuits de los usuarios a los
    que sigues.
-   Menciones: Si un usuario (lo sigas o no) te menciona en Twitter, lo
    verás en esta lista.
-   Mensajes directos: Aquí están los mensajes directos (privados) que
    intercambias con los usuarios que sigues y te siguen, o con
    cualquier usuario, si tienes configurada la opción para recibir
    mensajes directos de cualquier persona (esto es configurable desde
    las opciones de seguridad y privacidad en la web de Twitter). Esta
    lista solo muestra los mensajes recividos.
-   Mensajes directos enviados: En esta lista se muestran los mensajes
    directos que han sido enviados desde tu cuenta.
-   Tuits enviados: En esta lista se muestran los Tuits que se han
    enviado desde tu cuenta.
-   Favoritos: Aquí verás los Tuits que has marcado como favoritos.
-   Seguidores: Cuando los usuarios sigan tu cuenta, podrás verlos en
    esta lista, junto con unos cuantos detalles de su cuenta.
-   Amigos: Igual que la lista anterior, pero estos usuarios son a los
    que tú sigues.
-   Línea temporal de un usuario: Estas son listas que tú deberás crear.
    Es una lista que contiene únicamente los Tuits de un usuario. Se
    usan si algún día necesitas o quieres ver los Tuits que ha realizado
    solo una persona y no deseas buscar por todo tu timeline. Puedes
    crear tantas como usuarios necesites.
-   Eventos: Un evento en TW Blue es "algo" que pase en Twitter. En la
    línea de eventos, podrás ver registrados los eventos más comunes (p.
    Ej. Te han comenzado a seguir, han marcado o removido un tweet tuyo
    de los favoritos, te has suscrito a una lista). Son notificaciones
    que envía Twitter y el programa organiza para que no te pierdas lo
    que ha pasado con tu cuenta.
-   Lista: Una lista es parecida a una línea temporal, pero compuesta
    por los tweets de cada usuario que forme parte de ella.
-   Búsqueda: Un buffer de búsqueda contiene los resultados de una
    búsqueda hecha en TW Blue. Las búsquedas pueden ser por tuits, en
    cuyo caso buscas un término en los tuits relevantes de Twitter, o
    por usuarios, donde los resultados son nombres de usuario
    de Twitter.
-   Favoritos de un usuario: el programa puede crear buffers que te
    muestren los tuits que un usuario ha marcado como favoritos.
-   Tendencias: Un buffer de tendencias muestra los 10 términos más
    utilizados en una región geográfica. Esta región puede ser una
    ciudad o un país. Las tendencias son actualizadas cada
    cinco minutos.

If a tweet contains a URL, you can press enter in the GUI or Control +
Windows + Enter in the invisible interface to open it. If it contains
audio, you can press Control + Enter or Control + Windows + Alt + Enter
to play it, respectively. TWBlue will play a sound if the tweet contains
the \#audio hashtag, but there may be tweets which contain audio without
this. Finally, if a tweet contains geographical information, you can
press Control + Windows + G in the invisible interface to retrieve it.

### Campos para nombre de usuario

Estos campos de texto esperan un nombre de usuario de Twitter (sin el
signo de arroba). Están presentes en los diálogos para enviar mensajes
directos así como en el diálogo de acciones de usuario. Estos diálogos
serán abordados más tarde. El valor inicial de estos campos depende del
lugar desde donde fueron abiertos. Estos campos se rellenan
automáticamente con el nombre de usuario del tuit actual (si ha sido
abierto desde el buffer principal o de enviados, desde una línea
temporal de un usuario o una lista), el usuario que envió el mensaje
directo actual (si se abre desde el buffer de mensajes directos o
mensajes directos enviados) o del usuario actual (desde el buffer de
amigos o seguidores). Si uno de estos diálogos es abierto desde un tuit,
y si hay más de un usuario mencionado, puedes usar las flechas de
arriba/abajo para conmutar entre ellos. Alternativamente, puedes
escribir manualmente el usuario de Twitter en el campo de texto.

Las interfaces del programa
---------------------------

### Interfaz gráfica (GUI) {#interfaz-grafica-gui}

La interfaz gráfica de TWBlue está formada por una ventana que contiene
los siguientes elementos:

-   Una barra de menú que tiene cinco menús (aplicación, tuit, usuario,
    buffer y ayuda),
-   Una presentación en árbol,
-   Una lista de elementos
-   Cuatro botones, la mayoría de las veces: tuit, retuit, responder y
    mensaje directo.

Las acciones disponibles para cada uno de estos elementos serán
retomadas más adelante.

La interfaz gráfica contiene dos componentes importantes. Estos son el
grupo de controles que encontrarás si presionas tab en la ventana
gráfica, y los diferentes elementos que están en la barra de menú.

#### Botones de la aplicación {#botones-de-la-aplicacion}

-   Twit: Este botón abre el diálogo para escribir un tuit. El mensaje
    solo debe tener 140 caracteres. Al escribir el caracter número 141,
    un sonido será reproducido para indicarte que te has pasado del
    límite permitido por Twitter. Ten en cuenta que el número de
    caracteres escritos se muestra en la barra de título. Puedes querer
    acortar o desacortar una URL si la incluye tu tuit a fin de ganar
    más espacio donde escribir, para eso están los botones con
    esos nombres. Puedes también subir una foto, un archivo de audio,
    revisar la ortografía de tu mensaje o traducirlo seleccionando uno
    de los diferentes botones del diálogo. Además, puedes autocompletar
    los nombres de usuarios si pulsas Alt + A o el botón "autocompletar
    usuarios" del diálogo si has configurado la base de datos de
    autocompletado de usuarios. Pulsa Intro para enviar el tuit. Si todo
    sale bien, el mensaje se enviará y tú escucharás un sonido que te lo
    confirme, si no, el lector de pantalla te responderá con un error en
    inglés, que indica por qué no se ha podido enviar el mensaje.
-   Retuit: Este botón retuitea el mensaje que estás leyendo. Luego de
    presionarlo, si no has configurado la aplicación para no hacerlo, se
    te preguntará si deseas añadir un comentario al retuit o compartirlo
    tal y como fue escrito. Si decides añadir un comentario, y si el
    tuit original sumado a tu comentario sobrepasa los 140 caracteres,
    se te preguntará si quieres publicar tu comentario con una mención
    al usuario, y un enlace al tuit original.
-   Responder: Cuando estés visualizando un Tuit, puedes responderle al
    usuario que lo escribió pulsando sobre este botón. Se abrirá el
    mismo diálogo de Tuit, pero con el nombre del usuario (por
    ejemplo @usuario) en el, para que solo escribas el mensaje que
    quieres responderle. Si en el tuit hay más de un usuario mencionado,
    pulsa Shift+Tab y pulsa el botón "Mencionar a todos". Cuando estés
    en la lista de amigos o seguidores, este botón se llamará mencionar.
-   mensaje directo: Exactamente igual que enviar un Tuit, pero es un
    mensaje privado que solo podrá ver el usuario al que se lo envías.
    Pulsa Shift+Tab para ver el destinatario de tu mensaje. Si en el
    Tuit donde estabas para enviar el mensaje había más de un usuario
    mencionado, puedes navegar con las flechas de arriba y abajo para
    seleccionar otro, o escribir tú mismo el usuario (sin el signo
    de arroba).

Ten en cuenta que los botones aparecerán según las acciones que se
puedan hacer en la lista donde estés. Por ejemplo, en la línea
principal, menciones, enviados, favoritos y las líneas temporales de los
usuarios podrás ver los cuatro botones; mientras que en la lista de
mensajes directos solo estará disponible el botón de "Mensaje Directo" y
"tuit", y en las listas de amigos y seguidores, se verá el botón para
"Twit" y el de "Mensaje directo" junto a "mencionar".

#### Menús {#menus}

Visualmente, en la parte superior de la ventana del programa podrás
encontrar una barra de menú que hace las mismas cosas, y algunas cuantas
más. A la barra de menú se accede presionando la tecla Alt, encontrarás
cinco menús: Aplicación, Tuit, Usuario, Buffer y Ayuda. En esta sección
se describen las acciones para cada uno de ellos.

##### Menú aplicación {#menu-aplicacion}

-   Gestionar cuentas: Abre una ventana donde puedes ver todas las
    sesiones que has configurado con TWBlue, lo que te permite añadir
    más cuentas o eliminar las que ya hay configuradas.
-   Actualizar Perfil: Abre un diálogo desde donde se podrá actualizar
    parte de tu información en Twitter. Nombre, ubicación, dirección URL
    y descripción. Si ya tienes alguno de estos campos actualmente en el
    perfil se llenarán automáticamente con lo que tiene tu configuración
    de Twitter. También podrás subir una foto a tu perfil.
-   Esconder Ventana: Desactiva la interfaz gráfica. Lee el apartado
    sobre la interfaz no visible para más detalles sobre
    este comportamiento.
-   Búsqueda: Muestra un cuadro de diálogo desde donde puedes buscar por
    tuits o por usuarios en twitter.
-   Gestor de listas: Para poder utilizar las listas de Twitter, primero
    necesitarás crearlas. Este diálogo permite ver tus listas,
    editarlas, crearlas, borrarlas y, opcionalmente, verlas en buffers
    tal como lo harías con las líneas temporales.
-   Editar combinaciones de teclas: Abre un diálogo donde puedes
    configurar las combinaciones de teclado para la interfaz invisible
    de TWBlue.
-   Opciones de cuenta: Abre un diálogo que te permite configurar las
    opciones para la cuenta actual.
-   Opciones globales: Abre un diálogo para configurar las opciones que
    afectan a toda la aplicación.
-   Salir: pregunta si quieres salir o no del programa. Si la respuesta
    es sí, cierra la aplicación. Si no deseas que TWBlue te pregunte
    siempre antes de salir, puedes configurar esta opción desmarcando la
    casilla correspondiente desde el diálogo de opciones globales.

##### Menú Tuit {#menu-tuit}

-   Las primeras opciones del menú son Twit, responder y retuit, que
    corresponden a los botones del mismo nombre.
-   Marcar como favorito: Marca el tuit que estés viendo como favorito.
-   Quitar tuit de favoritos: Elimina el tuit de tus favoritos. Esto no
    significa que se borra de Twitter, solo deja de estar en tu lista
    de favoritos.
-   Ver tuit: Abre un diálogo donde puedes leer el tuit, mensaje
    directo, amigo o seguidor sobre el que te encuentras actualmente.
    Puedes leer el texto con las flechas de cursor. Es un diálogo muy
    parecido al que se utiliza para escribir un nuevo tuit, excepto que
    para este diálogo no se muestran las opciones de autocompletado,
    carga de archivos de audio e imágenes. Sin embargo, incluye un par
    de contadores que te permitirán saber el número de veces que el tuit
    ha sido retuiteado y marcado como favorito. Si estás en la lista de
    seguidores y amigos, el diálogo solo mostrará información del
    usuario y un botón para cerrarse.
-   Ver dirección: Si el tuit seleccionado contiene información
    geográfica, TWBlue puede mostrar un diálogo donde podrás leer la
    dirección desde donde se escribió el tuit. La dirección se obtiene
    enviando las coordenadas desde donde se hizo el Tuit a los servicios
    de mapas de Google.
-   Ver conversación: Si estás sobre un tuit donde se menciona a otro
    usuario, esta opción te permite abrir un nuevo buffer para seguir
    toda la conversación.
-   Eliminar: Elimina el Tuit o mensaje directo sobre el que estés,
    borrándolo definitivamente de Twitter y qitándolo de tus listas. Ten
    en cuenta que en el caso de los Tuits, Twitter solo permite borrar
    los que tú mismo has escrito.

##### Menú usuario {#menu-usuario}

-   Acciones: Abre un diálogo donde puedes interactuar con un usuario.
    Este diálogo colocará por defecto el nombre de usuario del tuit o
    mensaje directo sobre el que estabas al abrirlo, o en el caso de los
    amigos y seguidores, el usuario actualmente seleccionado. Si lo
    deseas, puedes editar el usuario manualmente. El diálogo presenta
    las siguientes opciones:
-   Follow: Follows a user. This means you'll see his/her tweets on your
    home timeline, and if he/she also follows you, you'll be able to
    exchange direct messages. You may also send / receive direct
    messages from each other if you have configured the option to allow
    direct messages from anyone.
-   Unfollow: Stops following a user, which causes you not being able to
    see his/her tweets on your main timeline neither exchanging direct
    messages, unless they have enabled receiving direct messages
    from anyone.
-   Mute: While muting someone, TWBlue won't show you nor his/her tweets
    on your main timeline; neither will you see that person's mentions.
    But you both will be able to exchange direct messages. The muted
    user is not informed of this action.
-   Unmute: this option allows TWBlue to display the user's tweets and
    mentions again.
-   Block: Blocks a user. This forces the user to unfollow you .
-   Unblock: Stops blocking a user.
-   Report as spam: this option sends a message to Twitter suggesting
    the user is performing prohibited practices on the social network.
-   Ignore tweets from this client: Adds the client from which the
    focused tweet was sent to the ignored clients list.
-   Línea temporal: Abre un diálogo desde donde puedes seleccionar el
    usuario para el que se creará la línea temporal. Al presionar intro,
    se creará. Si se hace una línea temporal de un usuario que no tenga
    Tuits, el programa fallará. Si se crea una línea que ya existe el
    programa te avisará y no permitirá crearla de nuevo.
-   Mensaje Directo: La misma acción que el botón.
-   Añadir a lista: Para que puedas ver los tweets de un usuario en tus
    listas, primero hay que añadirlo. Esta opción abrirá un diálogo
    desde donde puedes seleccionar al usuario que deseas añadir, para
    después abrir otra ventana donde puedes seleccionar la lista a la
    cual añadir a ese usuario. Una vez hecho esto, la lista contendrá un
    nuevo usuario y podrás ver sus tweets.
-   Remover de la lista: Te permite eliminar a un usuario de una de
    tus listas.
-   Ver listas: Muestra las listas en las que participa un
    usuario específico.
-   Ver Perfil del usuario: Abre un diálogo desde donde te permite
    seleccionar el usuario al que quieres ver el perfil.
-   Ver favoritos: Abre un buffer para seguir los favoritos que marca el
    usuario seleccionado.

##### Menú Buffer {#menu-buffer}

-   Nuevo buffer de tendencias: Abre un buffer desde el cual puedes
    realizar un seguimiento de las 10 tendencias de una ciudad o país
    del mundo. Se mostrará un diálogo desde el que puedes seleccionar si
    quieres ver las tendencias para un país, una ciudad o las tendencias
    mundiales (esta opción se encuentra dentro de la lista de ciudades,
    como Worldwhide). El buffer será creado una vez selecciones tu país
    o ciudad, y presiones sobre el botón "aceptar". Recuerda que este
    tipo de buffer se actualiza cada cinco minutos.
-   Cargar elementos anteriores: Permite recuperar más tuits, mensajes
    directos, amigos o seguidores, desde el buffer actual.
-   Silenciar: Silencia completamente el buffer, no escucharás sonido
    alguno cuando nuevos elementos aparezcan.
-   Leer automáticamente tuits para este buffer: Esta opción activa o
    desactiva la lectura automática de tuits. Si está activada, el
    lector de pantalla o la voz Sapi5 (si está activada una) leerá
    automáticamente los nuevos tuits conforme estos vayan llegando
    al buffer.
-   Limpiar Buffer: Vacía los elementos de este buffer.
-   Eliminar buffer: Borra la lista sobre la que te
    encuentras actualmente.

##### Menú Ayuda {#menu-ayuda}

-   Documentación: Abre este archivo, donde puedes leer algunos
    conceptos interesantes del programa.
-   Tutorial de sonidos: Abre un diálogo donde verás una lista de los
    sonidos de TWBlue, para que puedas aprenderlos y no te cueste
    trabajo familiarizarte con el cliente.
-   ¿Qué hay de nuevo en esta versión?: Abre un documento con la lista
    de cambios desde la versión actual, hasta la primera en existencia.
-   Comprobar actualizaciones: Cada que se abre el programa él mismo
    busca automáticamente si hay una nueva versión. Si lo hay, te
    preguntará si quieres descargarla; si aceptas, TWBlue descargará la
    actualización, la instalará y te pedirá reiniciarla (algo que
    hace automáticamente). Esta opción comprueba si hay actualizaciones
    sin tener que reiniciar la aplicación.
-   Reportar un error: Abre un diálogo que te permite reportar un error
    llenando unos cuantos campos. Presiona enter para enviar el reporte.
    si el proceso falla, el programa te notificará de ello.
-   Sitio web de TWBlue. Ve a nuestra [página
    principal](http://twblue.es) donde podrás encontrar toda la
    información y descargas relativas a TW Blue, así como participar de
    la comunidad.
-   Sobre TW Blue: Muestra información de créditos del programa.

### La interfaz invisible

La interfaz invisible, tal como su nombre lo indica, no tiene ventana
gráfica y funciona directamente con los lectores de pantalla como JAWS
for Windows, NVDA y System Access. Esta interfaz se encuentra
desactivada por defecto, pero puedes activarla presionando Control + M.
Funciona de forma parecida a The Qube y Chicken Nugget. Sus
combinaciones de teclado son similares a las que existen en ambos
clientes. Además, el programa incluye soporte para mapas de teclado para
estos clientes, mismos que puedes configurar desde el diálogo de
opciones globales. De forma predeterminada, no puedes usar los atajos de
teclado de esta interfaz desde la ventana gráfica, pero esto es
configurable también desde el diálogo de opciones globales.

La siguiente sección muestra la lista de atajos de teclado para ambas
interfaces. Ten en cuenta que aquí solo se describirán las combinaciones
de teclas para el mapa de teclado por defecto.

Atajos de teclado
-----------------

### Atajos de teclado para la interfaz gráfica (GUI) {#atajos-de-teclado-para-la-interfaz-grafica-gui}

-   Enter: Abre la dirección URL
-   Control + enter: Intentar reproducir un audio.
-   Control + M: Esconde la interfaz gráfica.
-   Control + N: Hacer un nuevo Tuit.
-   Control + R: Responder o mencionar.
-   Control+Shift+R: Hacer un Retuit.
-   Control+D: Enviar mensaje directo.
-   Control + F: marcar tuit como favorito.
-   Control+Shift+F: Quitar tuit de favoritos.
-   Control + S: Abre el diálogo de acciones de usuario.
-   Control + Shift + V: Ver tuit.
-   Control + Q: Salir del programa.
-   Control + I: Abrir línea temporal.
-   Control + Shift + I: Eliminar buffer.
-   F5: Subir volumen un 5%.
-   F6: Bajar volumen un 5%.
-   Control + P: Editar tu perfil.
-   Control + Suprimir: Eliminar un tuit o mensaje directo.
-   Control + Shift + Suprimir: Vaciar el contenido del buffer actual.

### Atajos de teclado para la Interfaz invisible (mapa de teclado por defecto)

-   Control + Windows + Flecha arriba: Se mueve al elemento de arriba en
    el buffer.
-   Control + Windows + Flecha Abajo: Va al elemento de abajo en
    el buffer.
-   Control + Windows + Flecha Izquierda: Se desplaza hacia el
    buffer anterior.
-   Control + Windows + Flecha Derecha: Se desplaza hacia el
    siguiente buffer.
-   Control + Windows + Shift + Flecha izquierda: Va a la
    sesión anterior.
-   Control + Windows + Shift + flecha derecha: Va a la
    siguiente sesión.
-   Control + Windows + C: Ver conversación.
-   Control + Windows + Enter: Open URL.
-   Control + Windows + ALT + Enter: Play audio.
-   Control + Windows + M: Mostrar o esconder la interfaz gráfica.
-   Control+Windows+N: Hacer un nuevo Tuit.
-   Control+Windows+R: Responder a un tuit / mencionar a un usuario.
-   Control+Windows+Shift+R: Hacer un retuit.
-   Control+Windows+D: Enviar un mensaje directo.
-   Windows+ Alt + F: Like a tweet.
-   Alt + Windows + Shift + F: Remove from likes.
-   Control+Windows+S: Abrir el diálogo de acciones de usuario.
-   Control+Windows+Alt+N: Ver detalles de un usuario.
-   Control+Windows+V: Ver tuit.
-   Control + Windows + F4: Salir de TWBlue.
-   Control+Windows+I: Abrir línea temporal.
-   Control+Windows+Shift+I: Eliminar buffer.
-   Control+Windows+Alt+Flecha Arriba: Subir volumen un 5%.
-   Control+Windows+Alt+Flecha Arriba: Subir volumen un 5%.
-   Control+Windows+Inicio: Ir al primer elemento de la lista.
-   Control+Windows+Fin: Ir al final de la lista.
-   Control+Windows+Retroceso de página: ir 20 elementos hacia arriba en
    la lista actual.
-   Control+Windows+Avance de página: Ir 20 elementos hacia abajo en la
    lista actual.
-   Windows + Alt + P: Editar tu perfil.
-   Control+Windows+Suprimir: Eliminar un tuit o mensaje directo.
-   Control + Windows + Shift + Suprimir: Vaciar el contenido del buffer
    actual
-   Control + Windows + Barra espaciadora: Repetir el último elemento
    leído por el lector de pantalla.
-   Control +Windows + Shift + C: Copiar tweet al portapapeles.
-   Control + Windows+ A: Añadir al usuario a una lista.
-   Control + Windows + Shift + A: qitar al usuario de una lista.
-   Control + Windows + Shift + M: Mute / unmute the current buffer.
-   Windows + Alt + M: Silencia/desactiva el silencio en la
    sesión actual.
-   Control+Windows+E: Activar o desactivar la lectura automática de
    nuevos tuits en el buffer actual.
-   Control+windows+- (guión): buscar en Twitter.
-   Control+Windows+K: Mostrar el editor de atajos de teclado.
-   Control + Windows + L: Muestra las listas en las que participa un
    usuario específico.
-   Windows + Alt+ Retroceso de página: Carga más elementos en el
    buffer actual.
-   control + Windows + G: Obtener la ubicación del tuit.
-   Control + Windows + Shift + G: Mostrar la ubicación del tuit en un
    mensaje de diálogo. ¨Control + Windows + T: Crear un buffer
    de tendencias.
-   Control + Windows + { (abrir llave): Buscar una cadena en el
    buffer actual.

Configuración {#configuracion}
-------------

Como se ha descrito anteriormente, la aplicación tiene dos diálogos de
configuración. El diálogo de opciones globales y el diálogo de opciones
de cuenta.

### El diálogo de opciones de cuenta {#el-dialogo-de-opciones-de-cuenta}

#### Pestaña general {#pestana-general}

-   Opciones de autocompletado: Te permite configurar el comportamiento
    de la base de datos de autocompletado de usuarios. Puedes añadir
    usuarios manualmente o permitir que TWBlue añada a todos los
    usuarios que se encuentren en tu buffer de amigos, seguidores
    o ambos.
-   Tiempos relativos: Te permite configurar si quieres que el programa
    calcule el tiempo relativo con el que se enviaron los tuits o
    mensajes directos (hace 2 días, una semana, dos meses, etc.) o si
    solamente quieres que te informe de la fecha y hora a la que fue
    publicado el tuit.
-   Llamadas a la API: Puedes configurar el número de llamadas a la API
    de Twitter que hará el programa.
-   Elementos por cada llamada a la API: Te permite especificar cuántos
    elementos se obtendrán por cada llamada a la API. De manera
    predeterminada, se obtienen 200 elementos por cada llamada. Este es
    el número máximo de elementos que se pueden obtener.
-   Buffers invertidos: Puedes activar esta opción para que los nuevos
    tuits aparezcan al principio de los buffers, y los antiguos se
    ubiquen al final.
-   Modo de retuit: Puedes escoger el comportamiento de TWBlue cuando
    haces un retuit. Las opciones son preguntar, retuitear añadiendo un
    comentario o hacer el retuit sin comentario.
-   Número de elementos de cada buffer a conservar en la base de datos:
    Puedes especificar cuántos elementos de cada buffer serán guardados
    en la base de datos de TWBlue. Cuando se alcance este límite, los
    elementos más viejos del buffer se eliminarán. Puedes escribir
    cualquier número, 0 para guardar todos los elementos sin borrar
    nada, y dejar en blanco el campo de texto para desactivar la base de
    datos completamente.

#### Pestaña buffers {#pestana-buffers}

Esta pestaña muestra la lista de los buffers disponibles en TWBlue, con
excepción de las búsquedas, líneas temporales, líneas temporales de
favoritos y listas. Desde aquí puedes mostrarlos, ocultarlos y moverlos.

#### La pestaña de clientes ignorados {#la-pestana-de-clientes-ignorados}

En esta pestaña, puedes añadir y eliminar clientes que serán ignorados
por el programa.

#### pestaña sonido {#pestana-sonido}

En esta pestaña puedes ajustar el volumen del sonido, seleccionar el
dispositivo de entrada y salida y establecer el paquete de sonidos que
el programa usará para la sesión actual.

#### pestaña Servicios de audio {#pestana-servicios-de-audio}

En esta pestaña puedes introducir tu API Key de SndUp (en caso que
tengas una) para subir audios a este servicio. Ten en cuenta que si no
se escribe ninguna API Key válida, los audios se subirán de forma
anónima a SndUp.

### Opciones globales

Este diálogo te permite configurar algunas opciones que afectan al
funcionamiento de toda la aplicación.

#### General tab {\#general-tab\_1}

-   Idioma: Permite cambiar el idioma con el que se muestra la interfaz
    y documentación del cliente. Los idiomas disponibles hasta el
    momento son inglés, Árabe, Catalán, Alemán, Español, Vasco,
    Finlandés, Francés, Gallego, Croata, Húngaro, Italiano, Polaco,
    Portugués, Ruso y turco.
-   Preguntar al salir de TWBlue: Esta casilla permite controlar si
    TWBlue pedirá confirmación al ser cerrado.
-   Reproducir un sonido cuando inicia TWBlue: Esta casilla permite
    controlar si TWBlue reproducirá un sonido cuando todos los buffers y
    sesiones hayan terminado de cargar.
-   Hablar un mensaje cuando TWBlue inicie: Esta casilla controla si
    TWBlue dirá "listo" al finalizar la carga de las sesiones y buffers.
-   Usar los atajos de teclado de la interfaz invisible en la ventana
    gráfica: Como la interfaz invisible y la ventana gráfica tienen
    atajos de teclado diferentes, podrías querer usar los atajos de la
    interfaz invisible siempre. Si esta opción está marcada, los atajos
    de teclado de la interfaz invisible funcionarán, incluso si tienes
    la ventana gráfica activa.
-   Activar SAPI 5 cuando no hay ningún lector de pantalla ejecutándose:
    Esta casilla controla si se debería proporcionar salida de voz via
    Microsoft SAPI 5 al no encontrarse ningún lector de pantalla
    en ejecución.
-   Esconder interfaz gráfica al iniciar: Esta casilla controla si
    TWBlue iniciará con la interfaz gráfica o la invisible.
-   Keymap: This option allows you to change the keymap used by the
    program in the invisible interface. The shipped keymaps are Default,
    Qwitter, Windows 10 and Chicken Nugget. The keymaps are in the
    "keymaps" folder, and you can create new ones. Just create a new
    ".keymap" file and change the keystrokes associated with the
    actions, as it is done in the shipped keymaps.

#### Pestaña Proxy {#pestana-proxy}

En esta pestaña puedes configurar TWBlue para usar un servidor proxy
completando los campos mostrados (servidor, puerto, usuario y
contraseña).

Licencia, código fuente y donaciones {#licencia-codigo-fuente-y-donaciones}
------------------------------------

TWBlue es software libre, cubierto por la licencia pública general de
GNU (GPL), versión 2. Puedes ver una copia completa de la licencia en el
archivo license.txt, o en internet en
<http://www.gnu.org/licenses/old-licenses/gpl-2.0.html>.

El código fuente de TWBlue está disponible en github en
<https://github.com/manuelcortez/twblue>.

Si te gustaría realizar un donativo para este proyecto, puedes hacerlo
en [la página de donaciones de TWBlue.](http://twblue.es/es/donate)

Contacto
--------

If you still have questions after reading this document, if you wish to
collaborate to the project in some other way, or if you simply want to
get in touch with the application developer, follow the Twitter account
[@tw\_blue2](https://twitter.com/tw_blue2) or
[@manuelcortez00.](https://twitter.com/manuelcortez00) You can also
visit [our website](http://twblue.es)

Créditos {#creditos}
--------

TWBlue is developed and mantained by [Manuel
Cortéz](https://twitter.com/manuelcortez00) and [José Manuel
Delicado](https://twitter.com/jmdaweb). It's supported and sponsored by
[Technow S. L.](https://twitter.com/technow)

También nos gustaría agradecer a los traductores de TWBlue, que han
permitido la difusión de la aplicación.

-   English: [Manuel Cortéz](https://twitter.com/manuelcortez00).
-   Árabe: [Mohammed Al Shara](https://twitter.com/mohammed0204).
-   Catalan: [Francisco Torres](https://twitter.com/ftgalleg)
-   Español: [Manuel Cortéz](https://twitter.com/manuelcortez00).
-   Vasco: [Sukil Etxenike](https://twitter.com/sukil2011).
-   Finés: [Jani Kinnunen](https://twitter.com/jani_kinnunen).
-   Francés: [Rémi Ruiz](https://twitter.com/blindhelp38).
-   Gallego: [Juan Buño](https://twitter.com/Quetzatl_).
-   Alemán: [Steffen Schultz](https://twitter.com/schulle4u).
-   Croata: [Zvonimir Stanečić](https://twitter.com/zvonimirek222).
-   Húngaro: Robert Osztolykan.
-   Italiano: [Christian Leo Mameli](https://twitter.com/llajta2012).
-   Japonés: [Riku](https://twitter.com/riku_sub001).
-   Polaco: [Pawel Masarczyk.](https://twitter.com/Piciok)
-   Portugués: Odenilton Júnior Santos.
-   Rumano: [Florian Ionașcu](https://twitter.com/7ro) y [Răzvan
    Ciule](https://twitter.com/pilgrim89)
-   Russian: [Наталья Хедлунд](https://twitter.com/Lifestar_n).
-   Serbio: [Aleksandar Đurić](https://twitter.com/sokodtreshnje)
-   Turco: [Burak Yüksek](https://twitter.com/burakyuksek).

Muchas gracias también a las personas que trabajaron en la
documentación. Inicialmente, [Manuel
Cortez](https://twitter.com/manuelcortez00) hizo la documentación en
Español, y traducido al inglés por [Bryner
Villalobos](https://twitter.com/Bry_StarkCR), [Robert
Spangler](https://twitter.com/glasscity1837), [Sussan
Rey](https://twitter.com/sussanrey17), [Anibal
Hernandez](https://twitter.com/anibalmetal), y [Holly
Scott-Gardner](https://twitter.com/holly1994). Fue actualizado por
[Sukil Etxenike](https://twitter.com/sukil2011), con algunas valiosas
correcciones por [Brian Hartgen](https://twitter.com/brianhartgen).

------------------------------------------------------------------------

Copyright © 2013-2016. Manuel Cortéz
