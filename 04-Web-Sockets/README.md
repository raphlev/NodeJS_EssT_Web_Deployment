# ./client directory contains chat application

npm install -g serve
serve ./client

Leave client app running on port 5000 for next section using ws

# Web Server with ws package using native client ws

https://www.npmjs.com/package/ws

ws is a simple to use, blazing fast, and thoroughly tested WebSocket client and server implementation.
Passes the quite extensive Autobahn test suite: server, client.
Note: This module does not work in the browser. The client in the docs is a reference to a back end with the role of a client in the WebSocket communication. Browser clients must use the native WebSocket object. To make the same code work seamlessly on Node.js and the browser, you can use one of the many wrappers available on npm, like isomorphic-ws.

npm install ws
node 01-socket-server-With-ws.js
http://localhost:3000/
start using chat with different tabs in Web Browser

# Web Server with more robust socket.io package that will replace WebSocket by HTTP if WebSocket is not supported by Browser

This section is not useing ./client app

npm install socket.io
npm install socket.io-client

Execution: in 3 different Terminal run:

- node 02-socket-server-With-socket.io
- node socket-client.js
- node socket-client.js
