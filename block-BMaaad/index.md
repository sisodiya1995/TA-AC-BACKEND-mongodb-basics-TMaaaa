writeCode

Write command to

- List collections from a database.
// show collection
- create a new collection in your country database which you created recently.
   // db.createCollection('delhi')

Write code to:-

- crate a database named `weather`
// use weather
- create a capped collection named `temperature` with maximum of 3 documents and try inserting more than 3 to see the result.
//db.createCollection('temperature', {caped : true ,size : 1024 , max : 3})

  db.temperature.insertMany([{'name' :'akash'} , {'name' :'aakash'}, {'name' :'akasha'},{'name' :'akashaa'}])
- create a simple collection named `humidity`

//db.createCollection('humidity')
- check whether `temperature` collection is capped or not ?

//db.temperature.isCapped() // true
// db.humidity.isCapped() // false
- Delete `humidity` collection and then the entire database(weather).

//db.humidity.drop() // true
 // db.dropDatabase()
