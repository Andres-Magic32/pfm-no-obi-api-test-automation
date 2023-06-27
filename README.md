# pfm-no-obi-api-test-automation
Proyecto  de automatización de pruebas  para PFM API (sin  obi)

Esta colección de Postman ha sido creada con el objetivo de optimizar y mejorar el proceso de pruebas y aseguramiento de la calidad en nuestro proyecto [PFM]. Como QA, he recopilado y organizado cuidadosamente una serie de solicitudes API esenciales que representan los principales escenarios y funcionalidades críticas de nuestra aplicación.

## Conjuntos de pruebas

Además de las solicitudes individuales, se han creado también diversos conjuntos de pruebas (test suites) para validar de forma automática la correcta respuesta de la API ante diferentes escenarios. Estas pruebas están basadas en aserciones predefinidas que verifican tanto los datos retornados como los códigos de estado.

### Planes de pruebas anexados.

#### Test Automation PFM no OBI | e2e | API.

Esta se encarga de realizar un flujo completo sobre la api teniendo como alcanze los siguientes modulos. access

users
financial entities
accounts
categories
transactions
budgets
country
insights

## Instrucciónes de uso.
Validar la versión de node de nuestro sistemas en caso de no tenerlas instalar por por favor. 

#### node --version

Instalar herramienta newman cli, el cual nos permitira ejecutar las pruebas el cual se instala mediante npm

#### npm install -g newman

Instalar el reporteador para que se genere el documento html con el detalle de las pruebas.

#### npm install -g newman-reporter-html

Para ejecutar las pruebas en la carpeta raiz donde se encuentren los archivos json usar el comando. 

#### newman run  PFM_Collection.postman_collection.json -e PFM_Environmet.postman_environment.json -r htmlextra --reporter-htmlextra-title "Informe de prueba PFM no OBI"

Gracias por tu tiempo.
