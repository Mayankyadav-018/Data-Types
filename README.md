Expt 2 - C++ Program Structure (Data Types)

Aim: To studyand implementC++ Program Structure (Data Types)
Theory:



Variable Definition in C++
type variable_list;
type variable_name = value;

example:
int    i, j, k;
char   c, ch;
float  f, salary;
double d;

extern int d = 3, f = 5;    // declaration of d and f. 
int d = 3, f = 5;           // definition and initializing d and f. 
byte z = 22;                // definition and initializes z. 
char x = 'x';               // the variable x has the value 'x'.

Storage Classes in C++
A storage class defines the scope (visibility) and life-time of variables and/or functions within a C++ Program. These specifiers precede the type that they modify. There are following storage classes, which can be used in a C++ Program
•	auto
•	register
•	static
•	extern
•	mutable
The auto Storage Class
The auto storage class is the default storage class for all local variables.
{
   int mount;
   auto int month;
}

The register Storage Class
The register storage class is used to define local variables that should be stored in a register instead of RAM. This means that the variable has a maximum size equal to the register size (usually one word) and can't have the unary '&' operator applied to it (as it does not have a memory location).
{
   register int  miles;
}
The static Storage Class:
The static storage class instructs the compiler to keep a local variable in existence during the life-time of the program instead of creating and destroying it each time it comes into and goes out of scope.
Therefore, making local variables static allows them to maintain their values between function calls.

The extern Storage Class:
The extern storage class is used to give a reference of a global variable that is visible to ALL the program files. 
When you use 'extern' the variable cannot be initialized as all it does is point the variable name at a storage location that has been previously defined.

Algorithm: Display Data Types and Their Sizes in C++
Start

1- Declare an integer variable a
  Prompt the user to enter an integer.
  Store the input in variable a.
  Display the value of a and its size using sizeof().

2- Declare a float variable b
  Prompt the user to enter a decimal number.
  Store the input in variable b.
  Display the value of b and its size.

3- Declare a double variable d
  Prompt the user to enter a number.
  Store the input in variable d.
  Display the value of d and its size.

4- Declare a char variable c
  Prompt the user to enter a character.
  Store the input in variable c.
  Display the value of c and its size.

5- Declare a string variable s
  Prompt the user to enter a string (single word).
  Store the input in variable s.
  Display the value of s and the size of the string object (note: this shows the object size, not length).

6- Declare two boolean variables
  Assign true to printTrue and false to printFalse.
  Display the value of printTrue.
  Display the size of bool using sizeof(printTrue).

End

Conclusion:
In this experiment, we learned about various data types in C++, such as int, float, char, double, and bool. We understood their sizes, usage, and how they store different types of values.
By writing simple programs, we observed how data types help in declaring variables correctly.
This experiment gave us a strong foundation for handling data efficiently in C++.
