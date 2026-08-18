- Expressis a lightweight web framework for **Node.js** that helps to build backend applications and APIs more easily.
- Creating an Express Server:
	1. Create a directory
	2. Create a index.js file
	3. Initialize NPM
	4. Install the Express package
	5. Write server application in index.js
	6. Start server
- **What is a Localhost?**
	- it is simply when we don't have a server on the internet and host our server locally making our own computer our server.
- **What is HTTP?**
	- HTTP(Hyper Text Transfer Protocol) is a set of rule or a language that allows computer(client) to talk to each other across the internet(server). 
	- Type of requests(Routes):
		1. Get: This is when we want to request a resource from the server.
		2. Post: It's when sending a resource to the server.
		3. Put: It's when replacing a resource with whatever is sent.<- it change the whole thing
		4. Patch: It's when patching up a resource. <- it only change the place that need fix.
		5. Delete:It's when deleting a resource from the server.
## body-parser
- Node.js body parsing middleware.
- Parse incoming request bodies in a middleware before your handlers, available under the `req.body` property.

## Morgan 
- HTTP request logger middleware for node.js.
		import morgan from "morgan";
		app.use(morgan("combined"));
- 