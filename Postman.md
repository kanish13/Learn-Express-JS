Postman enables you to create and send API requests. Send a request to an endpoint, retrieve data from a data source, or test an API's functionality. You don't need to enter commands in a terminal or write any code.

Download: https://www.postman.com/downloads/

![Screenshot 2023-09-01 134202](https://github.com/kanish13/Learn-Express-JS/assets/111358462/cd048f09-965f-4246-adc3-03c7b3c78138)

Exercise: 
    import express from "express";
    const app = express();
    const port = 3000;
    
    // *********************
    // Let’s practice using Postman. Make sure your server is running with nodemon.
    // Then test the 5 different routes below with Postman. Open a separate tab for each request.
    // Check that for each route you’re getting the correct status code returned to you from your server.
    // You should not get any 404s or 500 status codes.
    // *********************
    
    app.get("/", (req, res) => {
      res.send("<h1>Home Page</h1>");
    });
    
    app.post("/register", (req, res) => {
      //Do something with the data
      res.sendStatus(201);
    });
    
    app.put("/user/angela", (req, res) => {
      res.sendStatus(200);
    });
    
    app.patch("/user/angela", (req, res) => {
      res.sendStatus(200);
    });
    
    app.delete("/user/angela", (req, res) => {
      //Deleting
      res.sendStatus(200);
    });
    
    app.listen(port, () => {
      console.log(`Server started on port ${port}`);
    });

Sample Output:
![image](https://github.com/kanish13/Learn-Express-JS/assets/111358462/f41b243b-2745-4a83-a2c2-3e347065371c)


    
