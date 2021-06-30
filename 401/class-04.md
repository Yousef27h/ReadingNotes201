# OOP

## Objects

Software objects are conceptually similar to real-world objects: they too consist of state and related behavior. 

Real-world objects share two characteristics: They all have state and behavior. Dogs have state (name, color, breed, hungry) and behavior (barking, fetching, wagging tail). Bicycles also have state (current gear, current pedal cadence, current speed) and behavior (changing gear, changing pedal cadence, applying brakes).

An object stores its state in fields and exposes its behavior through methods .

 Methods operate on an object's internal state and serve as the primary mechanism for object-to-object communication. Hiding internal state and requiring all interaction to be performed through an object's methods is known as _data encapsulation_.

 benefits of using objects in programming:

 1- Modularity
 
  The source code for an object can be written and maintained independently of the source code for other objects. Once created, an object can be easily passed around inside the system.

 2- Information-hiding
 
  By interacting only with an object's methods, the details of its internal implementation remain hidden from the outside world.

 3- Code re-use

 If an object already exists (perhaps written by another software developer), we can use that object in our program.

 4- Pluggability and debugging ease

 If a particular object turns out to be problematic, you can simply remove it from your application and plug in a different object as its replacement.

 ## Class

 A _class_ is the blueprint from which individual objects are created. And In object-oriented terms we say for example that a bicycle is an *instance of the class of objects* known as bicycles.


The following Bicycle class is one possible implementation of a bicycle:

``` 
class Bicycle {

    int cadence = 0;
    int speed = 0;
    int gear = 1;

    void changeCadence(int newValue) {
         cadence = newValue;
    }

    void changeGear(int newValue) {
         gear = newValue;
    }

    void speedUp(int increment) {
         speed = speed + increment;   
    }

    void applyBrakes(int decrement) {
         speed = speed - decrement;
    }

    void printStates() {
         System.out.println("cadence:" +
             cadence + " speed:" + 
             speed + " gear:" + gear);
    }
}
```

The fields _cadence_, _speed_, and _gear_ represent the __object's state__, and __the methods__ (_changeCadence_, _changeGear_, _speedUp_ etc.) define its interaction with the outside world.

Bicycle class is just the blueprint for bicycles that might be used in an application. The responsibility of creating and using new Bicycle objects belongs to some other class in your application.

Here's a BicycleDemo class that creates two separate Bicycle objects and invokes their methods:

```
class BicycleDemo {
    public static void main(String[] args) {

        // Create two different 
        // Bicycle objects
        Bicycle bike1 = new Bicycle();
        Bicycle bike2 = new Bicycle();

        // Invoke methods on 
        // those objects
        bike1.changeCadence(50);
        bike1.speedUp(10);
        bike1.changeGear(2);
        bike1.printStates();

        bike2.changeCadence(50);
        bike2.speedUp(10);
        bike2.changeGear(2);
        bike2.changeCadence(40);
        bike2.speedUp(10);
        bike2.changeGear(3);
        bike2.printStates();
    }
}
```



## Binary, Decimal and Hexadecimal Numbers

### Decimals

Every digit in a decimal number has a "position", and the decimal point helps us to know which position is which.

The position just to the left of the point is the "Ones" position. Every position further to the left is 10 times bigger, and every position further to the right is 10 times smaller.

The Decimal Number System is also called "Base 10", because it is based on the number 10. So you start counting at 0, then 1, until you reach number 9 then you run out of digits ... so you start back at 0 again, but increase the number on the left by 1.


### Binary Numbers

Binary Numbers are just "Base 2" instead of "Base 10". So you start counting at 0, then 1, then you run out of digits ... so you start back at 0 again, but increase the number on the left by 1.

### Hexadecimal Numbers

They look the same as the decimal numbers up to 9, but then there are the letters ("A',"B","C","D","E","F") in place of the decimal numbers 10 to 15.


So the general rule is : Count up until just before the "Base Number", then start at 0 again, but first you add 1 to the number on your left.
