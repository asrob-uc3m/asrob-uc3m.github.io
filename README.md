Asociación de Robótica (ASROB) UC3M
------

Sitio web de la Asociación de Robótica (ASROB) UC3M

Web alojada actualmente en http://asrob-uc3m.github.io

Author: [David Estevez](https://github.com/David-Estevez)

# Cómo editar la web
Esta sección contiene la información necesaria para añadir o modificar contenidos
de la web.


## Configurando la información de la web

El archivo `_config.yml` contiene los parámateros básicos de configuración de la
web, así como otros parámetros avanzados.

### Configuración básica

El apartado `society` contiene la información básica sobre la asociación:

 * `name`: nombre completo de la asociación
 * `short_name`: nombre corto o siglas de la asociación
 * `email`: email de contacto

### Configuración de Redes Sociales
El apartado `society.social` contiene la información sobre las distintas redes
sociales de la asociación. En él se pueden eliminar o añadir nuevas redes sociales.

Una red social tiene los siguientes parámetros:

 * `id`: identificador de la red social (google-plus, flickr, dribbble, pinterest,
    instagram, tumblr, linkedin, etc). Para el correo usaremos `envelope`.
 * `name`: nombre de la red social.
 * `url`: url al perfil de la asociación en dicha red social.


### Configuración de Responsables
El apartado `society.management` contiene la información sobre los distintos
responsables de la asociación. En él se pueden modificar los responsables. Cada
responsable tiene un nombre, un correo de contacto y un link a una web de su
elección asociados.

El apartado `society.management.social` corresponde a los Responsables de Redes
Sociales, y puede contener más de una entrada.

### Configuración de la sección *Enlaces importantes*
El apartado `more_info` contiene la información de la sección *Enlaces importantes*
de la web. En caso de que hubiese que añadir, eliminar o modificar algún enlace,
basta con editar esta sección. Cada enlace tiene los siguientes parámetros:

 * `title`: título del enlace.
 * `description`: texto que acompaña al enlace.
 * `url`: url del enlace.
 * `picture`: imagen que acompaña al enlace. Lo ideal es que esta imagen sea de
 **318x180px** para mantener la estética de la web.

### Configuración de la sección *Más enlaces importantes*
El apartado `other_info` contiene la información de la sección *Más enlaces importantes*
de la web. En caso de que hubiese que añadir, eliminar o modificar algún enlace,
basta con editar esta sección. Cada enlace tiene los siguientes parámetros:

 * `name`: título del enlace.
 * `url`: url del enlace.

### Configuración de colaboradores
El apartado `collaborations` contiene la información de las entidades que colaboran
con la asociación. En caso de que hubiese que añadir, eliminar o modificar algún
colaborador, basta con editar esta sección. Cada colaborador tiene los siguientes parámetros:

 * `name`: nombre del colaborador.
 * `url`: enlace a la web del colaborador.
 * `picture`: logo del colaborador.

## Modificar *About*
La sección *About* muestra información genérica sobre la asociación. Esta información
se encuentra en el archivo `_posts/2017-05-27-about.markdown` en formato markdown.

## Añadir o modificar *grupos de trabajo*
La información sobre los *grupos de trabajo* se almacena en archivos markdown en
 las carpetas `_workgroups` (para *grupos de trabajo activos*) o `_old_workgroups`
  (para *antiguos grupos de trabajo*). A cada *grupo de trabajo* le corresponde un
archivo. Dentro de cada archivo encontramos una serie de parámetros que modificar
para modificar la información del *grupo de trabajo*:

  * `type`: tipo de archivo (**no modificar**, debe ser `workgroup`).
  * `layout`: plantilla que se le aplicará a este archivo (**no modificar**, debe
    ser `workgroup`).
  * `workgroup_id`: nombre corto, en minúsculas y sin espacios que designa a este
    grupo. Si se necesitan varias palabras es recomendable separarlas con `_`
    (por ejemplo: `printer_one`).
  * `name`: nombre del grupo. Si el grupo tiene siglas, este sería un buen sitio
    para ponerlas (por ejemplo: `G.A.M.E`).
  * `subtitle`: pequeña descripción del grupo (una línea máximo). Si el grupo tiene
    siglas, este sería un buen sitio para poner lo que significan (por ejemplo:
    `Group for Arcade Machine Experimentation`) [opcional].
  * `description`: descripción breve (un párrafo) que aparecerá en la portada de
    la web.
  * `url_wiki`: enlace a la página correpondiente al *grupo de trabajo activo*
  en la wiki [opcional].
  * `url_telegram,`: enlace al grupo de telegram del *grupo de trabajo activo*
  [opcional].
  * `picture`: thumbnail que aparecerá en la portada de la web. Lo ideal es que
  esta imagen sea de **700x300px** para mantener la estética de la web.
  * `picture_full`: imagen que aparecerá en la página de dicho grupo. Lo ideal es
  que esta imagen sea de **750x500px** para mantener la estética de la web.
  * `manager`: nombre del responsable del *grupo de trabajo activo*.
  * `manager_email`: email del responsable del *grupo de trabajo activo*.
  * `keys_info`: información acerca de quién tiene qué llaves dentro del *grupo de trabajo activo*.
  * `next_meeting`: información sobre la próxima reunión del *grupo de trabajo
  activo*. Por ejemplo: "Miércoles 4 a las 17h en aula 1.0.B06" o "Todos los
  Martes de 15:00 a 16:00 en 1.0.B06" [opcional].
  * `next_meeting_doodle`: link al doodle para decidir el horario del *grupo de
  trabajo activo* [opcional].
  * `active`: indica si el *grupo de trabajo* está activo o no (true o false).

La descripción completa del grupo, que aparecerá en la página de dicho grupo, se
incluye como texto en formato markdown después de la zona reservada a los parámetros.

## Añadir o modificar *proyectos*
La información sobre los *proyectos* se almacena en la carpeta
`_projects` en archivos markdown. A cada proyecto le corresponde un
archivo. Dentro de cada archivo encontramos una serie de parámetros que modificar
para modificar la información del *proyecto*:

 * `type`: tipo de archivo (**no modificar**, debe ser `project`).
 * `layout`: plantilla que se le aplicará a este archivo (**no modificar**, debe
  ser `project`).
 * `parent`: *grupo de trabajo activo* al que pertenece el proyecto. El valor
  debe coincidir con el valor del `workgroup_id` de algún *grupo de trabajo activo*.
 * `name`: nombre del proyecto.
 * `subtitle`: pequeña descripción del grupo (una línea máximo).
 * `description`: descripción corta (un párrafo) que aparecerá en la página del
  *grupo de trabajo activo*.
 * `url_wiki`: enlace a la página correspondiente al *proyecto* en la wiki. [opcional]
 * `url_github`: enlace al repositorio del *proyecto* en GitHub. [opcional]
 * `picture`: thumbnail que aparecerá en la página del *grupo de trabajo activo*.
  Lo ideal es que esta imagen sea de **318x180px** para mantener la estética de
  la web.
 * `picture_full`: imagen que aparecerá en la página de dicho proyecto. Lo ideal
  es que esta imagen sea de **900x300px** para mantener la estética de la web.
 * `status`: estado del proyecto. Los valores posibles son: "activo", "terminado",
 "abandonado" o "proyecto futuro".

 La descripción completa del proyecto, que aparecerá en la página de dicho
 proyecto, se incluye como texto en formato markdown después de la zona reservada
 a los parámetros.

## Añadir o modificar *noticias*
La información sobre los *noticias* se almacena en la carpeta
`_news` en archivos markdown. A cada noticia le corresponde un
archivo. Aunque por el momento sólo aparece el titular de la noticia en la portada
de la web, en el futuro se podrá redactar una noticia completa y visualizarla en
la web. Dentro de cada archivo encontramos una serie de parámetros que modificar
para modificar la información de la noticia:

 * `type`: tipo de archivo (**no modificar**, debe ser `news`).
 * `title`: título de la noticia.
 * `description`: breve descripción de la noticia (una línea máximo).
 * `picture`: imagen que aparecerá en la portada de la web. Lo ideal es que
 esta imagen sea de **1280x720px** para mantener la estética de la web.

## Añadir o modificar *premios y trofeos*
La información sobre los *premios y trofeos* se almacena en la carpeta
`_awards` en archivos markdown. A cada premio le corresponde un
archivo. Dentro de cada archivo encontramos una serie de parámetros que modificar
para modificar la información del premio:

 * `name`: Nombre del premio o competición.
 * `date`: Fecha en la que fue concedido el premio.
 * `place`: Puesto o posición en la competición.
 * `link`: Enlace a la web del premio o competición.
 * `team`: Incluye los miembros del equipo al que le fue concedido el premio.
 cada miembro tiene los siguiente parámetros:
    * `name`: nombre del miembro.
    * `link`: link  a una web del miembro [opcional].

La descripción el premio o competición, que aparecerá en la página de premios y
trofeos, se incluye como texto en formato markdown después de la zona reservada
a los parámetros.

## Redirecciones a doodle
Es posible generar una página fija que redireccione al Doodle semanal que se ha configurado para cierto *grupo de trabajo activo*. Para ello, hay que añadir un archivo markdown a la carpeta `_redirects`, que contenga los siguientes parámetros:

* `workgroup_id`: *grupo de trabajo activo* al que pertenece el proyecto. El valor
 debe coincidir con el valor del `workgroup_id` de algún *grupo de trabajo activo*.
* `layout`: plantilla que se le aplicará a este archivo (**no modificar**, debe
 ser `redirect_to_doodle`).

# Atribuciones
Esta web se inspiró en las siguientes plantillas:

 * [1 Col Portfolio](https://blackrockdigital.github.io/startbootstrap-1-col-portfolio/)
 * [Portfolio Item](https://blackrockdigital.github.io/startbootstrap-portfolio-item/)
 * [One Page Wonder](https://startbootstrap.com/template-overviews/one-page-wonder/)
