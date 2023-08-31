

Create index.js in your directory:

     touch index.js

 Set up a new or existing npm package:

     npm init -y

Install express package:

    npm i express

index.js:

    import express from "express";
    
    const app = express();
    const port=3000;
    app.listen(port,()=>{
        console.log(`Server running on port ${port}.`);
    })

Run:

    node index.js

Output:

    Server running on port 3000.
