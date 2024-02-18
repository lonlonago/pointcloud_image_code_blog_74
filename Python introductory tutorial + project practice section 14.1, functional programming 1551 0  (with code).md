directory 

14.1.1 understand function types 

Definition of 14.1.2 function 

14.1.3 function parameters, arguments, and calls 

Return value of 14.1.4 function 

Naming convention for 14.1.5 functions 

14.1.6 knowledge points 

Learn Python 14.1.7 System 

##  14.1.1 understand function types 

In Python, a function is also a data type. Before we understand function types, let's look at a simple code example that computes the sum of all composite numbers in a range: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570968
 ```  
In the above code, the sum of all composite numbers between 1 and 10 is calculated by the for loop. If the sum of all composite numbers between 100 and 1000 needs to be calculated in the following? So, how to write the code? The easiest thing to do is to use the for loop again to write a piece of code that is logically the same, but this will cause redundancy in the code. 

>  In computer programming, blocks of code that need to be reused can be encapsulated into a function, so that they can be called directly the next time they are used, without repeated writing. Students can understand a function as a converter from input to output. For example, a language translator is a function that outputs one language to another. 

![avatar]( 84c96d27adfce173a61d528f5fcde320.png) 

##  Definition of 14.1.2 function 

In Python, the keyword def is used to define functions. For the definition of def, you can execute help ("def") in interactive mode to find it: 

>  >>> help("def")

Function definitions

********************

A function definition defines a user-defined function object (see

section The standard type hierarchy):

...... 

The basic syntax of a function definition: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570968
 ```  
function_name represents the function name, when the function is called again in the following, it needs to be referenced by the function name, and the function without the function name is called an anonymous function. 

>  Function names in Python are usually lowercase English words or combinations of words. When naming a function, the function name should be highly readable, that is, the function's function can be known by the function name. Function names can refer to the naming style of variables. 

parameter_list denotes a list of parameters. The parameter list means that the function can contain multiple parameters, and the parameters are separated by English commas. The so-called parameters refer to the input of the function. Functions usually have an output. In Python, the return statement ends the execution of the function and returns a value. 

>  Students can simply understand Python as a conversion from input to output, defining the input of the function through the parameter list, and defining the output value through the return value of the function. The return in the function is not required, which means that the function can have no return value. 

Now we will calculate the sum of the composite numbers in the range of the interval and define it through the function to understand the function thoroughly. 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570968
 ```  
##  14.1.3 function parameters, arguments, and calls 

In the 14.1.2 section, a sum_of_composite_numbers function is defined to calculate the sum of composite numbers in the range of the interval. The function declared at the time of function definition is called a parameter, which is equivalent to a placeholder. The parameters actually passed when calling the function are called arguments. Syntax of function call: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570968
 ```  
function_name represents the name of the function, arguments_list represents the list of arguments, and the parameters are separated by commas. The number of parameters passed when calling the function must be the same as when the function is defined, and Python will correspond the positions of the arguments to the positions of the formal parameters one by one. Such parameters are called positional parameters. In Python, you can also call functions in the form of keyword parameters, which will be explained in detail in the following section. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570968
 ```  
When calling a function, if the number of parameters does not match the number when the function is defined, Python will throw an exception message with the wrong type: 

>  >>> sum_of_composite_numbers(100)

Traceback (most recent call last):

 File "<stdin>", line 1, in <module>

TypeError: sum_of_composite_numbers() missing 1 required positional argument: 'stop' 

In Python, everything is an object, and a function is also a data type. You can output the type name of the function through type and pass the function name directly in type: 

>  >>> type(sum_of_composite_numbers)

<class 'function'> 

As you can see from the output, the function type name in Python is function. 

##  Return value of 14.1.4 function 

Functions usually have a return value. In Python, the value is returned by return. The returned value can be of any data type. When multiple values need to be returned, they are separated by commas. "Multiple return values" in Python functions are essentially a tuple type. 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570968
 ```  
##  Naming convention for 14.1.5 functions 

In Python, function naming also has its own set of conventions. Function names must first conform to the basic rules for naming variables. 

>  Readers who are not yet familiar with variable naming conventions can review the content in Section 6.1, "Variable Naming". 

In addition to the basic rules, function names should also adhere to the following two important rules: 

>  1. Maintain good readability: that is, the function name must be meaningful, and readers can immediately know the purpose of the function when they see the function name. In addition, try to use English words to name the function.

2. Use lowercase for function names: Use lowercase to distinguish it from global variable names, class names, etc. Global variable names are generally uppercase, while class names use the uppercase form of the first letter of the word. If the function name needs to use multiple words to name, the words are separated by the underscore "_". 

For more details on the function naming convention, readers can refer to the famous PEP8 specification 

##  14.1.6 knowledge points 

>  (1) Functions in Python are also an abstract data type, and the type name of the function can be output by type

(2) Use the keyword def to define functions in Python. The parameter list when the function is defined is a formal parameter, and the parameter list when the function is called is an actual parameter

(3) Basic properties of functions: function name, parameters, return value 

##  Learn Python 14.1.7 System 

>  About the French fries teacher: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. French fries teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning, quantitative investment. 

