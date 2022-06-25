<!-- 
.. title: Preguntas frecuentes
.. slug: faq
.. date: 2016-10-03 05:16:01 UTC-05:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. type: text
-->

-   [¿Dónde puedo encontrar la última versión de TW Blue?](#download)
-   [¿Cada cuanto tiempo habrá una nueva versión?](#new_versions)
-   [Luego de la actualización TW Blue no abre. ¿Qué puedo
    hacer?](#update_issues)
-   [Tengo otro cliente de Twitter que ya utiliza una ventana invisible.
    ¿Puedo usar la interfaz no visible de TW Blue al mismo
    tiempo?](#multiple_hidden_windows)
-   [¿Cómo puedo forzar la actualización de un Buffer en TW
    Blue?](#updating_buffers)
-   [¿Puedo usar la función de traducción de TW Blue para comunicar con
    personas de otros países?](#translating)
-   [¿Puedo usar más de una cuenta con TW Blue?](#more_than_one_account)
-   [Tengo un API Key para Sndup, pero no sube el audio a pesar que lo
    he puesto en el diálogo de configuración. ¿Por qué?](#api_key)
-   [Quiero colaborar con el proyecto. ¿Cómo puedo hacerlo?](#help)

¿Dónde puedo encontrar la última versión de TW Blue? {#download}
----------------------------------------------------

La última versión de Tw blue siempre podrás descargarla desde [nuestra
página de descargas.](download.es.html) Puedes bajar la versión para tu
arquitectura (32 o 64 bits). Ten en cuenta que si ya tienes una versión
en uso, cuando haya una nueva disponible el programa automáticamente te
lo notificará y te preguntará si quieres descargar la actualización. Es
más recomendable, si ya tienes una versión de TW blue, seguir el proceso
de actualización, porque no tienes nada más que hacer que presionar
sobre “sí” al diálogo de descarga y el programa automáticamente
descargará y colocará los archivos necesarios para que la nueva
actualización arranque.

¿Cada cuanto tiempo habrá una nueva versión? {#new_versions}
--------------------------------------------

En un principio, cuando el proyecto recién se empezaba a formar, se
actualizaba todos los sábados. Afortunadamente la aplicación ha ido
haciéndose grande en código, lo que ha hecho que tarde más la
implementación de mejoras, que se traduce en una imposibilidad por
actualizar los sábados de cada semana. En este momento no existe día o
fecha prevista para cada actualización, porque tratamos de trabajar para
que las funciones agregadas sean estables y no generen errores, más que
para cubrir un límite de tiempo. Es preferible que el software se
entregue lo más estable que se permita, antes que entregar una nueva
versión cada sábado repleta de errores inesperados. Aunque si deseas
saber, por nuestra cuenta oficial,
[@tw\_blue2](https://twitter.com/tw_blue2) te haremos saber cuando esté
a punto de salir una nueva versión. También tu copia de TW Blue te lo
notificará.

Luego de la actualización TW Blue no abre. ¿Qué puedo hacer? {#update_issues}
------------------------------------------------------------

Si TW Blue te ha dejado de funcionar luego de haber sido actualizado,
prueba lo siguiente:

-   Descarga nuevamente la versión desde la página web en lugar de
    las actualizaciones.
-   Descomprime la versión descargada en un directorio que no lleve ni
    acentos ni ñ en la ruta. De preferencia tiene que ser en un
    directorio distinto que la versión que no funciona.
-   Copia el directorio config de tu versión que no funciona, y pégalo
    en el directorio donde está la versión que acabas de descargar.
-   Intenta abrir TW Blue.
-   Si no ejecuta, intenta eliminar la carpeta config que habías
    copiado, y repite el proceso. Tw Blue debería pedirte autorización
    de Twitter.
-   Si aún así sigue sin funcionar, abre un reporte de error y coloca el
    contenido de los archivos logs/tracebacks.log, logs/debug.log
    y logs/error.log.

Tengo otro cliente de Twitter que ya utiliza una ventana invisible. ¿Puedo usar la interfaz no visible de TW Blue al mismo tiempo? {#multiple_hidden_windows}
----------------------------------------------------------------------------------------------------------------------------------

No. Lo que esta acción causará, es que una de las aplicaciones que usen
la ventana no visible no funcione luego de activar la otra. La primer
aplicación que usa la ventana oculta quedará anulada por la segunda al
usar la misma característica y no se podrá volver a ella. Cuando se
activan dos ventanas no visibles, la que se usó más recientemente
reemplaza los atajos de teclado de la anterior, causando que la primera
sea inaccesible. No podrás recuperarla y tendrás que matar el proceso
para volver a poder acceder a la aplicación.

¿Cómo puedo forzar la actualización de un Buffer en TW Blue? {#updating_buffers}
------------------------------------------------------------

La respuesta corta es que no lo puedes hacer. La respuesta un poco más
detallada es que TW blue no funciona como otros clientes, que actualizan
de modo periódico.

Cuando abres TW Blue, y se han terminado de cargar todos los tweets en
los búferes (escucharás la palabra listo con un sonido), el método de
actualización será en tiempo real. Esto quiere decir que al momento que
un tweet, mención, directo o seguidor llegue a tu cuenta, el programa
debería reflejar los cambios automáticamente. No se puede forzar a que
intente actualizar, porque lo hace a todo momento. Si el programa sufre
una desconexión, por causa de la conexión a internet o del sistema
operativo, tratará de recuperar todos los tweets que se han perdido, así
como reconectar el servicio en cuanto tenga acceso a internet
nuevamente.

¿Puedo usar la función de traducción de TW Blue para comunicar con personas de otros países? {#translating}
--------------------------------------------------------------------------------------------

No. La función de traducción usa los servicios de [Google
Traductor](http://translate.google.com) y en el mismo se indica que si
bien la traducción en algunos casos puede llegar a alcanzar un buen
grado de presición, no es recomendable utilizarlo como reemplazo a un
traductor humano. Aunque siempre la elección final la tiene el usuario.
Si consideras que google traductor es suficiente para tus propósitos,
entonces la función de traducción de Tuits de TW Blue también lo será.

¿Puedo usar más de una cuenta con TW Blue? {#more_than_one_account}
------------------------------------------

De momento no está soportado. Si quieres utilizar la aplicación con más
de una cuenta puedes intentar copiar dos veces TW Blue en distintos
directorios del sistema, y ejecutar ambas instancias de la aplicación.
Esto te generará una ventana por cada cuenta a utilizar. Ten en cuenta
que solo podrás ocultar una ventana, y si no quieres perder ningún
proceso, asegúrate que no existe ningúna otra aplicación que haga uso de
las teclas de atajo en ese momento.

Tengo un API Key para Sndup, pero no sube el audio a pesar que lo he puesto en el diálogo de configuración. ¿Por qué? {#api_key}
---------------------------------------------------------------------------------------------------------------------

Asegúrate de dos cosas:

1.  TW Blue puede adjuntar archivos de audio de forma anónima.
2.  El API Key está en el diálogo de configuración tal y como se puede
    ver en tu perfil de [SndUp.](http://sndup.net) Presta especial
    atención a que no se copien retornos de línea ni carácteres de
    espacios de ningún tipo.

Si asegurándote de esto y realizando nuevamente el proceso no funciona,
reporta el error a través de la aplicación, en el menú ayuda.

Quiero colaborar con el proyecto. ¿Cómo puedo hacerlo? {#help}
------------------------------------------------------

Si te ha gustado este proyecto y quisieras colaborar para hacer que sea
más grande, que llegue a más personas y que sea una mejor aplicación,
puedes hacer muchas cosas. Toda colaboración es siempre bien recivida.
Estas son las cosas que puedes hacer para ayudar al desarrollo de TW
Blue:

-   Prueba las versiones de la aplicación para tu plataforma, y en caso
    de encontrar errores repórtalos al sistema de seguimiento de
    incidencias mediante la aplicación. Trata de ser específico en tu
    informe, y si puedes y quieres, proporciona una dirección para que
    podamos contactarte y dar un seguimiento más exacto al error.
-   Si te parece justo y te gusta el trabajo que hasta ahora hemos
    estado realizando, puedes colaborar [Realizando una pequeña
    donación](donate.es.html) para ayudar a que pasemos más tiempo
    desarrollando nuevas funcionalidades y corrigiendo errores para TW
    Blue que haciendo otras cosas.
-   Si te gusta la aplicación, puedes recomendarla a tus amigos y
    conocidos mediante tu cuenta de Twitter o cualquier otra red social.
-   Si tienes un blog o sitio web, sería fantástico si pudieras
    difundirnos escribiendo tus impresiones sobre TW Blue. Ideas y
    críticas constructivas son recividas con los brazos abiertos.
-   Si manejas otros idiomas, y deseas colaborar a que la aplicación
    esté disponible para más personas en países donde no hablan español,
    contacta con nosotros a <info@twblue.com.mx>, para incluir una nueva
    traducción y hacer llegar más lejos al proyecto.
-   Si controlas [Python](http://python.org) y [WX
    Python](http://wxpython.org) o algún otro lenguaje de programación,
    y quieres colaborar en el desarrollo de la aplicación o de varios
    otros proyectos para ampliar las posibilidades de TW Blue,
    contáctanos para ver como podemos trabajar.