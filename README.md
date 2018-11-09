# platzi_mongodb

## Text search 
```js

 db.getCollection('users').createIndex({name: "text"})
 db.getCollection('users').find({$text: {$search: "de"}})
 db.getCollection('users').find({$text: {$search: "de", $caseSensitive: true}})

```
