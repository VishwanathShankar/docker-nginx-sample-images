To start a docker nginx
docker run -it --rm -d -p 8080:80 --name test-webapp nginx

TO stop the container
docker stop test-webapp

To create a custom docker image
docker build -t webapp-2 . 

To run the custom docker image
docker run -it --rm -d -p 8081:80 --name app2 webapp-2

To stop the custom docker image
docker stop app2
