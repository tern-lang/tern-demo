ternlang
==============

Snap is an open source, optionally typed, object oriented scripting language for the Java platform. 
The learning curve is small for anyone with experience of Java, JavaScript, TypeScript, or Scala, 
amongst others. It has excellent integration with the host platform, and can do whatever can be 
done with Java and much more.

The language is ideal for embedding in to an existing application, and is a fraction of the size of 
similar languages for the Java platform. In addition to embedding it can be run as a standalone 
interpreter and has an development environment which allows scripts to be debugged and profiled.

[http://tern-lang.org/](http://tern-lang.org/)

#### Development Environment

Snap comes with a development environment that is available over HTTP on any web browser that 
supports Web Sockets. To develop and debug scripts the devlopment environment can be started with 
the command shown below. All that is required is a web browser and Java 1.5 or greater. The 
development environment is a single JAR file that can be downloaded from 
[here](https://github.com/ternlang/snap-release). In addition an embeddable version is available
which can be integrated in to any Java application.

*java -jar ternd.jar --mode=develop --directory=work --port=4457*

The development environment can use hot stand-by agents to improve responsiveness, the agent pool 
can be configured on the command line. In addition an agent can connect through the HTTP port using 
the HTTP CONNECT request and begin a debug session. An example configuration is shown below.

*java -jar ternd.jar --mode=develop --directory=work --port=4457 --agent-pool=4 --server-only=true*
