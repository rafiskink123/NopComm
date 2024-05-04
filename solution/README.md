# Part I:

# As part of Part I execution below are the steps followed to achieve the scenario:

# to run a container of infracloudio/csvserver:latest in background, 

docker run -d infracloudio/csvserver:latest

# So as we know it has pulled the image from this hub to my local machine and then created the container and immediately moved to Exited state as expected.

* As per my analysis I have removed it and deleted by using docker rm <container ID> , then I have re-ran using tail -f /dev/null adding to the previous command

docker run -d infracloudio/csvserver:latest tail -f /dev/null


- now the container is active and running and able to login to it using  " docker exec -it <container-name> /bin/sh "

