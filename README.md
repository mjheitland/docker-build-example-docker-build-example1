# How to build a Docker image and push it to Docker Hub

Details see https://docs.docker.com/docker-hub/ 


1. Login to Docker Hub and create a repository mjheitland/webserver: https://hub.docker.com/
2. Build image and push it to Docker Hub:
-    docker build -t mjheitland/webserver .
-    docker login
-    docker push mjheitland/webserver
-    docker rmi mjheitland/webserver
-    docker pull mjheitland/webserver
-    docker run -d --name webserver -p 80:80 mjheitland/webserver

Running http://localhost:80 in your browser should show "Now it works!"
