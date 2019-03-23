# Csharp-Questions1
this repo holds the questions and answers from the Csharp Questions1 challenge

1.)	What is a namespace?
-	“ a namespace is a set of symbols that are used to organize objects of various kinds, so that these objects may be referred to by name.” – Wikipedia
-	Basically, a namespace exists so that you can use the same class name in different areas of your program without running into a situation of name collision. A good example I found is to think of a namespace as someone’s last name. For instance, my name is Eric, but there are other people with the name Eric too, and last names are used to differentiate between them.

2.)	What is a value type?
-	“A variable of a value type contains a value of the type.” – docs.microsoft.com
-	Value types are variable types that hold an actual value inside of them. For example, a variable with the type “int” will hold a value of an integer, say 10. When the value is assigned to the variable, the value is copied into it. Examples of value types are ints, doubles, bools, etc.

3.)	What is a reference type?
-	“A reference type contains a pointer to another memory location that holds the data.” – docs.microsoft.com
-	Can’t really be put much simpler than that. A reference type holds a pointer that points to a memory location holding the information. I will add that this is a very helpful tool in programming languages such as C for pointer manipulation and passing values by reference, as to avoid using a return value. Examples of reference types are classes, objects, strings, etc.

4.)	What is an automatic property and how is it useful?
-	“Automatic properties are used when no additional logic is required in the property accessors.” – Stackoverflow.com
-	Automatic properties are useful because they allow the writer to omit several lines of code and makes your code look neater and more professional.

5.)	What is the purpose of Using statement?
-	“Provides a convenient syntax that ensures the correct use of IDisposable objects.” – docs.microsoft.com
-	The “using” statement basically ensures that dispose is called even if an exception occurs. The same effect can be achieved by using a “try” block and calling dispose in a “finally” block.

6.)	What are dynamic type variables?
-	“a new type that avoids compile time type checking.” – tutorialsteachers.com
-	This type of variable is checked at run time instead of compile time. It is declared using the keyword “dynamic” and, in most cases, acts as if it has the type “object.”

7.)	What is the purpose of the “is” operator?
-	The “is” operator is used to dynamically check if an object is compatible with a given type. The “is” operator returns a Boolean, true of false, and never has an exception, so it is reliable for application code.

8.)	What are generics and how is using them helpful?
-	“Generics allow you to define the specification of the data type of programming elements in a class or a method, until it is actually used in the program.” – tutorialspoint.com
-	Basically generics allow you to write a method that is compatible with any data type.

9.)	What is the scope of a public member of a class?
-	Any public member of a class can be accessed from anywhere inside or outside of the class.

10.)	 Can you create a function that can accept a varying number of arguments?
-	Yes, something like this can be written:
Void name(params int[] numbers)
The params keyword specifies a parameter that takes a variable amount of arguments

11.)	 How do you sort an array?
-	There are multiple ways to sort an array, but in my experience the easiest way to do this is using the Array.Sort() method, which sorts your array in ascending order. After this if you want it sorted in descending order you can use the Array.Reverse() method.

12.)	 What is a nullable type and what purpose does it serve?
-	A nullable type is a data type that you can assign any value to including null. An example of when to use a nullable type is when using a bool. Normally bools are either true or false, not allowing for an undefined value. A nullable bool allows you to define a bool as neither true nor false.

13.)	 What is an enumeration?
-	“An enumeration is a set of named integer constants.” – tutorialspoint.com
-	Enumerations are value types and are declared using the keyword enum. By default, the first enumerator is 0 and every member after that increases by 1.

14.)	 What is inheritance?
-	Inheritance is the ability of a class to inherit or derive its attributes and characteristics from an already existing class.

15.)	 Is multiple inheritance supported?
-	Multiple inheritance is supported, meaning that a class can inherit characteristics from more than one parent class.

16.)	 What is the purpose of “as” operator?
-	As operator is similar to the is operator, with a few differences. These differences include the following: As operator does not return a bool, it returns the object when its compatible with the given type. As operator performs conversion between compatible reference and nullable types and is only used for reference, nullable and boxing conversions.

17.)	 What is an object?
-	“Object, in C#, is an instance of a class that is created dynamically.” – techopedia.com
-	An object (or instance) is a block of memory that is allocated based on the class or struct it is in.

18.)	 What is the difference between a struct and a class?
-	The simplest difference between a class and a struct is that structs are value types and classes are reference types. Structs are stored on a stack and class are stored on a heap.

19.)	 What is the difference between continue and break statements?
-	A break statement breaks out of the loop and a continue statement skips the current iteration of the loop but does not break the loop.

20.)	 What is this and how is it used?
-	This keyword refers to the current instance of the class – docs.microsoft.com
-	This is used to pass an object as a parameter, declare indexers, and qualify members hidden by similar names

21.)	 What is try and catch and when are they used?
-	“A try block identifies a block of code for which particular exceptions is activated. It is followed by one or more catch blocks. A program catches an exception with an exception handler at the place in a program where you want to handle the problem. The catch keyword indicates the catching of an exception.” – tutorialspoint.com
-	The try block contains the code that could cause an exception and the catch block should contain an argument to catch any exception that may occur during the try block.

22.)	 How is exception handling done?
-	An exception is an error that occurs during a program. There are 4 keywords used for exception handling: try, catch, finally and throw. I already explained try and catch, a finally block is used to carry out a block of code regardless of whether an exception occurs or not. 

23.)	 What is finally and what is its purpose?
-	a finally block is used to carry out a block of code regardless of whether an exception occurs or not. 

24.)	 List the differences between Array and ArrayList
-	Arrays: can only contain the same data type, can not have null, and is strongly typed
-	ArrayLists: can store all data types, can have null, and is not strongly typed

25.)	 What is an object?
-	This is a repeat question, see #17

26.)	 Define constructor
-	“A constructor is a special method of the class which gets automatically invoked whenever an instance of the class is created.” – geeksforgeeks.org
-	A constructor is a method with the same name as its type. For instance:
Public class Dog
{
	Private string name;
	Private string weight;
	
	Public Dog(string name, string weight)
{
		//This is an example of a constructor
	}
}

27.)	 When can var be used to declare a variable and how is the type of the variable determined?
-	Var can only be used when a variable is declared and initialized at the same time. The type of variable is determined by the compiler by reading the right side of the initialization.

28.)	 What is an abstract class?
-	Abstract classes are classes that need to be implemented in a derived class. The purpose of these are to set a common definition of a base class for other derived classes to use.

29.)	 What is an interface?
-	An interface only holds the signatures of a method, indexer, property or event and is implemented by a class or struct using the members specified by the interface.

30.)	 What is a method?
-	A method is a code block that contains statements executed by the program. The main method is the entry point for every program.

31.)	 What is a property?
-	A property is a member of a method that tells the program to read, write or compute the value of a field.

32.)	 What is an access specifier?
-	Access specifiers tell you how accessible a type or member is. Examples are public, private, protected etc.

33.)	 What access specifiers are supported and what do they mean?
-	Public: type or member can be accessed anywhere in the program
-	Private: type or member can only be accessed in the same class or struct
-	Protected: type or member can only be accessed in the same class or a derived class
-	Internal: type or member can be accessed from anywhere within the assembly
-	Protected Internal: type or member can be accessed anywhere in which its declared or a derived class in another assembly
-	Private Protected: type or member can only be accessed within its declaring assembly, by code in the same class or in a type derived from the class

34.)	 What are collections?
-	Collections are a flexible way to work with a group of objects, allowing the group to grow or shrink dynamically.

35.)	 What is a Hash Table?
-	A hash table is a collection key and value pairs organized based on the hash code of the key
