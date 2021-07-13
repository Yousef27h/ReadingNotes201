# Related Resources

There are three relationships that van be defined by the association resources that Spring Data REST exposes for a repository:

- One-to-One Relationship

Association resources mist have different names.
We can customize association name default by using `@RestResource`.

- One-to-Many Relationship

Defined using the `@OneToMany` and `@ManyToOne` annotations and can have the optional `@RestResource` annotation just like one-to-one relationship to customize the association resource.

- Many-to-Many Relationship

Defined using the `@ManyToMany` annotation and can have the optional `@RestResource` annotation just like one-to-one relationship to customize the association resource.

# Integration Testing in Spring

Integration tests plays an important role in the application development cycle to ensure that everything works as planned.

We can use _MockMvc_ for testing, which encapsulates all web application beans and makes them available for testing.

MockMvc is defined as a main entry point for server-side Spring MVC testing. Tests with MockMvc lie somewhere between between unit and integration tests. It provides an easy-to-use API to call web endpoints and to inspect and assert their response at the same time.

