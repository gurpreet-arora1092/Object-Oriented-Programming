## Inheritance

Inheritance in programming is  a core concept of object-oriented programming (OOP) where one class (the child class or subclass) automatically inherits properties and methods from another class (the parent class or superclass). This allows for code reuse and establishes relationships between classes, promoting a hierarchical structure

Key aspects of inheritance:

-   **Code Reusability:**
    Child classes inherit the features (attributes and methods) of their parent, avoiding redundant code
**Hierarchical Relationships:**
   Inheritance creates a "is-a" relationship, where a child class is a specialized type of its parent. For example, a  `Dog`  is a type of  `Animal`

**Extensibility:**
Child classes can add new features (attributes and methods) to the inherited ones, building upon the functionality of the parent class

**Overriding:**
Child classes can redefine or override specific methods inherited from the parent, providing specialized behavior.


**Types of Inheritance:**

-   **Single Inheritance:** A class inherits from only one parent class.
-   **Multiple Inheritance:** A class inherits from multiple parent classes (though not supported by all languages).
-   **Multilevel Inheritance:** A class inherits from a class that itself inherits from another class, creating a hierarchy of inheritance

 **Benefits:**
    -   Simplifies code maintenance by centralizing common functionality in the base class.
    -   Promotes code organization and modularity.
    -   Facilitates code reuse, reducing development effort.
    -   Enables creation of class hierarchies that represent real-world relationships.

**
**Note :** Whenever Child Object is Created It's parent default constructer is also called.
It's not create a parent object  constructor is also responsible to initialise . The properties which are inheriting from parent  its should be initialise.