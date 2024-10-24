`<iostream>` is short for standard input /output streams. The `<iostream>` library provides objects which can read user input and output data to the console or to a file. All iostream objects are defined in the `<iostream>`header file. A list of all iostream objects can be found below.
# `cerr`
The `cerr` object is used to output error messages. It behaves identically to `cout` but it can be directed to a different destination such as an error log file. `cerr` and `clog` always write to the same destination.
Unlike `cout` and `clog` , `cerr` is not buffered. A buffered output would store the output temporarily in a variable and not write to the destination until certain conditions are met. Buffered outputs are more efficient because they do fewer operations on files. `cerr` is not buffered so that the error messages can be written to a file before the program crashes.
### Example
Direct `cerr` to write a file instead of to the console.
```cpp
#include <iostream>
#include <fstream>
using namespace std;

int main() {
  int x = 5;
  int y = 0;

  // Set "error.log" as the output file for the error messages
  ofstream log("error.log");
  cerr.rdbuf(log.rdbuf());
  
  // Write an error message
  if(y == 0) {
    cerr << "Division by zero: " << x << " / " << y << "\n";
  } else {
    cout << (x / y);
  }

  // Close the file
  log.close();
  
  return 0;
}
```
# `clog`
The `clog` object is used to log messages about the state of the program. It behaves identically to `cout` but it can be directed to a different destination such as a log file. `clog` and `cerr` always write to the same destination. The difference between this two is that `clog` is buffered and `cerr` is not. If the messages are important, use `cerr`instead because otherwise they may be lost if the program crashes.
### Example
Direct `clog` to write to a file instead of the console:
```cpp
#include <iostream>
#include <fstream>
using namespace std;

int main() {
  int myNum = 12;

  // Set "info.log" as the output file for the log messages
  ofstream log("info.log");
  clog.rdbuf(log.rdbuf());
  
  // Write to the log file
  clog << "The number " << myNum << " was given\n";

  // Close the file
  log.close();
  
  return 0;
}
```
# `cin`
The `cin` object is used to read keyboard input or data from a file. The `cin` object can be used with the extraction operator. The extraction operator converts input data to the appropriate type for the variable:
```cpp
int x;
cin >> x;
```
The extraction operator can be used more than once on the same line to put data into multiple variables:
```cpp
int x, y;
cin >> x >> y;
```
In addition to the extraction operator `>>`, the `cin` object also has methods to read input.
- get(): the `cin.get()` method reads one character from the input source and returns it.
```cpp
char c = cin.get();
cout << c;
```
