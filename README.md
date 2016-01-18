# Socket_07
Desarrolla un servidor web multihebra capaz de recibir varias solicitudes en paralelo; se
trata de implementar la versión 1.0 de HTTP, tal y como la define el documento RFC 1945.
HTTP/1.0 crea una conexión TCP separada para cada par solicitud/respuesta. Una hebra
separada gestiona cada una de las conexiones. También habrá una hebra principal en la que
el servidor escuche a los clientes que deseen establecer una conexión. Para simplificar la
tarea de programación, desarrollaremos el código en dos etapas. En la primera, escribiremos
el código para un servidor multihebra que simplimente muestre el código del mensaje de
solucitud HTTP que haya recibido. Una vez que este programa se ejecute correctamente
deberemos añadir el código necesario para generar una respueta apropiada.
A medida que vayas desarrollando el código, puedes probar tu servidor con un navegador
web. Pero recuerda que no estás proporcionando el servicio a través del puerto estándar 80,
por lo que habrá que especificar un número de puerto dentro de la URL que proporciones al
navegador. Por ejemplo, si el nombre de host es hos.unaEscuela.edu, tu servidor está
escuchando en el puerto 6789 y deseas recuperar el fichero index.html, entonces tendrás que
especificar la siguiente URL en el navegador:
http://host.unaescuela.edu:6789/index.html
Cuando tu servidor detecte un error, deberá enviar un mensaje de respuesta con el código
fuente HTML apropiado, de manera que la información a cerca del error se muestre en la
ventana del navegador.
