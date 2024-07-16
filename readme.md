<h1>1. ¿Que es un microservicio?</h1>
<div align="center">
<p width="700">Spring Cloud proporciona herramientas para que los desarrolladores construyan rápidamente algunos de los patrones habituales en los sistemas distribuidos (por ejemplo, gestión de la configuración, descubrimiento de servicios, disyuntores, enrutamiento inteligente, microproxy, bus de control, microservicios de corta duración y pruebas de contratos).</p>

<img src="https://miro.medium.com/v2/resize:fit:720/format:webp/1*cTPRDoBveeNbz9QAi5XJJg.png" width="500">

<br>

![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)&nbsp;
</div>
<br>

<h1>2. ¿Cómo funciona el ecosistema de Spring Framework?</h1>
<div align="center">

<h2>como funciona el ecosistema?</h2>

<p>
El ecosistema Spring Boot proporciona múltiples características para que el desarrollo se centre en la lógica de negocio y en el rápido desarrollo de aplicaciones en lugar de dedicar tiempo a las configuraciones manuales. La integración de frameworks como React y Angular y bases de datos crea un potente ecosistema de desarrollo de aplicaciones.
</p>
<br>
<br>
<ul align="start">
  <li><h2>Spring Core:</h2>
    <ol>
        Spring Core es el fundamento de Spring Framework. Simplifica el desarrollo Java a través de la Inyección de Dependencias (DI), gestionando el ciclo de vida de los objetos. Esto promueve la modularidad y la testabilidad del código, haciendo más fácil crear aplicaciones escalables y mantenibles.
    
</ul>
<br>
<ul align="start">
  <li><h2>Spring MVC: </h2>
    <ol>
    Spring MVC es un framework web de Java que facilita el desarrollo de aplicaciones web siguiendo el patrón Modelo-Vista-Controlador (MVC). Simplifica la gestión de solicitudes HTTP, la creación de vistas y la integración con otras tecnologías Spring. Es ideal para construir aplicaciones web robustas y escalables.
</ul>
<br>
<ul align="start">
  <li><h2>Spring Data: </h2>
    <ol>
    Spring Data simplifica el acceso a bases de datos. Ofrece una API unificada para interactuar con diversas fuentes de datos, reduciendo código y facilitando operaciones CRUD y consultas complejas. Ideal para aplicaciones que necesitan persistir datos de manera eficiente.
</ul>
<br>
<ul align="start">
  <li><h2>Spring Security: </h2>
    <ol>
    Spring Security es un framework que proporciona una capa de seguridad robusta para aplicaciones Java. Simplifica la implementación de funcionalidades como autenticación, autorización, protección contra ataques comunes y gestión de sesiones. Es altamente configurable y se integra perfectamente con otros módulos de Spring, permitiendo proteger tus aplicaciones de manera efectiva.
</ul>

<img src="https://miro.medium.com/v2/resize:fit:2000/1*i-jDIr4DVxiNuObYCKvaXA.jpeg" width="500">

<br>

![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)&nbsp;


</div>

<br>
<br>
<h1>3. ¿Qué es Eureka y para qué sirve?</h1>
<div align="center">
<h3>¿Qué es Eureka?</h3>

Eureka es una pieza fundamental dentro del ecosistema de Spring Cloud Netflix. Imagina una gran ciudad donde cada edificio representa un microservicio. Eureka es como una guía telefónica gigante que te permite encontrar rápidamente cualquier edificio que necesites. En términos técnicos, es un servicio de registro que actúa como un directorio centralizado para todos tus microservicios.

<h3>¿Cómo funciona como servicio de descubrimiento?</h3>

Cuando inicias un microservicio, se registra automáticamente en Eureka, proporcionando información como su dirección IP y puerto. De esta manera, Eureka mantiene una lista actualizada de todos los microservicios disponibles en tu aplicación.

Si un microservicio necesita comunicarse con otro, simplemente consulta a Eureka. Eureka le proporcionará la dirección del servicio que busca, permitiéndole establecer una conexión de forma directa y eficiente. Esto elimina la necesidad de codificar direcciones estáticas en cada microservicio, lo que hace que tu aplicación sea más flexible y fácil de mantener.

<b>En resumen</b>, Eureka es el corazón del descubrimiento de servicios en Spring Cloud Netflix. Al proporcionar un mecanismo centralizado y dinámico para localizar microservicios, facilita la construcción de aplicaciones distribuidas robustas y escalables. Es como tener un GPS para tus microservicios, siempre listo para guiarte hacia el servicio que necesitas.


<img width="500" src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhcMZBv7AZQvpLEMR7kO9p7QAR6gN7EsYQnkDJz6rG0m2sgCnflPr4rZoXwW8HZv2Y7KU9mMa_JHVen62eYiG81hNZYm1saPpfuBJGjlD-XMS0sMkpn9nHQYbFSaBoXwnPzxA0ac8j-L0irv85FEuu7KG2jFzzWMtl6FRnY0bv1XTVYTugS_SK9lDGD/s1920/Spring%20Boot%20Microservices.012.jpeg">

<br>

![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)&nbsp;
</div>

<br>
<br>
<h1>4. ¿Qué es Discovery Server?</h1>
<div align="center">
<h3>¿Qué es un Discovery Server?</h3>

Imagina una ciudad grande y compleja donde cada edificio representa un microservicio. Para que los habitantes (o en este caso, los microservicios) puedan encontrar el lugar que necesitan, existe una guía telefónica centralizada. Ese es, en esencia, un Discovery Server.

En una arquitectura de microservicios, un Discovery Server actúa como un registro central donde cada servicio se inscribe al iniciar. Al registrarse, proporciona información crucial como su dirección IP, puerto y nombre. De esta manera, cuando un servicio necesita comunicarse con otro, simplemente consulta el Discovery Server, que le indica la dirección exacta.

<h3>¿Cómo funciona como punto central de registro y descubrimiento?</h3>
<ol align="start">
  <li><b>Registro:</b> Al iniciarse, cada microservicio se registra en el Discovery Server, proporcionando sus datos de contacto.</li>
  <li><b>Consulta:</b> Cuando un servicio necesita otro, consulta al Discovery Server para obtener su dirección.</li>
  <li><b>Descubrimiento:</b> El Discovery Server busca en su base de datos y devuelve la información del servicio solicitado.</li>
  <li><b>Comunicación:</b> Con esta información, el servicio puede establecer una conexión directa.</li>
</ol>

<img src="https://miro.medium.com/v2/resize:fit:1400/0*dE4Df3LmyNpH94lz" width="500">

<br>

![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)&nbsp;
</div>

