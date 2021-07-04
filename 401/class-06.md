# Inheritance and Interfaces

An object stores its state in _fields_ and exposes its behavior through _methods_.

A class is a blueprint from which objects are created.

## Inheritance

Objet-oriented programming allows classes to inherit fields and methods from other classes. In Java each class is allowed to have one direct superclass.

We use the keyword _extends_ follow by the name of superclass we want to inherit from:

```
class  subClass  __extends__  superClass{

    // new fields and methods

}
```

## Interface

Methods are the interface of class with the outside world. 

An interface is like a contract and it is made up of a group of methods with empty bodies. To implement any interface, all methods must appear in its source code before compiling.

We can define new interface just like creating classes but with using _interface_ keyword.

methods inside interface doesn't have curly braces, and are ended up with a semicolon.

To use an interface, we use the keyword _implements_ after class name then the name of the interface.

```
public class className __implements__  interfaceName{

    // constants if there are
    // method signatures

}
```

Unlike classes, an interface can extend any number of interfaces.

