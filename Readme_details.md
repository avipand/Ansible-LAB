Some point need to remember during running ansible :
-----------------
user : ansible
password : ansible

-----------------
Some command must to know to manage images :

1. Running of docker composefile .
          docker-compose up
2. Stopping of docker composefile.
          docker-compose stop
3. Deleting conatiner 
          docker rm <conatiner id>
4. Deleting images
          docker rmi <image_id>
5. Checking of docker container id
          docker ps - a
6. Checking of docker images id
          docker images
7. command to remove all images
          docker rmi -f $(docker images)
8. command to remove all conatiner 
          docker rm -f $(docker ps)
