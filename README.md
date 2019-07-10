# nodejs
### create a HTTP server?

```HTTP``` module is Node.js ```core module```(a module included in Node.js's source, that does not require installing additional resources). 
-- The http module provides the functionality to create an HTTP server using the ```http.createServer()``` method.

Ex:
```const http = require('http');
http.createServer((req,res) => {
  res.writeHead('200',{
  'Content-Type': 'text/plain'
  });
  res.write('Hello, World!\n');
  response.end();
}).listen(8081);
```
### what is express? How can we use it?
```Express.js``` is a commonly-used web framework that is useful for creating HTTP API's. It is especially designed for building single-page, multi-page, and hybrid web applications.

__Command to install__ : ```npm install express --save```

Ex:```
const express = requires('express');
const app = express();
const port = 3030;
app.get('/user, function(req, res){
  res.send("Users list");
});

app.listen(port, function() { // making the app listen on port 3030
console.log('Server listening on http://localhost:' + port);
}); ```

### Basic routing in nodejs?

Ex:
```
const http = require('http');
function index(req, res){
  res.writeHead(200);
  res.end('hello world');
}
http.createServer(function(req, res){
  if(req.url === '/'){
    response.writeHead(404);
    response.end(http.STATUS_CODES[404]);
}).listen(1337);
```
###

  
