# Node.js
## What is Node.js?

Node.js is a JavaScript runtime built on Chrome's V8 JavaScript engine that allows JavaScript to be run on the server side.

## What is the event loop in Node.js?

The event loop is the mechanism that allows Node.js to perform non-blocking asynchronous operations by handling I/O operations in a single thread.

## What are streams in Node.js?

Streams are objects that enable reading or writing data in a continuous flow. There are four types of streams: Readable, Writable, Duplex, and Transform.

## What is the difference between require() and import in Node.js?

require() is the CommonJS module system, used in Node.js for importing modules.
import is part of ECMAScript modules (ESM), introduced for JavaScript to allow imports and exports in the same way across all environments.
## What is the fs module in Node.js?

The fs module provides file system-related functionality, such as reading, writing, and manipulating files.

## What is Express.js in Node.js?

Express.js is a web application framework for Node.js that simplifies routing, middleware handling, and HTTP request/response management.

## How do you handle errors in Node.js?

Errors in Node.js can be handled using try-catch blocks for synchronous code or by using callback functions with error arguments or Promises for asynchronous code.

## What is middleware in Express.js?

Middleware is a function that has access to the request, response, and the next middleware function in the application’s request-response cycle.

## What is the http module in Node.js?

The http module is used to create HTTP servers and clients for handling requests and responses.

## What is the difference between __dirname and __filename in Node.js?

__dirname: Represents the directory name of the current module.
__filename: Represents the full path to the current module file.
## What is the process object in Node.js?

The process object provides information and control over the current Node.js process, such as environment variables, exit codes, etc.

## How do you create a simple HTTP server in Node.js?

You can use the http module to create a basic server:

```js
Copy
const http = require('http');
http.createServer((req, res) => {
    res.write('Hello, World!');
    res.end();
}).listen(3000);
```
## What are callbacks in Node.js?

Callbacks are functions passed as arguments to other functions and are executed after an asynchronous operation is completed.

## What is require() in Node.js?

require() is used to import modules, JSON files, and local files into a Node.js application.

## What is the buffer module in Node.js?

The buffer module is used to handle binary data directly in memory, especially for I/O operations such as file manipulation or HTTP requests.

## What is npm in Node.js?

npm is the Node Package Manager, a tool for managing dependencies, libraries, and modules in a Node.js project.

## What is asynchronous programming in Node.js?

Asynchronous programming in Node.js allows non-blocking execution by utilizing callbacks, Promises, and async/await.

## What is the cluster module in Node.js?

The cluster module enables the creation of child processes (workers) to handle concurrent operations, taking advantage of multi-core systems.

## What is EventEmitter in Node.js?

EventEmitter is a core Node.js module that allows objects to emit and listen to custom events.

## What is setTimeout() in Node.js?

setTimeout() is a Node.js function that allows you to execute a function after a specified delay.

