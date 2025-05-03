
## POLYMORPHISM


Poly morphism means  many forms
Someone who has many forms for example  A Man is a child , A Man is a Husband, A Man is a Father.

ParentClass reference can be used to store  reference of a child class object

Method Overloading (Compile Time Polymorphism)
In Simple words Inside a single class multiple behaviour are defined.

Method overloading in programming  allows a class to have multiple methods with the same name, but different parameters (number, type, or order). This is a form of polymorphism, enabling a single method name to be used for different functionalities based on the input arguments.

Key Concepts:

-   **Multiple Methods with the Same Name:**

    Overloaded methods share the same name, but they must differ in their parameter lists.

-   **Different Parameters:**

    The parameters can differ in number, type, or order.

-   **Compile-Time Polymorphism:**

    Method overloading is a compile-time polymorphism, meaning the compiler determines which method to call based on the arguments provided.

-   **Increased Readability and Flexibility:**

    Overloading can improve code readability and make it more flexible by allowing the same method name to be used for different tasks.


Note :  Return type of Method is not considered because Return type is not resolving in Compile time.
( A Man is a child , A Man is a Husband, A Man is a Father)

Method Overriding (Run Time Polymorphism)
In Simple in Multiple Classes Behaviours are defined
Method overriding in object-oriented programming is  a mechanism that allows a subclass to provide a specific implementation of a method that is already defined in its superclass. This means a subclass can refine or change the behavior of a method it inherits. It's a key part of polymorphism, enabling runtime behavior selection based on the object's actual type.


-   **Inheritance:**

    Method overriding works within a class hierarchy where a subclass inherits from a superclass.

-   **Method Signature:**

    The overriding method in the subclass must have the same name, same parameters (signature), and same or compatible return type as the method in the superclass.

**Runtime Behavior:**

When a method is called on an object, the actual method that gets executed is determined by the object's runtime type, not the type of the reference variable. This means if you have a parent class reference that holds an object of the subclass, calling the method will execute the subclass's version.


-   **Polymorphism:**

    Method overriding is a core aspect of polymorphism, which allows objects of different classes to be treated as objects of a common parent class.

-   **Code Reusability and Flexibility:**

    Method overriding enhances code reusability by allowing subclasses to build upon the behavior of their superclasses and also enhances flexibility by allowing subclasses to customize behavior.

class Animal {
  public void makeSound() {
    System.out.println("Generic animal sound");
  }
}

class Dog extends Animal {
  @Override
  public void makeSound() {
    System.out.println("Woof!");
  }
}

class Cat extends Animal {
  @Override
  public void makeSound() {
    System.out.println("Meow!");
  }
}

public class Main {
  public static void main(String[] args) {
    Animal animal = new Animal();
    Animal dog = new Dog();
    Animal cat = new Cat();

    animal.makeSound(); // Output: Generic animal sound
    dog.makeSound();     // Output: Woof!
    cat.makeSound();     // Output: Meow!
  }
}

In this example,  `Animal`  is the superclass, and  `Dog`  and  `Cat`  are subclasses. Both  `Dog`  and  `Cat`  override the  `makeSound()`  method, providing their own specific implementations. When the  `makeSound()`  method is called on a  `Dog`  object, the  `Dog`'s implementation is executed, and similarly for  `Cat`.



**
