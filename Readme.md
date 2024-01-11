 **Node.js HTTP Server**

This is a simple Node.js HTTP server that listens on port 8080 and responds to requests with the message "Hello Node".

**How it works**

The server is created using the `http.createServer()` function, which takes a callback function as its argument. The callback function is called whenever a request is made to the server.

The callback function first writes the message "Hello Node" to the response object. Then, it calls the `end()` method on the response object, which sends the response to the client.

The server is then started using the `listen()` method, which takes the port number as its argument. The `listen()` method also takes a callback function as its argument, which is called when the server starts listening on the specified port.

**Code snippets**

Here are the code snippets that show how to create the server and start it:

```javascript
// Create the server
const server = http.createServer(function(req,res){

    res.write("Hello Node")

})
```

```javascript
// Start the server
server.listen(port,function(error){

    if(error){
        console.log("Something went wrong",error);
    }
    else{
        console.log("Server is listenig on port " + port);
    }

})
```

**Step-by-step explanation**

Here is a step-by-step explanation of how the code works:

1. The `http.createServer()` function is called to create the server.
2. The callback function is defined. This function is called whenever a request is made to the server.
3. The callback function writes the message "Hello Node" to the response object.
4. The callback function calls the `end()` method on the response object, which sends the response to the client.
5. The `listen()` method is called to start the server. The `listen()` method takes the port number as its argument.
6. The `listen()` method also takes a callback function as its argument, which is called when the server starts listening on the specified port.

**Conclusion**

This is a simple Node.js HTTP server that listens on port 8080 and responds to requests with the message "Hello Node". The code is well-commented and easy to understand, making it a good example for junior developers who are

