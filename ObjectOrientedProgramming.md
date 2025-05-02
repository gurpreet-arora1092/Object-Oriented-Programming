**

# Object Oriented Programming

**
**

> It's a programming paradigm that organizes code into reusable units
> called objects and classes. In a simple sense, OOPS is a way of
> structuring programs using objects that interact with each other.

**


Let's Understand Class and Object

Class : A Class is just a Conceptual Design or a Container

Let's take an example of some entities of some institute
Institute can  made up of some entities like :-
Student
Instructor
Course
Batch
Assignments

An entity refers to **something that exists and can be identified as a distinct and independent unit**

Now think about Specific entity what information can be stored by entity

Entity Contain  Some data and behaviour / action
For Example  STUDENT

Some Data Attributes / Properties
studentId
studentName
studentRollNo
studentEmail

Some Behaviour /action like
attendClass
changeEmail
rateLecture
solveProblem

**We need something which can help is group all of this information (data and behaviour) together !**

Class is Blueprint of an entity  group data & behaviour together
Class is also knows as Custom dataType
Class is Just a Conceptual Design / A Blueprint

**Note** : We Cannot Store data or use the method just by creating a blueprint. Because it's Just a Blueprint and Blueprint can't exists in real .
For Example: A Map of House is not a real house, or design of a Vehicle is not a real vehicle.

**Code Example  :-**
class Student {

//  data attributes
int studentId;
string studentName;
string studentEmail;

/// behaviour / action
	void rateClass() {

	}

}


Objects :  Objects are the real world entity.

ClassName  variablename  = new ClassName();

new Keyword is here responsible to create a Object.

new ClassName() // this is a function call. this is a Special function/method is called Constructor  which is used to initialize an Object or responsible to create an Object  when it is created .
EveryProgramming language provide a default constructor  if and only if we don't create any consutructor.

Default Constructor is Public and same name as a class name
Constructor  never return a value.

Once Programmer create any constructor  Default constructor is not provided by programming language.

Now, variablename is a real entity called object that exists in memory.


**

## Principles / Pillars of Object Oriented Programming

**

 - Encapsulation
 - Inheritance
 - Polymorphism
 - Abstraction

**

## Encapsulation

**

Bundling of data (attributes) and Behaviour (methods / functions) that operate on  that data into a Single unit called a class.

It also involves restricting direct access to some of the Object's component for better control by using **Access Modifier**

Access Modifier Helps us to control the access of our data and behaviour.

Public  :  public means access  anywhere #NoRestriction.

Private :  private means private to specific class where member is declared.

default : default means accessible within  a same Package #withinSamePackage.

Protected : protected accessible in derived class only.



Note : To access Private Data Member from outside class. Then getter and setter method helps to do that
 In Getter and Setter Method  Add Some checks and validation before changing  the data member directly..