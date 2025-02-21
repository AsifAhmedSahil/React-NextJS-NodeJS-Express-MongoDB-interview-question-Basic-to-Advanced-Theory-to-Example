# Express.js
## What is Express.js?

Express.js is a minimal and flexible Node.js web application framework that provides a robust set of features for building web and mobile applications, including routing, middleware support, and easy handling of HTTP requests and responses.

## How do you create a basic Express app?

To create a basic Express app:

```js
Copy
const express = require('express');
const app = express();
app.get('/', (req, res) => {
    res.send('Hello World');
});
app.listen(3000, () => {
    console.log('Server running on port 3000');
});
```
## What are middleware in Express?

Middleware functions are functions that have access to the request, response, and the next middleware function in the application’s request-response cycle. They can modify the request and response objects, end the request-response cycle, or call the next middleware function.

## How do you handle POST requests in Express?

Express provides the .post() method to handle HTTP POST requests. You can access request data using req.body (after configuring body parsing middleware).

```js
Copy
app.post('/submit', (req, res) => {
    res.send('Data received');
});
```
## How do you parse JSON in Express?

To parse JSON in Express, you can use the built-in express.json() middleware.

```js
Copy
app.use(express.json());
How do you handle query parameters in Express?

You can access query parameters in Express using req.query.
```
```js
Copy
app.get('/search', (req, res) => {
    const { term } = req.query;
    res.send(`Searching for ${term}`);
});
```
## What are route parameters in Express?

Route parameters are dynamic segments of the URL in the route path. You can access them via req.params.

```js
Copy
app.get('/user/:id', (req, res) => {
    res.send(`User ID: ${req.params.id}`);
});
```
## How do you handle errors in Express?

Express provides an error-handling middleware that can be used to catch errors in the application.

```js
Copy
app.use((err, req, res, next) => {
    console.error(err);
    res.status(500).send('Something went wrong');
});
```
## What is the next function in Express?

next is a function that passes control to the next middleware function in the stack. If there are no other middleware, it will end the request-response cycle.

## How do you serve static files in Express?

You can use express.static() to serve static files (like images, CSS, or JavaScript files).

```js
Copy
app.use(express.static('public'));
```
## What is a route in Express?

A route is a URL pattern that is mapped to a handler function. Express routes are defined using HTTP methods (.get(), .post(), .put(), .delete()).

## What is the difference between app.get() and app.post()?

app.get() is used to define routes that handle HTTP GET requests, while app.post() is used to handle HTTP POST requests.

## What is the res.send() method in Express?

res.send() is used to send a response to the client. It can send text, HTML, JSON, or other data.

## How do you handle form submissions in Express?

You can handle form submissions by using middleware to parse application/x-www-form-urlencoded data. Express provides express.urlencoded() to handle this.

```js
Copy
app.use(express.urlencoded({ extended: true }));
```
## What is the app.listen() method in Express?

app.listen() binds and listens for connections on a specified port.

## What is the purpose of the res.status() method in Express?

res.status() sets the HTTP status code for the response. For example, res.status(404) sets a 404 Not Found status.

## What is an HTTP request in Express?

An HTTP request is an object that represents the client's request to the server. It contains data like query parameters, body, headers, etc.

## What is an HTTP response in Express?

An HTTP response is an object that represents the server's response to the client. You can send data back to the client using res.send(), res.json(), etc.

## How do you use template engines in Express?

Express supports template engines like EJS, Pug, and Handlebars. You need to set the view engine using app.set('view engine', 'ejs'), for example.

## What is express.Router()?

express.Router() is a method that creates modular, mountable route handlers. You can use it to define routes in separate files or components.
## What is express.Router()?

express.Router() is a method that creates modular, mountable route handlers. You can use it to define routes in separate files or components.
