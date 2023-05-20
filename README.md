# docker
To build our image, run the following command:

```
$ docker build -t webserver .
```
Now we can run our image in a container but this time we do not have to create a bind mount to include our html.
```
$ docker run -it --rm -d -p 8080:80 --name web webserver
```
Open your browser and navigate to http://localhost:8080 to make sure our html page is being served correctly.
