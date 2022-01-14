# init the project 
docker-compose up --build

# run the project
docker-compose up

# See the data
http://localhost:8000/api/cleanings/


# check the fastapi docs
http://localhost:8000/docs

# Go to the docker bash
1. find the phresh_server container id
```
docker ps 
```
2. Go to the docker bash
```
docker exec -it <container id> bash
```

# Go to the psql 
```
docker-compose exec db psql -h localhost -U postgres --dbname=postgres

```


# Reference
```
https://www.jeffastor.com/blog/up-and-running-with-fastapi-and-docker
https://www.jeffastor.com/blog/pairing-a-postgresql-db-with-your-dockerized-fastapi-app
https://www.jeffastor.com/blog/hooking-fastapi-endpoints-up-to-a-postgres-database
```