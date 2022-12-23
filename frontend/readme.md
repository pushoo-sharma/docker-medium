# build the image from the dockerfile
docker build -t classy-end-aws-frontend .
# then check the images
docker images
# remove the images
docker rmi <image id>
# run the image 
docker run -p 3000:3000 classy-end-aws-frontend
# checking the conatiner
docker ps
# stoping the conatiner
docker stop <id of the container>


-- Pushpak Sharma