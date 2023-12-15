Docker Commands
Container is the running version of image. You can consider container as mini server. It too have 0-65,535 ports.

1. To display the available images

   docker images

2. To pull the image from Docker Hub. If you dont mention version it will pull the latest version by default.

   docker pull [image-name]:[version]

3. To create container out of image

   docker create [image-id]

4. To display the running containers.

   docker ps

5. To display all the containers.

   docker ps -a

6. To start the container

   docker start [container-ID]

7. To pull, create and start the container with single command.

   docker run [image-name]:[version]

8. By default docker containers run in the foreground attached to the screen. If you want to detach use -d

   docker run -d [image-name]:[version]

9. To stop the running container

   docker stop [container-ID]

10. To remove the container. If it is running container use -f to force

    docker rm [container-ID]

11. To remove images.

    docker rmi [image-ID]

12. To assign a port to the container

    docker run -d -p [host-port]:[container-port] [image-name]:[version]

13. To name the container.

    docker run -d --name [name-you-wish] [image-name]:[version]

14. To login the container shell. To come out use CTRL+d

    docker exec -it [container-id] bash