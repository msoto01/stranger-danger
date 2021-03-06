# Using the docker images for Java Goof
- go to the "java_goof_docker" directory in the (unpacked) zip file

Import docker images
```
$ docker load -i javagoof.tar
```
Start application
```
$ docker-compose up
```
From a browser navigate to the following URL: [http://localhost:8080/](http://localhost:8080/).
You will see this application.

![Java Goof homepage](../images/image9.png)


### Important:

We will use be using the following tools
* [cUrl](https://curl.haxx.se/download.html) - download and install a binary for your OS
* [Httpie](https://httpie.org/) - (brew install httpie)

You can use these tools from your local machine **OR** you can access the Docker image that have these tools pre-installed

To access the shell
```
$ docker exec -it javagoof bash
```