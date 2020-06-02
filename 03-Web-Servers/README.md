# Web Server with Server to server static files
./client directory contains client app with Dictionary

npm install -g serve

serve ./client

# Web Server with Express and Express Middleware to server static + dynamic routes
npm install
node server.js

http://localhost:3000/

- express server that serves static file in ./client (react app)
- express serves also dynamic routes from client front-end
  http://localhost:3000/dictionary/ : GET (from client app and also from web browser) - list all ski terms in json
  http://localhost:3000/dictionary/ : POST (from client app and also from postman)
  http://localhost:3000/dictionary/:term : DELETE :term=id of the ski terms (from client app using the delete button and also from postman)
