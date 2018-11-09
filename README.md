# platzi_mongodb

## Users
```js
db.getCollection("users").insert([
  { _id: "1", name: "Renato Cacho", rides: 10  },
  { _id: "2", name: "Fulano de Tal", rides: 20 },
  { _id: "3", name: "perengano Glez", rides: 19 },
  { _id: "4", name: "Rafaelo Gimenez" , rides: 25 },
  { _id: "5", name: "Angela Aguas", rides: 33 },
  { _id: "6", name: "Anastasia Mercado", rides: 5 },
  { _id: "7", name: "Clementina Ramirez", rides:  10},
  { _id: "8", name: "Anastasia Ruiz", rides: 0 },
  { _id: "9", name: "Arnulfa Guzman", rides: 0 },
  { _id: "10", name: "Godino Bea", rides: 0 },
  { _id: "11", name: "Diego De ceballos", rides: 0 }
])
```

```js
// Proyections
  db.getCollection('users').find({},{name: 1})

// Limit:
  db.getCollection('users').find({},{name: 1}).limit(5)

// Sort:
  db.getCollection('users').find({}).sort({name: 1})

```

