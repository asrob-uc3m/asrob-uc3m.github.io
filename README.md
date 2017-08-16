Asociación de Robótica (ASROB) UC3M
------

Sito web de la Asociación de Robótica (ASROB) UC3M

Web alojada actualmente en http://asrob-uc3m.github.io

# Editar la web
## Configurando la información de la web
### Configuración básica

El archivo `_config.yml` contiene los parámateros básicos de configuración de la
web, así como otros parámetros avanzados.

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
 * `picture`: imagen que acompaña al enlace. Lo idea es que esta imagen sea de
 318x180px para mantener la estética de la web.

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
