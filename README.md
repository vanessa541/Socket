# Sockets
documentacion de sockets
## El módulo Socket en Python, es un canal de comunicación que permite conectar dos equipos a través de la red (normalmente cliente-servidor). La separación entre cliente servidor en estas conexiones es de tipo lógico. Esto significa que no es necesario tener corriendo el servidor en una única máquina, sino que puede estar en varias, e incluso en varios programas. Socket es un módulo estándar del lenguaje de programación Python (y de otros muchos) que proporciona una interfaz de bajo nivel que permite conexiones TCP/IP y UDP. Esto ofrece soluciones sencillas a problemas sencillos.
https://www.escribecodigo.com/sockets-en-python/ 

### Tipos de sockets
https://docs.python.org/3/library/socket.html 
#### SOCK_RAW 
##### El modo RAW está básicamente ahí para permitirle omitir parte de la forma en que su computadora maneja TCP / IP. En lugar de pasar por las capas normales de encapsulación/desencapsulación que hace la pila TCP/IP en el kernel, simplemente pasa el paquete a la aplicación que lo necesita. No hay procesamiento TCP/IP, por lo que no es un paquete procesado, es un paquete sin procesar. La aplicación que está usando el paquete ahora es responsable de quitar los encabezados, analizar el paquete, todas las cosas que la pila TCP / IP en el kernel normalmente hace por usted
#### SOCK_RDM
##### SOCK_RDM modela la semántica de datagramas confiables en modo sin conexióncomunicación. Los mensajes llegan sin duplicar y en orden, y se notifica al remitente si los mensajes se pierden. Un socket de tipo SOCK_RDM no requiere configuración de conexión antes. La comunicación puede comenzar y puede comunicarse con múltiples compañeros.
#### SOCK_SEQPACKET
##### SOCK_SEQPACKET modela circuitos virtuales basados en conexión con límites de registro y proporciona una transferencia bidireccional fiable de flujos de bytes ordenados sin duplicación de datos, al tiempo que se conservan los límites dentro del flujo de datos. Un zócalo de tipo SOCK_SEQPACKET. Se comunica con un único interlocutor y requiere la configuración de la conexión antes de que la comunicación pueda empezar
#### SOCK_PACKET
