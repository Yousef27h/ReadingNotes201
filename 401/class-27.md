# Amplify Connection

Serverless is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers.

The Philosophy of servless is to focus on business and application and not care about infrastructure.
it will save a lot of time, effort, implementing things; so the point is i focus on business and UI and they provide me backend and infrastructure.
it’s provided by companies like Amazon and Google. it’s very beneficial since developers no longer have to work with infrastructure e.g. implementing, debugging.

The `@connection` enables you to specify relationships between model types.

The `@connection` directive supports one-to-one, one-to-many, and many-to-one relationships.

To implement a many-to-many relationships we may use two one-to-many connections.

Relationships between types are declared using `@connection` annotating fields on `@model` object type.

The limit number of nested objects is 100. but you can override it by setting the limit argument.

