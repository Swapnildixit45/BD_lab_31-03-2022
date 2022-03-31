mongo
> show dbs
> use swapnil
> db.collection.insertOne({ firstName: 'swapnil', lastName: 'dixit'  })
> db
> db.collection.find()

> db.collection.insertMany([
... {
... firstName: 'vansh', lastName: 'sharma'
... },
... {
... firstName: 'ayush', lastname: 'yadav'
... }
... ])

> db.collection.find()
> db.collection.find({ "firstName":"ayush" })

> db.collection.updateOne({
... firstName:"ayush"},
... {
... $set:
... {
... lastname: "kumar"}
... })

> db.collection.update({}, {$unset: {lastName:1}},false,true}

> db.collection.deleteMany(
... {
... lastname : "kumar"})
