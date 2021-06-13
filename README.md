https://www.youtube.com/watch?v=Dm0CmZz-QyI

Commands:
server:

1. docker build . -tag image-name
2. docker run --name container-name -p port:port -d image-name

server-postgres

1. docker run --name postgresdb-container-name -e POSTGRES_PASSWORD=123456 -d -p 4321:5432 postgres
2. docker exec -it postgresdb-container-name psql -U postgres-user-name
3. docker compose up --build -d
4. docker exec server-container-name npm run migrate // Run migration file
5. docker exec server-container-name npm run seed // Add dummy users to the database
6. docker volume ls
7. docker compose down
