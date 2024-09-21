## Frontend with React

## Backend with Node and FastAPI

## MongoDB for data storage
- if you wish to run this application on your local machine, fork and clone the repo down and create a mongodb cluster using node.js and put the URI in a .env file in the root of the project
- then proceed to the docker compose cmd below

## Docker used to run 3 main sections. 
- The nginx reverse proxy that routes the request to the front and backend
- the nodejs frontend application and
- the python based backend application.

**This usage of Docker Compose is going to create a consistent repreducable development environment that closely mimics the production setup and we can start the enitre application stack with all three containers with a single command. **

**use this cmd in the root directory of the project:**
`docker compose up --build`
