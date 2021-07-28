# Spring and Sockets

A __socket__ is one endpoint of a two-way communication link between two programs running on the network. A socket is bound to a port number so that the TCP layer can identify the application that data is destined to be sent to.

Normally, a server runs on a specific computer and has a socket that is bound to a specific port number. The server just waits, listening to the socket for a client to make a connection request.

On the client-side: The client knows the hostname of the machine on which the server is running and the port number on which the server is listening. To make a connection request, the client tries to rendezvous with the server on the server's machine and port. The client also needs to identify itself to the server so it binds to a local port number that it will use during this connection. This is usually assigned by the system.

In spring we do this by first creating a client side message and server side response (we can do it by creating simple java classes with message and respone fields), then we create controller with ` @MessageMapping` and `@SendTo` annotations to map a response for a message recieved. 

After that we need to configure a broker, which acts like a middleware between client-side and server, and that's done by implementing `WebSocketMessageBrokerConfigurer` with `@EnableWebSocketMessageBroker` annotation.
