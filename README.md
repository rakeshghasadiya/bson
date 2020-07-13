bson
=========
[![Build Status](https://travis-ci.org/mongo-dart/bson.svg?branch=master)](https://travis-ci.org/mongo-dart/bson)

Bson library for Dart programming language


```
 var listData = json.decode(jsonData) as List;

    //List to Bson
    var bsonBinary = BSON().serialize(listData);
    var haxString = bsonBinary.hexString;

    //Bson to List
    var bsonBinary = BsonBinary.fromHexString(haxString);
    bsonBinary.makeByteList();
    bsonBinary.rewind();
    var data = (BSON().deserialize(bsonBinary) as Map).values.toList()
```
