# SHOPPING CART REST API

Have setup instance of Mongodb server connected with Python Flask Framework

Mongo Setup
Install MongoDb Community Server Edition (stable release)
Once you have set the right PATH for mongodb in the environment variables.

Do check if its properly installed and then Activate Mongodb Instance using below steps:
1. Open Command Prompt and Run 'mongod'
2. In another terminal run 'mongo'
3. Start with Collection and Database creation process mentioned below:
    > use Ecommercecart                                                                 
    > db.createUser({user:'raza', pwd:'execute', roles:['readWrite', 'dbAdmin']})
    > db.createCollection('cartItems')
4. Install following packages like flask and pymongo using pip install 
5. Once the code is executed using python app.py, run the following request methods to Postman: [GET, POST, PUSH, DELETE]. Please do check below object for a sample JSON object as reuqest to server:
Sample Request :
  {
            
            "name": "DDD",
            "description":"ZZZ",
            "quantity":"b",
            "price":"c"

}


Step 6 (Request & Types) -

    POST http://localhost:5000/item (Create Item)
    
    GET http://localhost:5000/item (Read All Items)
    
    GET http://localhost:5000/item/{:id} (Read Specific Item)
    
    PUT http://localhost:5000/item/{:id} (Update Specific Item)
    
    DELETE http://localhost:5000/item/{:id} (Delete Specific Item)
    
    Check Outputs folder for the results of the projects
