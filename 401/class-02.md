# Packages and Import

Packages is folders where classes can be joined together.

The first statement, other than comments, in a Java source file, must be the package declaration. Following the optional package declaration, you can have import statements, which allow you to specify classes from other packages that can be referenced without qualifying them with their package.


The statement order is as follows: 

1- Package statment (optional).
2- Imports (optional).
3- Class or interface definitions.

```
package illustration;

import java.awt.*;

public class Drawing {
    . . .
}
```
There are three ways we can import classes from another packages:

1- When we use (*), which is called the wildcard character, we specify that all classes with that package are availabe to our program. By doing that the object file doesn't get larger, since it only tells the compiler where to look for symbols.

The wildcard "*" only makes the classes in this package visible, not any of the subpackages.

```j
import javax.swing.*;  // Make all classes visible altho only one is used.

class ImportTest {
    public static void main(String[] args) {
        JOptionPane.showMessageDialog(null, "Hi");
        System.exit(0);
    }
}
```

2- Classes can be specified explicitly on import instead of using the wildcard character.

```
import javax.swing.JOptionPane;  // Make a single class visible.

class ImportTest {
    public static void main(String[] args) {
        JOptionPane.showMessageDialog(null, "Hi");
        System.exit(0);
    }
}
```

3- We can put fully qualified class name without an import.

```
class ImportTest {
    public static void main(String[] args) {
        javax.swing.JOptionPane.showMessageDialog(null, "Hi");
        System.exit(0);
    }
}
```


# Loops

Looping in programming is the execution of block of code until the controlling condition evaluates to _false_.

Here are the types of loops that we can find in Java:
 
- Simple _for loop_
- Enhanced _for-each loop_
- _while_ loop
- _Do-While loop_

## _For_ loop

A *for* loop is a control structure that allows us to repeat a set of instructions depending on loop counter number.


## _While_ loop

It repeats a statement or a block of statements *while* its controlling *Boolean-expression* is true.

## _Do-While_ loop

Works just like while loop except it will execute at least one time before checking Boolean-expression and condition evaluation happens.