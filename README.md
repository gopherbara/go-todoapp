# go-todoapp
backend for todo-app with PostgreSQL

Try develop app with principles of Clean Code.
Backend todoapp using PostgreSQL for saving data at relational database.

## Small description
Layers:
handler - get http request and handle it, send it to service - depends from service.
service - (business) logic of project, connect with database (repository) - depends from repository.
repository - realization of database requests.

Any layer can be changed and everything gonna work as before (can change database to any other (for example Microsoft SQL Server) and app still work).
Communication between layers throught interfaces

## Use

PosgreSQL - relational database for saving data.

github.com/lib/pq - driver for PostgreSQl.
https://github.com/jmoiron/sqlx - for working with database.
https://github.com/golang-jwt/jwt - for generating and parsing jwt tokens.
https://github.com/gin-gonic/gin - for initializing routes.
https://github.com/joho/godotenv - for setting and use of enviroment variables.
https://github.com/spf13/viper - for work with config.yml
