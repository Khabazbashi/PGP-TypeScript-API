# Puppies API with Typescript and Express
The aim of this project was to create a REST API with Express and to get more familiar with Typescript in Node.js. The application supports CRUD operations. 

## **Database** 
The database for this task is a simple in-memory store represented as a puppies object provided by the puppies.service module.
The puppies object implements the puppies.interface.

## **Endpoints**
- GET: `api/puppies`
- GET: `api/puppies/:id`
- POST: `api/puppies`
- PUT: `api/puppies/:id`
- DELETE: `api/puppies/:id`

___

## **Try it out** 
1. Clone the repo
2. Install dependencies: `npm ci`
3. Create a .env file: `touch .env`
4. Populate the .env file: `PORT=7000`


### **Get a puppy**
```
curl http://localhost:7000/api/puppies/1
```

### **Get all puppies**
```
curl http://localhost:7000/api/puppies
```

### **Add a puppy**
```
curl -X POST -H 'Content-Type: application/json' -d '{
  "name": "Cookie",
  "breed": "Cocker spaniel",
  "description": "Cocker spaniels are known for being gentle, easy-going and affectionate yet lively.",
  "image": "https://media-be.chewy.com/wp-content/uploads/2021/05/05180433/Cocker-Spaniel_FeaturedImage.jpg"
}' http://localhost:7000/api/puppies
```

### **Delete a puppy**
```
curl -X DELETE http://localhost:7000/api/puppies/2
```
