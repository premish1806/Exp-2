# Exp-2
Data types in C++

## Aim:
 to understand the concept of data type sizes in C++ and to explore the behavior of static and non-static variables within a function.

## Software Used:
- Dev c++

## Theory:
Data Type Sizes:<br>
In C++, different data types occupy varying amounts of memory, which is crucial to know for optimizing performance and managing resources effectively. The sizeof operator is used to determine the size, in bytes, of any data type or object. Understanding these sizes helps in ensuring that the program uses memory efficiently and that there is no unintended overflow or underflow in variables.

Static Variables:<br>
Static variables in C++ maintain their value between function calls. Unlike local variables, which are reinitialized each time a function is invoked, static variables are initialized only once and retain their value even after the function exits. This is useful in scenarios where the function needs to remember the state from previous executions.

## Program 1:  Write a program to show size of different data types.
<strong> Code: </strong>
<br>
```cpp
// Premish Ninawe
// 23070123092
// ENTC B1
#include<iostream>
using namespace std;
int main()
{ 
    cout << "Size of Integer is: " << sizeof(int) <<" bytes"<< endl;
    cout << "Size of Float is: " << sizeof(float) <<" bytes"<< endl;
    cout << "Size of String is: " << sizeof(string) <<" bytes"<< endl;
    cout << "Size of Character is: " << sizeof(char) <<" bytes"<< endl;
    cout << "Size of Short Integer is: " << sizeof(short int) <<" bytes"<< endl;
}
```
<strong> Output: </strong>
<br>


## Program 2:  Write a program to show size of different data types.
<strong> Code: </strong>
<br>
```cpp
// Premish Ninawe
// 23070123092
// ENTC B1
#include<iostream>
using namespace std;

void staticExample(){
    int z = 0;
    z++;
    cout<<"The value of z is: "<<z<<endl;
}

int main(){
    staticExample();
    staticExample();
    return 0;
}
```
<strong> Output: </strong>
<br>

## Conclusion:
We learned that knowing the size of data types helps in managing memory efficiently. We also discovered that static variables keep their value between function calls, while regular variables do not.



