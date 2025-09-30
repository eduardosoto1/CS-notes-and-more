# Intro to Syntax and STL

C++ is an **objected-orientated programming (OOP)** language. We will dive into what this means later).

C++ is based off C programming language, but **adds features** like OOP, the **Standard Template Library (STL), and etc**. 

# Basic Syntax

```cpp
#include <iostream> // Header File library
using namespace std; // Allows access to names in the standard libray

int main()
{
	//.. Code goes here..
	
	return 0;
}
```

- Each line is important and is how your code runs
- #include <iostream>
    - is a **header file library**.
    - adds functionality such as input and output which is what iostream focuses on.
    - Forgetting #include <iostream> will cause error as I/O functions will not be defined
- using namespace std;
    - The **standard namespace** contains common objects and functions and makes it easier to write code
    - Removes writing std:: before a keyword
    - Example: Don’t use std::cout, just cout << “Hello”
    - Without using namespace std; must use std:: before
- int main()
    - Where your program execution begins
    - It must return an integer (int), usually 0 to indicate success
- return 0;
    - Ends program and signals execution to OS.

 

## “Hello, World” Program

```cpp
#include <iostream>
using namespace std;

int main()
{
	// Otuputs Hello, World in terminal
	cout << "Hello, world!" << end;
	return 0;
}
```