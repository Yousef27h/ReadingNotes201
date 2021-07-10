# Inheritance and Interfaces

An object stores its state in _fields_ and exposes its behavior through _methods_.

A class is a blueprint from which objects are created.

## Inheritance

Inheritance is an important pillar of OOP(Object-Oriented Programming). It is the mechanism in java by which one class is allowed to inherit the features(fields and methods) of another class.

Inheritance is a class (superclass) that is derived from another class (subclass). Every class in java is emplicitly inherited from _Object_ class.

We use the keyword _extends_ follow by the name of superclass we want to inherit from.


## Interface

Methods are the interface of class with the outside world. 

An interface is like a contract used to group related methods with empty bodies.

We can define new interface just like creating classes but with using `interface` keyword.

methods inside interface doesn't have curly braces, and are ended up with a semicolon.

To access the interface methods, the interface must be `implemented` (kinda like inherited) by another class with the implements keyword (instead of `extends`).

Unlike classes, an interface can extend any number of interfaces.

