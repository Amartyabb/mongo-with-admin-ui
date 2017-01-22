# mongo-with-admin-ui
Learn mongo and mongo-express. A project for launching docker based mongodb and admin ui (browser based) for learning basics of mongo db.


## Technology & Tools
  - [Docker](https://www.docker.com/)
  - [Docker Compose](https://docs.docker.com/compose/)
  - [Mongo DB](https://www.mongodb.com/)
  - [Mongo-Express](https://github.com/mongo-express/mongo-express)

## Dev setup
  1. Install Docker (choose suitable version for your OS)
    - [Mac](https://docs.docker.com/engine/installation/mac/)
    - [Windows](https://docs.docker.com/engine/installation/windows/)
    - [Linux](https://docs.docker.com/engine/installation/linux/)
  2. Install Docker Compose
    - [Instructions](https://docs.docker.com/compose/install/) 
  3. Clone this repo
  ```
    git clone git@github.com:ddffx/mongo-with-admin-ui.git

    cd mongo-with-admin-ui

    create a directory *dbData*, this directory used for mapping a volume for */data/db*

    mkdir dbData
  ```

## Run 
```
  docker-compose up 

  ## or if you would like to run the services in the background

  docker compose up -d
```

### Access the admin ui
Go to http://localhost:8081 in your browser
You can create new database, create collections, insert documents and query the collections.

### Access mongo shell
 - Open a terminal (mongo and admin ui are already running)
 - do `docker ps` to display the list of running containers for the services. Note the name of the mongo container, 
 in this case it is **mongowithadminui_mongo_1** and then run below to launch mongo shell
```
  docker exec -it mongowithadminui_mongo_1 mongo
```
