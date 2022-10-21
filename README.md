# Puppies API with Typescript and Express
The aim of this project was to create a RESTAPI with Express and to get more familiar with Typescript in Node.js. The application supports the CRUD operations and is strongly types with TypeScript. 

### **Database** 
The database for this task is a simple in-memory store represented as a puppies object provided by the puppies.service module.
The puppies object implements the puppies.interface.

### **Puppy data model**
The puppy object implements the puppy.interface and has the following properties:
* id: (number)
* name: (string)
* breed: (string)
* description: (string)
* image: (string)

### **Endpoints**
- GET: `api/puppies`
- GET: `api/puppies/:id`
- POST: `api/puppies`
- PUT: `api/puppies/:id`
- DELETE: `api/puppies/:id`

