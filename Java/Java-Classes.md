# OOPS

- OOP in java stands for Object oriented programming.

Procedural programming is about writing procedures or methods that perform operations on the data, while object-oriented programming is about creating objects that contain both data and methods.

A class is a template for objects, and an object is an instance of a class.

When the individual objects are created, they inherit all the variables and methods from the class.

#### Creating a Class: 
we can create a class using the keyword class.

```Java
class Main
{
  int x=5;
}
```
#### Creating an Object:
We can create objects for that class using the class name.

``` Java
public class Main
{
  public static void main(String[] args)
  {
    Main myobj=new Main();
  }
}
```
- We can create as many objects as we want to the class.

#### Attributes:
 Attributes are nothing but variables declared in the class.

 ``` Java
class One
{
  int s=8;
}
```
#### Accessing attributes
We can access the attributes using objects of the class.

```Java
class Sample
{
  int s=5;
}
class Main
{
  public static void main(String[] args)
  {
    Sample obj=new Sample;
    System.out.println(obj.x);
  }
}
```
Not only accessing the attributes,we can also modify them.If you don't want anyone to change your attribute values' you can simply declare them final.
We can also access a same variable using multiple objects in a class.

#### Methods in Java
Methods are used to perform certain actions when they are called.
``` Java
public class Main
{
  static void speak()
  {
    System.out.println("This is my first method in java");
  }
  public static void main(String[] args)
  {
    speak();
  }
}
```

#### Public Vs Static methods
* Public: Methods which are declared as public can be called by using an object.
* Static: Methods which are declared as static can be called without using an object,they can simply be called.
  
``` Java
public class Sample
{
  static void first()
  {
    System.out.println("This is a static method");
  }
  public void second()
  {
    System.out.println("This is a public method");
  }
}
public class Main
{
  public static void main(String[] args)
  {
    Sample obj=new Sample();
    obj.second();
    first();
  }
}
```
