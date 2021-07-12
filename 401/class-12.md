# Spring RESTful Routing & Static Files

## Spring RequestMapping

`@RequestMapping` is used to map web requests to sping controller methods.


The very basic mapping an HTTP request is by Path, and by the HTTP method.

we can add HTTP header attribute to the mapping, or even multiple headers.

Parts of the mapping URI can be variables using `@PathVariable` notation.

Also we can have multiple parts of the URI being mapped to multiple values using `@PathVariable`.

We can also use regular expressions when mapping the `@PathVairable`.

`@RequestMapping` also allows for mapping of URL parameters with the `@RequestParam` annotation. Multiple params values can be set, and not all of them have to be used.


## CrudRepository, JpaRepository, and PagingAndSortingRepository


- `CrudRepository` provides CRUD functions.

- `PagingAndSortingRepository` provides methods to do pagination and sort records.

- `JpaRepository` provides JPA related methods such as flushing the persistence context and delete records in a batch.


Because `JpaRepository` extends `PagingAndSortingRepository` and `CrudRepository`, it contains the full API of the two.


CRUD functionality: save, findOne, findAll, count, delete, exists.


JpaRepository functionality: findAll, save, flush, saveAndFlush, deleteInBatch. 