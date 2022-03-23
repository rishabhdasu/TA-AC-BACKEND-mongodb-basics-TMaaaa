writeCode

Write code to:-

- create a database named `sports`.

- use sports

- list all databases present in local mongod server.

- show dbs

- create 3 collections named `cricket`, `football`, `TT` in sports databse.

- db.createCollection('Cricket');
- db.createCollection('Football');
- db.createCollection('TT');

- add multiple players in those collections which should have fields like `name`, `age` and `email` and `bid_price`.

- db.Cricket.insertMany(players);
- db.Football.insertMany(players);
- db.TT.insertMany(players);

- list all collections in sports database.

- show collections

- rename `TT` collection to `tennis`.

- db.TT.renameCollection('Tennis');

- create a capped collection called `khokho` which should have max 3 documents.
  Try inserting more than 3 and see what happens?

  - db.createCollection('Khokho', {capped : true, size : 1024, max : 3});

  - db.Khokho.insertMany(players);

- check whether a collection is capped or not?

- db.Khokho.isCapped();

- drop all documents from `football` collection.

- db.Football.remove({});

- delete cricket collection completely.

- db.Cricket.drop();

- delete sports database.

- db.dropDatabase();

- check which database you are connected to ?

- db

- connect to test database

- use test
