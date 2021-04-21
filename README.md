# go-jwt-http-form-server
go front end server, proxy to backend server and Postgres database.

This project uses 3 go programs: the first is the frontend server that the client
interacts with. The 2rd go program is a proxy server which takes request from the
frontend and redirects them to the backend server. The backend server processes 
the client requests along with database access. We are using JWT tokens to authenticate 
with the backend server. JWT tokens are sent via http headers. The backend server is
using the Postgres database for user validation and data that the client requests.
Software used: go program language and Postgress database. The backend server is using
"github.com/dgrijalva/jwt-go" for JWT tokens.
