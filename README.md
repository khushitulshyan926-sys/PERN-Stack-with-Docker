# PERN stack project along with Docker

To start with make server and run it to check the right connections.

Go to Server folder and run command:
- npm i express pg cors
- nodemon index

Then to connect with Postgres and setup run command:
- psql -U *DB Name* 

Make sure you enter the right password and connect to DB properly.

Then set up client side using the following commands in client folder:
- npx create-react-app client
- npm install(if project is cloned/mocked)
- npm start

This should be enough to run the PERN stack project in localhost.

After Completing the PERN stack go to Containerization of the client, server and db in this case using Docker.
To start with Docker file create run command:
- npm i express pg (makes changes in the server file)
- npm run dev

Create Dockerfile and specify image and other things in the compose file as well. Run command:
- docker build -t *image name* .
- docker compose up

This will create and run the docker image. This can be done for all client, server and db. These will be 3 images in 1 container.

Here to get a clear picture PERN is the container and client,postgres and server are 3 images. These images needs to be balanced and running so that the application is running smoothly. 

NOTE: You can install Docker Desktop ot easily manage and run the images and containers and commands can be run the docker CLI to manage images.

Congratulations! The project is nnow completed and up and running. It includes learning of Postgres, Express, ReactJS, NodeJs and Docker.

Reference: 
- https://www.youtube.com/watch?v=sDPw2Yp4JwE
- https://www.youtube.com/watch?v=ldYcgPKEZC8
