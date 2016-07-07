El Proyecto
===========

Descripción General
-------------------

La aplicacion en general contara con tres tipos de usuarios: usuarios comunes,
usuarios artistas y usuarios administradores

De cara a los usuarios comunes su funcion es la de ser una agenda de actividades
culturales que ocurran en la ciudad de Quetzaltenango y de los artitas que participen,
mostrando una cronologia de fechas, permitiendo filtrarlas por tematica, con opcion
a dejar reseñas en alguna actividad, puntuarlas, siendo notificados de alguna que le
interese, tambien permite buscar y consultar perfiles de artistas, ademas de recibir
contenido educativo en forma de capsulas informativas sobre temas de interes cultural

Dirigido hacia los Artistas, ademas de las funciones que tiene el publico comun,
la aplicacion permite que puedan crear un perfil con sus datos, el perfil necesita
ser verificado y aprobado por un administrador del sistema, el Artista tiene permitido
crear eventos que la aplicacion calendarizara los cuales tambien seran verificados y
aprobados por el administrador del sistema.

Tanto artistas como actividades seran clasificados segun la tematica cultural con la
que trabajen.

Por ultimo existe un tipo de usuario especial, el Administrador, sus funciones
comprenden el aprobar la creacion de perfiles de Artista y Actividades, retirar artistas y
actividades segun crea necesario, crear actividades organizadas por la propia casa de
cultura, calendarizar las capsulas informativas que recibiran los demas usuarios y
un acceso a los reportes y estadisticas con la informacion que la aplicacion recaudara.


Modulos
^^^^^^^

  diagrama de caso de uso: :ref:`ref_vistaGeneral`.

Actividades:
************
  Se encarga de mostrar a los usuarios las actividades proximas a realizarse en forma de cartelera,
  visualizando el nombre, descripcion, imagen promocional, lugar, fecha, hora, artistas que participen,
  tematica, precio de entradas.

  Tiene funciones para filtrar y buscar actividades en especifico, agregar o retirar comentarios, puntuarlas,
  y permitir la creacion (o cancelacion) de nuevas actividades por parte de un artista o administrador,
  cada actividad nueva creada no se publicara hasta que un administrador lo autorize.

  diagrama de caso de uso: :ref:`ref_actividades`.

Artistas:
*********
  Accesible para todo los usuarios, permite visualizarlo a los artistas registrados en forma de directorio
  y contara con la capacidad de buscar y filtrarlos por nombre o tematica cultural en la que trabajen.

  Si un usuario se registra como artista manejara un perfil donde colocar al publico sus datos de contacto y
  personales si desea, foto de perfil, sexo, edad, telefono y/o correo electronico, mas un espacio donde describir
  su trabajo.

  Un artista no sera mostrado en el directorio hasta que su registro sea autorizado por un administrador.

  diagrama de caso de uso: :ref:`ref_artistas`.

Capsulas Informativas:
**********************
  Su funcion es la de mostrar informacion educativa cultural a los usuarios comunes, y permitir
  a los administradores del sistema calendarizar las que se mostraran en las proximas fechas.

  diagrama de caso de uso: :ref:`ref_capsulas`.

Administracion de Artistas y Eventos:
*************************************
  Se encarga de moderar tanto a artistas como eventos, autorizar o denegar el registro de un artista, autorizar la
  publicacion de una actividad o retirarla si fuera necesario.

  diagrama de caso de uso: :ref:`ref_adminArtEven`.

Administracion de Cuentas:
**************************
  Se encarga de manejar las distintas cuentas de usuario creadas, tendra las acciones de eliminar artista,
  crear nuevo usuario administrador, modificar contraseñas y datos de cualquier cuenta.

  diagrama de caso de uso: :ref:`ref_cuentas`.

Estadisticas de Uso:
********************
  Una seccion de generacion de reportes con toda la informacion que se recopile con el uso de los
  demas usuarios, es utilizado por el administrador

  diagrama de caso de uso: :ref:`ref_estadisticas`.
