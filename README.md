# platzi_mongodb

## Aggregation

```js

// Raliza la suma total de viajes
db.getCollection('users').aggregate([
    { $match: {}},
    { $group: {_id: "001", totalRides: { $sum: "$rides"}}}
])


// Redefine cada valor decimal en el campo "rides" como número entero
db.getCollection('users').find({}).forEach( function(doc){
  db.getCollection('users').update({_id:doc._id}, {$set: {rides: NumberInt(doc.rides)}})
})


```
