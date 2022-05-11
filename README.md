To launch this web app perform the following steps:

# Launches all of the infrastructure including the user-wishlist-app, postgres-SQL, reddis containers,
# and a bridge network (see note below)
docker-compose up

Open a web browser to http://localhost:80

Note:
I modified the docker-compose.yml to use the image from my DockerHub repo. However, if you want to build the image locally
just uncomment line 4 and comment out line 5 as follows:

docker-compose-yml:
    build: ./
    # image: skdavidson/user-wishlist-app

# If you're building the dockerfile locally run this command BEFORE docker-compose up. 
# Build the user-wishlist-app image 
docker-compose build

Source: 
- Git:      https://github.com/cloudxlab/user-wishlist-app
- YouTube:  https://www.youtube.com/watch?v=ZTpEK3dEZVk