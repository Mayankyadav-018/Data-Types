Expt 2 - C++ Program Structure (Data Types)

Aim: To studyand implementC++ Program Structure (Data Types)
Theory:
C++ Data Types
Primitive Built-in Types
Type	Keyword
Boolean	bool
Character	char
Integer	int
Floating point	float
Double floating point	double
Valueless	void
Wide character	wchar_t

Type	Typical Bit Width	Typical Range
char	1byte	-127 to 127 or 0 to 255
unsigned char	1byte	0 to 255
signed char	1byte	-127 to 127
int	4bytes	-2147483648 to 2147483647
unsigned int	4bytes	0 to 4294967295
signed int	4bytes	-2147483648 to 2147483647
short int	2bytes	-32768 to 32767
unsigned short int	2bytes	0 to 65,535
signed short int	2bytes	-32768 to 32767
long int	8bytes	-9223372036854775808 to 9223372036854775807
signed long int	8bytes	same as long int
unsigned long int	8bytes	0 to 18446744073709551615
long long int	8bytes	-(2^63) to (2^63)-1
unsigned long long int	8bytes	0 to 18,446,744,073,709,551,615
float	4bytes	
double	8bytes	
long double	12bytes	
wchar_t	2 or 4 bytes	1 wide character


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

Conclusion:
In this experiment, we learned about various data types in C++, such as int, float, char, double, and bool. We understood their sizes, usage, and how they store different types of values.
By writing simple programs, we observed how data types help in declaring variables correctly.
This experiment gave us a strong foundation for handling data efficiently in C++.
