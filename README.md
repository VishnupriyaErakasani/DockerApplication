In this docker application we create an web application and push that into DockerDesktop
commands used:
1.docker build --platform linux/amd64 -t <username>/<directoryname>:local . 
2.docker images(check if docker image is creaed)
3.docker run --platform linux/amd64 -d -p 8081:8080 --name <directoryname>-local <username>/<directoryname>:local
4.curl http:localhost:8081 (To verify what we have built is successful in the web browser)
5.docker tag <username>/<directoryname>:local <username>/<directoryname>:latest(creating tags in docker)
6.docker push <username>/<directoryname>(Pushing it to dockerdesktop finally)
