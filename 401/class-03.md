# Java Primitives versus Objects

Java has a two-fold type system:

- primitives such as int, boolean

- reference types such as Integer, Boolean

Every primitive type corresponds to a reference type.

The process of converting a primitive type to a reference one is called autoboxing, the opposite process is called __unboxing__.

## Pros and Cons

### Single Item Memory Footprint

Primitive type variables have the following impact on the memory:

- boolean
- byte
- short, char
- int, float
- long, double

Variables of these types live in the stack and hence are accessed fast.

While the reference types are objects, they live on the heap and are relatively slow to access.

- Boolean
- Byte
- Short, Character
- Integer, Float
- Long, Double

### Memory Footprint for Arrays

Despite the fact that Long and Double classes, arrays of primitive types long and double consume more memory.

### Performance

primitive types are faster than wrapper classes.


### Default Values


Default values of the primitive types are _0_ for numeric types, _false_ for the boolean type, _\u0000_ for the char type. For the wrapper classes, the default value is _null_.


# Exceptions 

An exception is an event, which occurs during the execution of a program, that disrupts the normal flow of the program's instructions.

When an error occurs within a method, a method throws an exception. if it doesn't find an appropriate exception handler after searching all methods, the runtime system terminates.

# Scanning 

Scanner used to read files, by breaking them down into tokens and translating them. By default scanner uses white spaces to separate tokens.
