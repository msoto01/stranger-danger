# Using the docker images for Goof

- go to the "goof" directory in the (unpacked) zip file

Import docker images
```
$ docker load -i snyk-demo-todo_goof.tar
$ docker load -i mongo.tar
```
Start application
```
$ docker-compose up
```
From your browser of choice, navigate to [http://localhost:3001](http://localhost:3001) and you should see the following page.

![Goof homepage](../images/image12.png)

### Important:

We will use be using the following tools
* [cUrl](https://curl.haxx.se/download.html) - download and install a binary for your OS
* [Httpie](https://httpie.org/) - (brew install httpie)

You can use these tools from your local machine **OR** you can access the Docker image that have these tools pre-installed

To access the shell (this is only needed if you do not have cUrl on your local machine)
```
$ docker exec -it goof bash
```