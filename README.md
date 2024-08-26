# EXPERIMENT 10

## AIM
To study and implement Pointer Operations (call by value and call by reference) 

## THEORY
Call by Value and Call by Reference are two approaches of how arguments can be passed to functions in programming.

Call by Value:

A copy of the actual value is given to the function.

The parameter’s changes that occur in a function have no effect on an initial object.

Commonly used in languages like C, which pass basic data types (such as int or float) by value.

Call by Reference:

A reference (or address) to the actual data is passed to the function.

Changes made to the parameter inside the function directly affect the original argument.

This method is useful when using languages such as C++ (with pointers).

## CODE
a.<br>

```
#include <iostream>
using namespace std;

//call by value
int a,b;
void swap (int a, int b)
{
    int sw;
    sw = a;
    a = b;
    b = sw;
    cout<<"Swapped Values: "<<endl;
    cout<<"a: "<<a<<endl;
    cout<<"b: "<<b<<endl;
}

int main()
{
    int a,b;
    cout<<"Using call by value: "<<endl;
    cout<<"Enter a number: ";
    cin>>a;
    cout<<"Enter another number: ";
    cin>>b;
    cout<<"User Values: "<<endl;
    cout<<"a: "<<a<<endl;
    cout<<"b: "<<b<<endl;
    swap(a,b);
    
}
    
```
<br>

b.<br>

```
#include <iostream>
using namespace std;

//call by value
int a,b;
int *pa, *pb;
void swapr (int *pa, int *pb)
{
    int *psw;
    int sw;
    psw = &sw;
    *psw = *pa;
    *pa = *pb;
    *pb = *psw;
    cout<<"Swapped Values: "<<endl;
    cout<<"a: "<<*pa<<endl;
    cout<<"b: "<<*pb<<endl;
}

int main()
{
    int a,b;
    int *pa, *pb;
    cout<<"Using call by refrence: "<<endl;
    cout<<"Enter a number: ";
    cin>>a;
    pa = &a;
    cout<<"Enter another number: ";
    cin>>b;
    pb = &b;
    cout<<"User Values: "<<endl;
    cout<<"a: "<<a<<endl;
    cout<<"b: "<<b<<endl;
    swapr(pa,pb);
    
}

```
## OUTPUT

![image](https://github.com/user-attachments/assets/4d76a0dd-856b-4e65-a286-81a9256b7d65)

![image](https://github.com/user-attachments/assets/4bdf3ced-7f3b-48ae-9b92-aa7f95d7f40f)




## CONCLUSION
 We learnt about call by value and call by reference in C++. <br>
 We learnt the use case of each in C++. <br>
