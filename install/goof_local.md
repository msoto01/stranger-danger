#Goof on local machine

In a terminal, start mongod, using the following command:

```
$ mongod &
```

Next you’ll need to fork the goof repository, clone it and build your application. The application can be found on GitHub here: [https://github.com/snyk/goof](https://github.com/snyk/goof).

Fork this application to your local repository so that any remediation you choose to perform will only happen on your repository and won’t affect others in this workshop.

Clone the repository onto your local file system and navigate into the project’s root directory. Run the following commands to download the dependencies for the goof application:

```
$ npm install
```

Your application should be ready to run. You can start the application by running the following command from within the main project directory:

```
$ npm start
```

From your browser of choice, navigate to [http://localhost:3001](http://localhost:3001) and you should see the following page.

![Goof homepage](../images/image12.png)