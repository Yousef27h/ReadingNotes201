# Room

Room is a library that persists data and provides an abstraction layer over SQLite to allow access to database while using full capabilities of SQLite.


Primary components in Room :

- The database class that holds the database, where data will be persisted.

- Data entities which they are the tables in database.

- Data access objects (DAO), the methods we use to query, update, insert, and delete data in databse.


The DAOs are provided by the database class. The app can use DAOs to retrieve data from the database as instance of data entity object. 

The objects inside databse are represented by entities that we define. Each entity corresponds to a table in database, and each object instance of that entity represents a row of data in the corresponding table.

We define each entity as a class with `@Entity` annotation, which include fields for each column in our table in database, and one or more fields that comprise the primary key defined with `@PrimaryKey` annotation or if we want to define a composite primary key we can do that by listing those columns in the `primaryKey` property of `@Entity`.

If we want to ignore columns, we can annotate them using `@Ignore`.

If we'd like to express an entity or data object as a cohesive whole in our database logic, we can use `@Embedded` annotation to represent an object into its subfields within a table.


we define relationships between entities by adding a reference to the primary key of one entity in the other, then we create a new entity which contains the fields combined with fields under `@Relation` annotation to define parent and entity columns.



