# Odoo-Tests

Crear un repositorio en GitHub.

Generar una carpeta llamada extra-addons.

Dentro de extra-addons, organizar el contenido en dos partes:

Crear una subcarpeta llamada dummy_module:

Dentro de esta carpeta, incluir dos archivos:
__init__.py (vacío).
__manifest__.py (con contenido de configuración del módulo).

Añadir un archivo llamado .gitkeep (vacío), útil para mantener la estructura de carpetas en Git.

Crear el archivo Dockerfile con el código necesario para la configuración del entorno.

Asegurarse de que el nombre del archivo Dockerfile sea exactamente el mismo en todos los lugares donde se utilice.

Crear un nuevo proyecto en la plataforma Render.

Dentro del proyecto, configurar dos servicios:
OdooInstalacion
Progress_db

Una vez que el entorno esté cargado, seleccionar la opción “New PostgreSQL”.

Crear una base de datos y vincularla al proyecto.

En el servicio Progress_db, configurar las siguientes credenciales de conexión:
Hostname
Port
Database
Username
Password

En el servicio OdooInstalacion, acceder a la sección “Environment” y definir las siguientes variables de entorno, utilizando los valores correspondientes de Progress_db:
PGDATABASE
PGHOST
PGPASSWORD
PGUSER
