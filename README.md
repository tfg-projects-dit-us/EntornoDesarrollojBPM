# EntornoDesarrollojBPM
Este repositorio contiene los recursos necesarios para facilitar el despliegue del entorno de desarrollo y pruebas para proyectos kie+FHIR

Se presentan dos configuraciones:

## Fhir+BC
Incluye únicamente los servicios hapi fhir y Business central. En este caso será necesario montar en business central la ruta al repositorio maven del host, para que ambos compartan el mismo repositorio maven

## Fhir+BC+repo
Incluye, además de los anteriores, el servicio de repositorio de artefactos reposilite
