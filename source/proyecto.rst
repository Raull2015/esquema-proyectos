El Proyecto
===========

Descripcion General
-------------------

La aplicación en general contara con tres tipos de usuarios: usuarios comunes,
usuarios artistas y usuarios administradores

De cara a los usuarios comunes su función es la de ser una agenda de actividades
culturales que ocurran en la ciudad de Quetzaltenango y de los artistas que participen,
mostrando una cronología de fechas, permitiendo filtrarlas por temática, con opción
a dejar reseñas en alguna actividad, puntuarlas, también permite buscar y consultar
perfiles de artistas, además de recibir contenido educativo en forma de capsulas
informativas sobre temas de interés cultural.

Dirigido hacia los Artistas, además de las funciones que tiene el público común,
la aplicación permite que puedan crear un perfil con sus datos, el perfil necesita
ser verificado y aprobado por un administrador del sistema, el Artista tiene permitido
crear eventos que la aplicación calendarizara los cuales también serán verificados y
aprobados por el administrador del sistema.

Tanto artistas como actividades serán clasificados según la temática cultural con la
que trabajen.

Por ultimo existe un tipo de usuario especial, el Administrador, sus funciones
comprenden el aprobar la creación de perfiles de Artista y Actividades, retirar artistas y
actividades según crea necesario, crear actividades organizadas por la propia casa de
cultura, calendarizar las capsulas informativas que recibirán los demás usuarios y
un acceso a los reportes y estadísticas con la información que la aplicación recaudara.

Modulos
-------

  Diagrama de caso de uso: :ref:`ref_vistaGeneral`

Actividades
***********
  Se encarga de mostrar a los usuarios las actividades próximas a realizarse en forma de cartelera,
  visualizando el nombre, descripción, imagen promocional, lugar, fecha, hora, artistas que participen,
  temática, precio de entradas.

  Tiene funciones para filtrar y buscar actividades en especifico, agregar o retirar comentarios, puntuarlas,
  y permitir la creación (o cancelación) de nuevas actividades por parte de un artista o administrador,
  cada actividad nueva creada no se publicara hasta que un administrador lo autorice.

  Diagrama de caso de uso: :ref:`ref_actividades`

Artistas
********
  Accesible para todo los usuarios, permite visualizarlo a los artistas registrados en forma de directorio
  y contara con la capacidad de buscar y filtrarlos por nombre o temática cultural en la que trabajen.

  Si un usuario se registra como artista manejara un perfil donde colocar al publico sus datos de contacto y
  personales si desea, foto de perfil, sexo, edad, teléfono y/o correo electrónico, mas un espacio donde describir
  su trabajo.

  Un artista no será mostrado en el directorio hasta que su registro sea autorizado por un administrador.

  Diagrama de caso de uso: :ref:`ref_artistas`

Capsulas Informativas
*********************
  Su función es la de mostrar información educativa cultural a los usuarios comunes, y permitir
  a los administradores del sistema calendarizar las que se mostraran en las próximas fechas.

  Diagrama de caso de uso: :ref:`ref_capsulas`

Administracion de Artistas y Eventos
************************************
  Se encarga de moderar tanto a artistas como eventos, autorizar o denegar el registro de un artista, autorizar la
  publicación de una actividad o retirarla si fuera necesario.

  Diagrama de caso de uso: :ref:`ref_adminArtEven`

Administracion de Cuentas
*************************
  Se encarga de manejar las distintas cuentas de usuario creadas, tendrá las acciones de eliminar artista,
  crear nuevo usuario administrador, modificar contraseñas y datos de cualquier cuenta.

  Diagrama de caso de uso: :ref:`ref_cuentas`

Estadisticas de Uso
*******************
  Una sección de generación de reportes con toda la información que se recopile con el uso de los
  demás usuarios, es utilizado por el administrador

  Diagrama de caso de uso: :ref:`ref_estadisticas`
