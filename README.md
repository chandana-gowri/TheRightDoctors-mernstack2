This project is a Node.js RESTful web service that uses Express.js and MongoDB Atlas to store and manage person details in the cloud.
The application starts execution using the command node server.js, where the database connection is established using mongoose.connect() with a MongoDB Atlas connection string.
Person data is stored using a Mongoose schema defined as new mongoose.Schema({ name, age, gender, mobile }).
The REST APIs are implemented using app.get('/person') to retrieve all records, app.post('/person') to insert new data, app.put('/person/:id') to update existing records, and app.delete('/person/:id') to remove a person from the database.
Dependencies are installed using npm install express mongoose, and the server runs on http://localhost:3000/person, where all API responses are returned in JSON format.
