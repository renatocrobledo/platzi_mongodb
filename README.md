# platzi_mongodb: CRUD

[Manual MongoDb crud](https://docs.mongodb.com/manual/crud/)

## Users
```js
db.getCollection("users").insert([
  { _id: "1", name: "Renato Cacho", rides: 10  },
  { _id: "2", name: "Fulano de Tal", rides: 20 },
  { _id: "3", name: "Perengano Glez", rides: 19 },
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

## Cars
```js
db.getCollection('cars').insert([
  { _id: "1", driverUser: "6", 
    location: {
      type: "Point",
      coordinates: [-74.088068, 4.683302]
    }
  },
  { _id: "2", driverUser: "5", 
    location: {
      type: "Point",
      coordinates: [-74.128745, 4.650886]
    }
  },
  { _id: "3", driverUser: "4", 
    location: {
      type: "Point",
      coordinates: [-74.064179, 4.681856]
    }
  },
  { _id: "4", driverUser: "3", 
    location: {
      type: "Point",
      coordinates: [-74.073695, 4.681856]
    }
  },
  { _id: "5", driverUser: "2", 
    location: {
      type: "Point",
      coordinates: [-74.128745, 4.695666]
    }
  },
  { _id: "6", driverUser: "1", 
    location: {
      type: "Point",
      coordinates: [-74.088068, 4.683302]
    }
  }
])
```

## Sessions
```js
db.getCollection('sessions').insert([
  {user:"1", date: new Date("2018-11-09")},
  {user:"2", date: new Date("2018-11-08")},
  {user:"3", date: new Date("2018-11-07")},
  {user:"4", date: new Date("2018-11-06")},
  {user:"5", date: new Date("2018-11-05")},
  {user:"6", date: new Date("2018-11-04")},
  {user:"7", date: new Date("2018-11-03")},
  {user:"8", date: new Date("2018-11-02")},
  {user:"9", date: new Date("2018-11-01")},
  {user:"10", date: new Date("2018-11-01")},
  {user:"11", date: new Date("2018-11-01")}
]) 
```

## Rides
```js
db.getCollection('rides').insert([
  { 
    user: "7", car: "2", 
    startLocation: {
      type: "Point",
      coordinates: [-74.088068, 4.683302]
    }, 
    endLocation: {
      type: "Point",
      coordinates: [-74.128745, 4.650886]
    }
  },
  { 
    user: "8", car: "1", 
    startLocation: {
      type: "Point",
      coordinates: [-74.088068, 4.683302]
    }, 
    endLocation: {
      type: "Point",
      coordinates: [-74.128745, 4.650886]
    }
  },
  { 
    user: "9", car: "3", 
    startLocation: {
      type: "Point",
      coordinates: [-74.088068, 4.683302]
    }, 
    endLocation: {
      type: "Point",
      coordinates: [-74.128745, 4.650886]
    }
  },
  { 
    user: "9", car: "4", 
    startLocation: {
      type: "Point",
      coordinates: [-74.088068, 4.683302]
    }, 
    endLocation: {
      type: "Point",
      coordinates: [-74.073695, 4.681856]
    }
  },
  { 
    user: "9", car: "3", 
    startLocation: {
      type: "Point",
      coordinates: [-74.088068, 4.683302]
    }, 
    endLocation: {
      type: "Point",
      coordinates: [-74.128745, 4.650886]
    }
  },
  { 
    user: "9", car: "4", 
    startLocation: {
      type: "Point",
      coordinates: [-74.088068, 4.683302]
    }, 
    endLocation: {
      type: "Point",
      coordinates: [-74.073695, 4.681856]
    }
  }
])
```

