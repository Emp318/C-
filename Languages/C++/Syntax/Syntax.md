Let's break up the following code to understand it better:
![[Pasted image 20241023141456.png]]
- `#include <iostream>` is a header file library that lets us work with input and output objects, such as `cout`. Header files add functionality to C++ programs
- `Using namespace std` means that we can use names for objects and variables from the standard library.
- A blank line which ignored by the C++ compiler. It makes the code more readable.
- `int main()` is a function. Any code inside its curly brackets `{}` will be executed.
- `cout`(pronounced "see-out") is an object used together with the insertion operator (`<<`) to output/print text. It will output "Hello World!".
- `return 0;` ends the main function.
### Note: Every C++ statement ends with a semicolon `;`. C++ is case-sensitive: "`cout`" and "`Cout`" has different meaning. The body of `int main()` could also be written as `int main () { cout << "Hello World!"; return 0; }`. White spaces are ignored by the C++ compiler. White spaces are just used to make the code more readable.
# Omitting Namespace
Some C++ programs can run without the standard namespace library. The `using namespace std` line can be omitted and replaced with the `std` keyword, followed by `::` operator for some objects:
![[Pasted image 20241023143350.png]]
