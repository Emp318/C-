Variables are containers for storing data values. In C++, there are different **types** of variables (defined with different keywords), for example:
- `int` - stores integers (whole numbers), without decimals, such as 123 or -123
- `double` - stores floating point numbers, with decimals, such as 19.99 or -19.99
- `char` - stores single characters, such as 'a' or 'B'. Char values are surrounded by single quotes
- `string` - stores text, such as "Hello World". String values are surrounded by double quotes
- `bool` - stores values with two states: true or false
# Declaring (Creating) Variables
To create a variable, specify the type and assign it a value:
`type variableName = value;`
Where `type` is one of C++ types (such as `int`), and `variableName` is the name of the variable (such as `x` or `myName`). The **equal sign** is used to assign values to the variable.
You can declare a variable without assigning the value and assign the value later:
![[Pasted image 20241024005644.png]]
Note that if you assign a new value to an existing variable, it will overwrite the previous value:
![[Pasted image 20241024005749.png]]

To declare more that one variable of the same type, use a comma-separated list:
![[Pasted image 20241024005918.png]]

You can assign the same value to multiple variables in one line:
![[Pasted image 20241024005954.png]]
# Identifiers
All C++ variables must be identified with unique names. These unique names are called identifiers. Identifiers can be short names (like ` x` and `y`) or more descriptive names (age, sum, totalVolume). It is recommended to use descriptive names in order to create understandable and maintainable code:
![[Pasted image 20241024010428.png]]
The general rules for naming variables are:

- Names can contain letters, digits and underscores
- Names must begin with a letter or an underscore ().
- Names are case-sensitive (`myVar` and `myvar` are different variables)
- Names cannot contain whitespaces or special characters like !, #, %, etc.
- Reserved words (like C++ keywords, such as `int`) cannot be used as names.
# Constants
When you do not want others (or yourself) to change existing variable values, use the `const` keyword (this will declare the variable as "constant", which means **unchangeable and read-only**):
![[Pasted image 20241024011012.png]]
When you declare a constant variable, it must be assigned with a value:
![[Pasted image 20241024011145.png]]
