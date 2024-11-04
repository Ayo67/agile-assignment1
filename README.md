## Docker Assignment - Agile Software Practice.

__Name:__ Ayo Oguntuyi

__Demo:__ (https://www.youtube.com/watch?v=AZDe9ndqAGk)

This repository contains the containerization of the multi-container application illustrated below.

![](./images/arch.png)

### Database Seeding.
In this application, i have automated the seeding of the application's database by creating a separate container "mongodb-seed" within the docker-compose file. This container is responsible for loading the initial data into MongoDb

### M.ulti-Stack.
To support both development and production stack i created a dev profile which inclues "mongo-express" and "mongodb-seed", these services are only started when the "--profile dev up" command is run while the "docker compose up" command excludes those features.
