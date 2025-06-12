# jwt-demo 
Este proyecto valida el contenido de un JWT,
el secret del cual se genero fue "SFRU/TKNnLyKcUEMyVxO82c5gatSHbvHBWYAlyQ90HI=" y 
para validar el contenido se utilizo la pagina de https://jwt.io/ en donde se puede cambiar las propiedades de "sub",
"name" de la seccion de PAYLOAD, ademas de que en bloque de "VERIFY SIGNATURE" se necesita agregar el secret antes mencionado.

Una vez que esto se haga se puede probar el servicio expuest en http://localhost:8080/api/whoami pasando el Header de
Authorization con el valor de "Bearer <token>" este token es el brindado de la pagina de https://jwt.io/.
Para levantar el servicio en local, como cualquier proyecto Java (version 17 para este caso) hace falta clonarlo, construirlo (mvn clean install), y levantarlo (mvn spring-boot:run).
