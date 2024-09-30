#postgres 
# Using Docker

## Pull Postgres Image

Pull the latest Postgres image.

`docker pull postgres`

## Configure and Run Server

Run the image, provide a server name, and password. The `-e` sets an environment variable, the `POSTGRES_PASSWORD` is required to start the server. More about Docker specific environment variables can be found [here](https://www.docker.com/blog/how-to-use-the-postgres-docker-official-image/#:~:text=1.-,Environment%20variables,-We%E2%80%99ve%20touched%20briefly).

`docker run --name [SERVER_NAME] -e POSTGRES_PASSWORD=[PASSWORD] -d postgres`

## Connecting to PostgreSQL Server

Before connecting you may want to [[PostgreSQL Version|check your version]] of Postgres.

`psql -h [HOST] -p [PORT] -U [USERNAME] [SERVERNAME]`

`HOST` is the IP to access, localhost is possible.

`PORT` the default value for Postgres servers is `5432`.

`USERNAME` denotes the user which you would like to access the server as. 
*When not provided defaults to the current user's name.*

`SERVERNAME` denotes the name of the server.
*Not always needed.*

### Example Command for Connection to the Server

`psql -h localhost -p 5432 -U admin my-postgres-server`