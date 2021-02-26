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

To do a docker login for laptop
Set the proxy in Docker proxy tab
Turn on manual DNS configuration in docker proxies tab
https://stackoverflow.com/questions/49387263/docker-error-response-from-daemon-get-https-registry-1-docker-io-v2-servic


To push the docker image to docker hub
docker login
docker tag webapp-1 <dockerid>/webapp-1
docker push <dockerid>/webapp-1
