# README

- Best practice for learning in classroom is with peer instruction


## Week One

- Defining Classes and Creating Objects
  - 1. Class a new type of data, a template
  - 2. member variables, this
    >1. Make the member variable to be private
  - 3. overloading method
  - public vs private
    >1. public can be accessed anywhere
    >2. private can be only accessed within the class defined with nowhere else.
    >3. getters and setters(add some precautions in setters)
    >4. **Accessing private properties causes compiler time error.**

Method signature means the method name and parameters. Overloading the method return types is not allowed in java.(At compile time, Java C, the compiler, has to decide which version of the overloaded method you're actually trying to call.)

```java
public class SimpleLocation {
  private double latitude;
  private double longitude;
  
  public SimpleLocation(double latitude, double longitude){
    this.latitude = latitude;
    this.longitude = longitude;
  }

  // overload
  public SimpleLocation() {
    this.latitude = 0;
    this.longitude = 0;
  }
}
```
  

## Week Two

 
- [memory model reasoning](https://www.coursera.org/learn/object-oriented-java/lecture/gOFlb/core-drawing-memory-models-with-objects)
  - Memory model for primitive type
  - Memory model for object type

- [scope](https://www.coursera.org/learn/object-oriented-java/lecture/mqFZ3/core-introduction-to-scope)
  - local variable(inside method)
  - parameters(behave like local variables)
  - member varibales 

With a scope being destroyed, all variables defined in that scope disappear.

- keyword **this** is not strictly required in constructor and methods. You can omit it, and java will work just fine.

- JDK and JRE

  >1. JDK (Java development Kit) is the binary file that contains the toolkit for developing application in Java.
  >2. JRE(Java runtime enviroment) is a software that makes it available for uses to run JAVA application using a combination of Java code and libraries from the JDK.
  