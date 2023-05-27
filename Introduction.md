# Introduction 

#### Why JAVA and not C++?
- C++ is platform dependent. The excutable file of C++ might run on one platform and not on another
- Java solves this problem. It generates a JavaByte Code that can be run on any machine through JVM.
- This concept was used later on by Python and C#. 
- Java provides monitoring facilities as well
- No pointers in JAVA so more secure. 
- It is statically typed language

To run JAVA codes we need a JDK. 
- JDK (Java Development Kit) = JRE (Java Runtime Environment) + Dev Tools 
- JRE = JVM (Java Virtual Machine) + Java class library 
- JRE can be implemented in 2 ways: 
  - Just in time compilation: Compiles bytecode into native machine code at run time.
  - Interpreters : Not preffered usually 

- Camel case for variable is standard in Java
- upper case for constant is standard in Java

### Primitive DataTypes

- __byte__ : -128 to 127
- __bool__
- __int__
- __long__
- __float__
- __char__
- For floating points number use `12.0f`
- For Double use `12.0d`

### Non-Primitive DataTypes

These are usually classes that are defined by the users or predefined classes in Java.

```java
class Point{
    int x; 
    int y;
}

class Test{
  public static void main(String [] args){
      Point P = new Point();
      P.x = 10 # accessing x on P
      P.y = 20 # accessing y on P
  }
}
```

### Primitive v/s Non Primitive Datatype

- Non-Primitive datatypes variables are always references. Primitive datatypes create new memory spaces. 
- Memory for Non-primitive datatypes are always allocated on Heap. Primitive datatypes are allocated in stack.
- Members of Non-primitive variables have some default values (int = 0, bool = false, float = 0.0). Not in primitive type and we get **compilation error**.

> Heap memory is used to allocated dynamic memory. 

```java
# Driver code
    Point P1 = new Point();
    P1.x = 10; P2.y = 20;
    Point P2 = P1;
    P2.x = 30 # this changes the value of P1 as well because it is reference 
```


