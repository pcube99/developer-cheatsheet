### MongoDB shell commands
### 1) Show available databases
```
show dbs
```
### 2) create new database
```
use "database_name"
```
### 3) create new collection
```
db.collection_name.insertOne({ name: "hello world" })
```
### 4) show all data within collection
```
db.collection_name.find()
```
### 5) show all data within collection (pretty format)
```
db.collection_name.find().pretty()
```
### 6) Create
#### inserts one json object
```
insertOne(data, options)
```
#### inserts many json object

```
insertMany(data, options)
```
### 7) Read
#### finds all entries with given filter
```
find(filter, options)
```
#### finds first matched entry with given filter
```
findOne(filter, options)
```
#### greater than filter
```
db.flightData.find({distance: {$gt: 10000}}).pretty()
```

### 7) Update
#### update first matched entry
```
updateOne(filter, data, options)
```
#### update all matched entry
```
updateMany(filter,data, options)
```
#### replace one document entirely
```
replaceOne(filter,data, options)
```
#### updates distance field if not present then appends distance field
```
db.flightData.updateOne({distance: 950},{ $set: {distance: 1200}})
```
#### overwrites the whole document
```
db.flightData.update({distance: 950}, {distance: 1200})
```
### 8) Delete
#### delete first matched entry
```
deleteOne(filter, data, options)
```
#### delete all matched entry
```
deleteMany(filter,data, options)
```
```
db.flightData.deleteOne({distance: 950})
```
### 8) forEach function to iterate collection
```
db.passengers.find().forEach((passenger) => { printjson(passenger)})
```
### 9) toArray() function to display all documents at once
```
db.passengers.find().toArray()
```
### 10) projection to filter the data
#### this includes \_id as default
```
db.passengers.find({}, {name: 1}).pretty()
```
#### to exclude \_id from projection
```
db.passengers.find({}, {name: 1, _id: 0}).pretty()
```


