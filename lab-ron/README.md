Cowsay App:

This app uses an http server to return your phrase in the speech bubble of an animal.

Starting the server:

node server.js or nodemon server.js

Server Endpoints:

GET request to /

This will return a string that says 'Hello World'.

GET request to /cowsay

Use a query string to return the message of your choice.

Here is what the command looks like:

curl 'localhost:3000/cowsay?text=message&animal=dragon'

POST request to /cowsay

You may POST a talking cow by posting to /cowsay.

Here is what the command looks like: curl -i -H "Accept: application/json" -H "Content-Type: application/json" -X POST -d '{"text": "message"}' localhost:3000/cowsay
