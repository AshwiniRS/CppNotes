# C++

**What is C++?**
C++ is the programming language that primarily is used for applications which demands energy consumption, speed and performance. 

## Chapter 1 : Getting Started
### 1.1 Writing simple C++ program:
Every C++ program has one or more functions in which one must be named as **main** . The OS runs C++ program by calling main function.

Every function has **four** elements:
		- a return type
		- a function name
		- parameter list enclosed in parenthesis
		- function body
		
Consider following sample main() function in C++.
``` 
int main(){
	return 0;
}
```
In the above code snippet the four elements are:
	- a return type - int
	- a function name - main
	- parameter list enclosed in parenthesis - no parameters hence empty parenthesis
	- function body - block of statements enclosed in curly braces.

A return value from function indicates the success or failure of function. *Return value of 0 indicates success and a nonzero indicates what kind of error occurred.*

**Key Concept - Types**
	Types are one of the most fundamental concept in programming which defines both the contents of data element and the operations that are possible on those data. When varaible v is of type T, then we say that "v is T" or "v has type T".

### 1.2 First Look at Input/Output
C++ includes an extensive standard library that provides IO. We will be looking at examples in this book which uses the iostream library. Fundamental to iostream library are to types named - istream and ostream, which represents input and output streams respectively. A stream in a sequence of characters (generated, or consumed sequentially over time) which is read from or written to IO device.

**Standard Input and Output Objects**

There are four IO objects : 
1. cin - istream object - standard input
2. cout - ostream object - standard output
3. cerr - ostream object - standard errror (for warning and error messages)
4. clog - ostream object - for general information about the execution of the program.

Lets use these input and output objects in a program. For example, we will write a C++ program to calculate sum of two numbers.

```
#include <iostream>
int main(){
	std::cout << "Enter two numbers :" <<std::endl;
	int v1=0,v2=0;
	std::cin >> v1 >> v2;
	std::cout << "The sum of " << v1 << " and " << v2 << " is " << v1+v2 << std::endl;
	return 0;
}
```


