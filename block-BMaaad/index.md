writeCode

Write command to

- List collections from a database.

- show dbs

- create a new collection in your country database which you created recently.

- db.createCollection('City');

Write code to:-

- crate a database named `weather`

- use weather

- create a capped collection named `temperature` with maximum of 3 documents and try inserting more than 3 to see the result.

- db.createCollection("temperature", {capped : true, size : 1024, max : 3});

- db.temperature.insertMany([{'Delhi' : 44}, {'Mumbai' : 37}, {'Lucknow' : 42}]);

- db.temperature.find();

- db.temperature.insert({'Bangalore' : 30});

- create a simple collection named `humidity`

- db.createCollection('Humidity');

- check whether `temperature` collection is capped or not ?

- db.temperature.isCapped();

- Delete `humidity` collection and then the entire database(weather).

- db.Humidity.drop();
