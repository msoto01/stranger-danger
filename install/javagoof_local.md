# Java Goof on local machine
To start with, you’ll need to clone the java-goof repository, and build your application. The application can be found on GitHub here: [https://github.com/snyk/java-goof](https://github.com/snyk/java-goof).

Clone the repository onto your local file system

```
$ git clone https://github.com/benas/todolist-mvc.git
```

Open a terminal and run the following command from the root directory:

```
$ mvn install
```

Navigate into the ```todolist-web-struts``` directory and run the following to start the server:

```
$ mvn tomcat7:run
```