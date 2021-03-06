---
title: Functions in C++
---
## Definition:

A function is a group of statements that together perform a task. Every C++ program has at least one function, which is `main()`.

A function declaration tells the compiler about a function's name, return type, and parameters. A function definition provides the actual body of the function.
One must always make sure, before using a function in the program, the function is defined.
Even if function definition is after the main, just the function name and its arguments have to be declared above, so that compiler knows what is being talked about.

## The general form of a C++ function definition:

```cpp
return_type function_name( parameter list )
{
   body of the function
}
```

### Return type:
A function may return a value. The `return_type` is the data type of the value the function returns. Some functions perform the desired operations without returning a value. In this case, the `return_type` is the keyword `void`, but the [return type of main() must always be int](https://stackoverflow.com/a/4207223/).

### Function name:
This is the actual name of the function. The function name and the parameter list together constitute the function signature.

### Parameters:
A parameter is like a placeholder. When a function is invoked, you pass a value to the parameter. This value is referred to as actual parameter or argument. The parameter list refers to the type, order, and number of the parameters of a function. Parameters are optional; that is, a function may contain no parameters.

### Function body:
The function body contains a collection of statements that define what the function does.

##Example:

```cpp
int max(int num1, int num2)
{
   // local variable declaration
   int result;
 
   if (num1 > num2)
      result = num1;
   else
      result = num2;
 
   return result; 
}
## calling a function:

int res;
res=max(5,10);

// if the function returns a value, assign it to that variable, else just call it like function(arg1,arg2);
```

## Why are functions important?

Functions support modularity (breaking down of work into smaller pieces called modules), which is an essential feature of object-oriented programming (OOP) which primarily separates C++ from C.

Having specific functions to perform specific tasks removes confusion and shortens the length of the main function.

The function also performs reusability of code. So the next time you have to calculate the maximum of two different numbers again and again in the same program, you do not need to copy and paste your code. You just have to call the function and it does rest of the work.

## More Information

* [TutorialsPoint](https://www.tutorialspoint.com/cplusplus/cpp_functions.htm)
