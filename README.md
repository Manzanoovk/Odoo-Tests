# Odoo-Tests
PARTE GITHUB
Creamos un repositorio llamado "Odoo-tests", y luego creamos el archivo "Dockerfile" con su respectivo código, después creamos, todo en la rama Main, la carpeta "extra-addons" y dentro de esa carpeta creamos el archivo "Gitkeep" y otra carpeta llamada "dummy_module" donde crearemos los archivos "__init__.py" y "__manifest__.py" que este último ya tendrá el código metido. Y commiteamos todos los cambios.

PARTE RENDER
Primero nos creamos una cuenta en Render, y luego la vinculamos a Github.
Después de haber vinculado Github con Render, iniciamos un nuevo servicio web en base a Github, detectará el lenguaje como Docker automáticamente por el archivo "Dockerfile" de Github.
Seleccionamos la región en Frankfurt, y el plan gratuito.
Esperamos a que el servicio web se inicie y se acabe de configurar.

Ya dentro de Render con el servicio web iniciado creamos un nuevo postgres, lo nombraremos y ahi es donde tendremos la base de datos, vinculada al anterior proyecto con el servicio web.
Esperamos a que el postgres acabe de iniciarse y ya con todo iniciado, volveremos a la configuración "Enviroment" del servicio web y añadiremos las variables "PGUSER, PGPASSWORD, PGDATABASE, PGPORT y PGHOST", y añadimos los valores a las variables, sacado del postgres que habrá generado esos valores automáticamente.


