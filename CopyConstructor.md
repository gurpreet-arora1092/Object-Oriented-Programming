
**

## COPY CONSTRUCTOR

Let's take an example  we have an existing Object, We need to create exact copy of given object


Example :

Student st = new Student();
Let's Understand
Student st  // st is Just a reference Variable not an Object It Only Contain  **Address of the Object NOT AN ACTUAL OBJECT**
new Student();  // It only allocate Some Memory to Student Object , Object is only residing in Memory

Student st1 = st; // In st1 Only the reference of st is copied **not an Object**
Now Both of the reference variable Point to the Same Address .
**
// So How to Copy the Actual Object

Student st2 = new Student() // this create a new Object  here st2 store the address of memory which is separate from st.
 // Below is the way to Actual Copy of Object .But this is lengthy way let say if i want to copy all attributes data it takes time.
st2.age = st.age;
st2.year = st.year

There is Another way to Copy the existing object into new by using Copy Constructor

Constructor is Used to Initialise the  value

Student(Student other) {
this.age = other.age;
this.name = other.age;

}

Student st1 = new Student();

//this is the way of Copy Constructor Inside the st1 i initialise the value
// Here st1 data is copy into st2
Student st2 = new Student(st1);





**

## DEEP & SHALLOW COPY

**
Shallow COPY  Whenever you want to Shallow Copy at any particular level, Just need to Copy  the reference at that level

Student st1 = st; // This is the Shallow Copy When the reference is copied

Deep Copy  // deep copy  you need to create a new Object at every level Copy the details instead of reference;
Student st2 = new Student() // this create a new Object  here st2 store the address of memory which is separate from st.
 // Below is the way to Actual Copy of Object .But this is lengthy way let say if i want to copy all attributes data it takes time.
st2.age = st.age;
st2.year = st.year

