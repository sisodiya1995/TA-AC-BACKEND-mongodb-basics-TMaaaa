writeCode

Write code to:-

- create a database named `sports`.
// use sports

- list all databases present in local mongod server.
// show dbs

- create 3 collections named `cricket`, `football`, `TT` in sports databse.

// db.createCollection('cricket')
// db.createCollection('football')
// db.createCollection('TT')

- add multiple players in those collections which should have fields like `name`, `age` and `email` and `bid_price`.
  db.createCollection('players')
  db.players.insertMany([{name :"akash" ,age : 25 ,email : "akash@gmail" ,bid_price : 34} , {name :"akash" ,age : 25 ,email : "akash@gmail" ,bid_price : 34}, {name :"akash" ,age : 25 ,email : "akash@gmail" ,bid_price : 34}])

- list all collections in sports database.
// show collections

- rename `TT` collection to `tennis`.

- create a capped collection called `khokho` which should have max 3 documents.

//db.createCollection('khokho', {caped : true ,size : 1024 , max : 3})

  Try inserting more than 3 and see what happens?
- check whether a collection is capped or not?
// db.football.isCapped() //false
// db.cricket.isCapped() // false
// db.players.isCapped()  // false

- drop all documents from `football` collection.
- delete cricket collection completely.
// db.cricket.drop()
- delete sports database.

- check which database you are connected to ?
- connect to test database
