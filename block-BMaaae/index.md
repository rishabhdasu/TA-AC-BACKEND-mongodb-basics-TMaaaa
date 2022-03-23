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

- db.Cricket.insertMany([{'name' : 'V Kholi', 'age' : 33, 'email' : 'kohli@gmail.com', 'Bid Price' : '18Cr'}, {'name' : 'R Sharma', 'age' : 34, 'email' : 'rsharma@gmail.com', 'BidPrice' : '15CR'}]);

- list all collections in sports database.

- show collections

- rename `TT` collection to `tennis`.

- db.TT.renameCollection('Tennis');

- create a capped collection called `khokho` which should have max 3 documents.
  Try inserting more than 3 and see what happens?

  - db.createCollection('Khokho', {capped : true, size : 1024, max : 3});

- check whether a collection is capped or not?

- db.Khokho.isCapped();

- drop all documents from `football` collection.

- db.Football.Collections.drop();

- delete cricket collection completely.
- delete sports database.

- check which database you are connected to ?

- connect to test database
