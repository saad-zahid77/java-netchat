# NetChat

This application is a simple text based chat application over TCP sockets in Java, with a support for just two people, and with the User Interface. The project is divided into two sub-projects, **ChatServer** and **ChatClient**, the **ChatServer** part is the code for running the server and **ChatClient** part is the code for running the client which would communicate with the server.



##  Building

####  Requirements

- JDK 1.7 or above
- Apache Ant 1.9.16 or above

```bash
ant jar
```

After the build is complete, the executable jar file would get created into `dist` directory.



##  Running

Once the jar files are created for each of the sub-projects, we can continue by first running the **ChatServer** which would host our chat over the network.

```bash
java -jar ChatServer/dist/ChatServer.jar
```

Then, setup the server by providing it with a name and a port number.

Once the server is running, it's time to run the **ChatClient** which would connect to the server over the network on the provided port number and the hostname / ip address of the **ChatServer** instance.

```bash
java -jar ChatClient/dist/ChatClient.jar
```

When both are setup, we can use the crappy GUI to chat using the server and client.
