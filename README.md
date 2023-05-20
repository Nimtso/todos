## Overview
Create a basic http server using NodeJs, Express and MongoDB. Here are some rules for the project. 
*  Code the tasks synchronous order
* Use the official mongoDB module (not mongoose)
* Use a local mongodb container to run an instance of mongodb

Good luck!

## Task Schema: 
	{
		id: String
		dueDate: Date - ISO Format
		description: String
		
	}

## GET/ health
Method: GET
Body: Task objedct
Params: None
Response: 'I am alive!'
Status Code: 200



## POST/ tasks
  - Method: GET
  - Body: task
  - Params: None
  - Response:  The created task
  - Status Code: 201



## GET/tasks
  - Method: GET
  - Body: None
  - Params: None
  - Response:  An array of all the tasks
  - Status Code: 200



## Middleware
Create your own middleware for logging data. Log the time, and the message in a format that you think is readable.



## GET/tasks/:id
  - Method: GET
  - Body: None
  - Params: id
  - Response:  The task with the id specified
  - Status Code: 200 on success. 404 If not found.



## DELETE/tasks/:id
  - Method: GET
  - Body: None
  - Params: None
  - Response:  The number of deleted Documents. 
  - Status Code: 200

## PATCH /tasks/description
  - Method: PATCH
  - Body: { id, description}
  - Params: None
  - Response: The upated document
  - Status: 200


## DELETE/tasks/
  - Method: GET
  - Body: None
  - Params: None
  - Response:  The number of deleted Documents. 
  - Status Code: 200

## Swagger
  - Add Swagger to the routes

##  Validation:
  - Schema validation for your route. Use the module joi

## Testing:
  - Create unit tests for the get routes in the order that you wrote them.
  - Use jest and supertest.
