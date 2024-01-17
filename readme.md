#Use the Dockerfile to build and run the container with proper port connection and name according to you
docker build -t phpdocker .
docker run -dp 0.0.0.0:3000:80 phpdocker

#To upload the Docker image into the dockerhub
#login with your credential and then replace the repo name with yours
docker images
docker login
docker image tag 61e81c89fc89 sekuwa/devops-assesment:phpdocker
docker push sekuwa/devops-assesment:phpdocker


