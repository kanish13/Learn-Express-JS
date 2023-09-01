HTTP:

* The Hypertext Transfer Protocol is an application layer protocol in the Internet protocol suite model for distributed, collaborative, hypermedia information systems.
  ![fetching_a_page](https://github.com/kanish13/Express-JS-/assets/111358462/85676215-7f11-489e-a09d-ba3f0e7cb298)


  ![Screenshot 2023-09-01 120900](https://github.com/kanish13/Express-JS-/assets/111358462/99d678ad-7250-4660-aa42-356c8ae7b271)


Basic Web Server with Routes:

      import express from "express";
      
      const app=express();
      const port=3000;
      app.get("/",(req,res)=>{
         res.send("<h1>kanish</h1>")
      })
      app.get("/about",(req,res)=>{
          res.send("<h1>About</h1>")
       })
       app.get("/contact",(req,res)=>{
          res.send("<h1>Contact</h1>")
       })
      app.listen(port,()=>{
          console.log(`Server running at port ${port}`)
      })
      

