# node-mongo-docker
A node and express docker template with Mongo


# build all the images and instruction that are set in the file docker-compose
docker-compose build 
# It will start eveything at the same time
# Note : In our case if mongo don't first our docker will throw errors
docker-compose up 
# To avoid this you can run mongo first 
docker-compose up -d mongo
# and now the app
docker-compose up -d app
# see the logs of the containers
docker logs <id of the container>
# stopping the container
docker logs <id of the container>

-- Pushpak Sharma