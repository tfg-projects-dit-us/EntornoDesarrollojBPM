# Servidores
## Funcionalidad
Estos ficheros permiten levantar los servidores necesarios para dar soporte al desarrollo de soluciones jbpm+fhir

Usar el comando ``docker compose up -d`` para arrancar los contenedores de fhir y business central
### Servidor fhir
Estará disponible en el puerto 8888 de la máquina host

Backend para la persistencia de la información clínica en formato FHIR R5

La configuración de este servidor está en el fichero application yaml que se monta en el contenedor
### Servidor Business Central (BC)
Estará disponible en el puerto 8080 de la máquina host

Servidor para el control del motor kie de la aplicación en modo development. Permite desplegar contenedores en el motor (modificando procesos si es necesario), ejecutar tareas humanas, etc... desde BC en caliente, es decir, sin necesidad de reiniciar la aplicación

Se monta la ruta al repositorio maven del máquina host en el contenedor, para que se comparta el mismo repositorio entre contenedor y host. Será necesario editar esta ruta en función de la configuración maven de la máquina host.
