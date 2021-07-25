# Spring Authentication



Application security basically consists of two parts: Authentication (Who you are?) and Authorization (What are you allowed to do?).


Spring Security is a powerful and highly customizable authentication and access-control framework. It is the de-facto standard for securing Spring-based applications. 


Spring Security is the primary choice for implementing application-level security in Spring applications. Generally, its purpose is to offer you a highly customizable way of implementing authentication, authorization, and protection against common attacks

The main interface we use for authentication is `AuthenticationManager`, and spring boot provides a default `AuthenticationManager` with only one user unless we provide our own bean of the same type.


After authentication is successful, we move on to authorization, the main interface for it is `AccessDecisionManager`.


Spring Security is based on Servlet Filters. There are multiple layers of filters each playing a special role, even though its viewed by its container as one filter.

