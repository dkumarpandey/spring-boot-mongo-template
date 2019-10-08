# spring-boot-mongo-template
MongoTemplate
##Note:

Need to create a user stocks for sandbox db as shown below uusing mongo shell console.

use sandbox
db.createUser(
  {
    user: "stocks",
    pwd: "password",
    roles: [ { role: "readWrite", db: "sandbox" } ]
  }
)


To test the example open browser
http://localhost:8080/stocks/

You should get the response similar to below.
{"stockId":0,"companyName":"Tesla","symbol":"TLSA","ceo":"Elon Musk","price":250.0}