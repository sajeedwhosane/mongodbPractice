## mongodb commands
#### create a database (or) use database
 `use db_name`
#### drop database
#### switch to the database you want to drop and then use the following command.
 `db.dropDatabase()` 
#### to show the databases present.
 `show dbs`;
#### create collection.
`db.createCollection(name,options)`

`eg: db.createCollection("users",{autoIndexId:true})`
#### dropping collection.
`db.collectionName.drop()`
### inserting records in the documents.
##### insert() method.
`db.collection_name.insert({document})`
`eg:  db.Users.insert({"Name":"Shaik Sajeed Hussain", email:"shaik.sajeed.16@gmail.com", gender:"M", age: 25, }, {"Name":"Salman Khan" })`
##### insertOne() method.
`db.COLLECTION_NAME.insertOne(document)`
`eg: db.Users.insertOne({ "Name":"Salman Khan", "email":"coolkhansalman@gmail.com", "gender":"M", "age":26})`
##### insertMany() method.
`db.COLLECTION_NAME.insertMany({document},{document},{document}})`
`eg db.Users.insertMany([]
    {
        Name:"Mohit Saraf",
        email:"mohitsaraf@gmail.com",
        gender:"Male",
        age:40
    },
    {
        Name:"Kangana Ranaut",
        email:"someemail@gmail.com",
        gender:"female",
        age: 25
    }
    ])`
