# Docker Project
   Small Project Servlet/Postgres/Docker
   usando [GitHub Pages](https://pages.github.com/)
## URL's:

- GET: [localhost:8080/my-webapp/ola](http://localhost:8080/my-webapp/ola) - Msg of HelloWorld
- GET: [localhost:8080/my-webapp/book_entities](http://localhost:8080/my-webapp/book_entities) - Create database and table in PostgreSQL
- POST: [localhost:8080/my-webapp/books](http://localhost:8080/my-webapp/books) - Insert one register of test
- List: [localhost:8080/my-webapp/books](http://localhost:8080/my-webapp/books) - List inserted books
   
## Clone and execute

1. Clone the project
```
clone marcoseduardos...
```

2. Compile the project
```
mvn install
```

3. Run in root of project
```
docker-compose up -d
```

## Stop and remove

1. Stop the project
```
docker container kill my-webapp my-database
```
- Note: For stop all containers, execute: "docker container kill $(docker container ls -aq)"

- Note: **Kill** option is faster with **stop**

2.Remove containers:
```
docker container rm my-webapp my-database
```
3.Remove image:
```
docker rmi my-tomcat:1.0
```
- Note: For remove all containers, execute: "docker container prune"
