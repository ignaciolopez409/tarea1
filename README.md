# tarea1
Para realizar la tarea implementé Jenkins y SonarQube sobre un servidor Centos utilizando Docker compose, un repositorio en GitHub donde se encuentra el pipeline (https://github.com/ignaciolopez409/tarea1), un repositorio donde se encuentra el código a construir para poder realizar los tags y actualización de versión mediante el plugin de release de Maven (ignaciolopez409 / orders-service-example) y las imágenes Docker generadas se publican en el repositorio de mi cuenta de hub.docker: https://hub.docker.com/r/ignaciolopezventimiglia/orders-service-example/tags. 
Al ejecutar el pipeline se debe indicar mediante parámetros el proyecto a generar (dejando abierta la posibilidad de con el mismo pipeline generar todos los microservicios del laboratorio realizado a futuro) y el tipo de tarea Maven a ejecutar (build o release). En ambos casos se ejecuta el análisis de SonarQube. Una vez construido el proyecto se realiza el tag y publicación de las imágenes Docker correspondientes a la versión para cada uno de los ambientes (dev, test y stage).

