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
```
inserts one json object
insertOne(data, options)
```
```
inserts many json object
insertMany(data, options)
```
### 7) Read
```
finds all entries with given filter
find(filter, options)
```
```
finds first matched entry with given filter
findOne(filter, options)
```
### 7) Update
```
update first matched entry
updateOne(filter, data, options)
```
```
update all matched entry
updateMany(filter,data, options)
```
```
replace one document entirely
replaceOne(filter,data, options)
```
### 8) Delete
```
delete first matched entry
deleteOne(filter, data, options)
```
```
delete all matched entry
deleteMany(filter,data, options)
```
