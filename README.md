# NOTES

## Extensions:
- Docker (by Microsoft)
- ESLint (by Microsoft)
- Prettier – Code formatter (by Prettier)
- MongoDB for VS Code (by MongoDB)

## Run Front End:
npm run dev

## Creating a Docker Container:
docker run -i -t ubuntu:24.04 /bin/bash

## Setting up MongoDB in Docker:
docker run -d --name dbserver -p 27017:27017 --restart unlessstopped mongo:6.0.4

## Adding Info to Mongo DB:
```
Right Click on Container and Attach Shell
mongosh mongodb://localhost:27017/mydb
db.users.insertOne({ username: 'dan', fullName: 'Daniel Bugl', age: 26 })
db.users.insertMany([ { username: 'jane', fullName: 'Jane Doe', age: 32 }, { username: 'john', fullName: 'John Doe', age: 30 } ])
##db.users.findOne({ username: 'jane' }##
```

## Run Back End Server:
node backend/backend_server.js