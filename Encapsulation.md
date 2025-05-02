
## Encapsulation

**

Bundling of data (attributes) and Behaviour (methods / functions) that operate on  that data into a Single unit called a class.

It also involves restricting direct access to some of the Object's component for better control by using **Access Modifier**

Getter and setter methods provide controlled access to a class's internal state, hiding direct access to the properties themselves. This helps maintain data integrity and allows for internal implementation details to be changed without affecting external code

Access Modifier Helps us to control the access of our data and behaviour.

Public  :  public means access  anywhere #NoRestriction.

Private :  private means private to specific class where member is declared.

default : default means accessible within  a same Package #withinSamePackage.

Protected : protected accessible in derived class only.



Note : To access Private Data Member from outside class. Then getter and setter method helps to do that
 In Getter and Setter Method  Add Some checks and validation before changing  the data member directly..



**Getter and Setter** methods are fundamental in object-oriented programming, particularly when dealing with object properties or attributes. Getters allow you to access the value of a property, while setters enable you to modify it, often with validation or transformation applied during the process

Getter Methods:

-   **Purpose:** Retrieve the value of a property or attribute.
-   **Example (Java):** `public int getAge() { return age;` `}`

**A getter is always invoked with no arguments**, so defining it with any parameter is likely an error

**Read-Only Properties:**

You can choose to provide only getter methods, making a property read-only

Setter Methods:

-   **Purpose:** Modify the value of a property or attribute.
-   **Example (Java):** `public void setAge(int age) { this.age = age;` `}`

**Validation and Transformation:**

Setters can include logic to validate input or transform the value before assigning it to the attribute.
 **Convention:**

    In many languages (like Java and C#), getters typically start with "get" followed by the property name (e.g.,  `getName()`), while setters start with "set" followed by the property name (e.g.,  `setName(value)`).



In essence, getters and setters are a powerful mechanism for controlling access to and modification of object attributes, enhancing encapsulation, data integrity, and code flexibility.