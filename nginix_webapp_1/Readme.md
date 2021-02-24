To start a docker nginx
docker run -it --rm -d -p 8080:80 --name test-webapp nginx

TO stop the container
docker stop test-webapp

To create a custom docker image
docker build -t webapp-1 . 

To run the custom docker image
docker run -it --rm -d -p 8080:80 --name app1 webapp-1

To stop the custom docker image
docker stop app1
