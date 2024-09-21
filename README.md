
<div align="center">
  <div>
    <img src="https://shields.io/badge/react-black?logo=react&style=for-the-badge" alt="reactjs" />
    <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black" alt="javascript" />
    <img src="https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white" alt="docker" />
    <img src="https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi" alt="fastapi" />
  </div>
</div>

## Frontend with React (JavaScript)

## Backend with Node and FastAPI (python)

## MongoDB for data storage
- if you wish to run this application on your local machine, fork and clone the repo down and create a mongodb cluster using node.js and put the URI in a .env file in the root of the project
- then proceed to the docker compose cmd below

## Docker Compose -Containerize the entire applciation by running 3 main sections. 
- The nginx reverse proxy that routes the request to the front and backend
- the nodejs frontend application and
- the python based backend application.

**This usage of Docker Compose is going to create a consistent repreducable development environment that closely mimics the production setup and we can start the enitre application stack with all three containers with a single command. **

**use this cmd in the root directory of the project:**
`docker compose up --build`


### FastAPI dependency notes:
**fastapi[all]** - the all includes add depenciencies like uvicorn for serving the app
Comment
Suggest edit
Edit from here

**motor** - asyncronous mongodb driver for python (we are using the SRV extra which adds support for mongodb's SRV connection strings)

**beanie** - object document mapper for mongodb built ontop of motor (allows us to defgine our data models as python classes and provides an intuitive API for database opperations)

**aiostream** - package provides tools for working with ayncronous streams which can be usefull when dealing with large datasets or real time data.

(After initial setup you can use 'pip install -r requirments.txt' if fork/cloning repo)
