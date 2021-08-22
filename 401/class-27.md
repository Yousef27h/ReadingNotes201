# Amplify Connection

The `@connection` enables you to specify relationships between model types.

The `@connection` directive supports one-to-one, one-to-many, and many-to-one relationships.

To implement a many-to-many relationships we may use two one-to-many connections.

Relationships between types are declared using `@connection` annotating fields on `@model` object type.

The limit number of nested objects is 100. but you can override it by setting the limit argument.

