directory 

14.2.1 Position Parameters and Keyword Parameters 

Default values for parameters 14.2.2 function 

14.2.3 function reference type parameters 

Variable parameters of 14.2.4 function 

14.2.5 knowledge points 

Learn Python 14.2.6 System 

##  14.2.1 Position Parameters and Keyword Parameters 

Positional parameters are related to the position of the parameters, where the position refers to the left-to-right parameter arrangement order when defining the function. When calling the function, the positions of the entities participating in the formal parameters are automatically matched. If a one-to-one correspondence between the parameters cannot be established, the Python interpreter will throw an exception message with the wrong type. 

>  When the number of real parameters is less than or greater than the number of formal parameters, one-to-one correspondence between parameters cannot be established. 

Keyword parameters refer to the calling of a function, using the parameter name as the key name and the actual parameter as the key value, and calling it in the form of the syntax of key name = key value. The calling syntax of keyword parameters: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957458882
 ```  
Here, key is the parameter name, and value is the argument value. When called in the form of keyword parameters, the Python interpreter will automatically correspond the argument value to the parameter without remembering the parameter's location. 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957458882
 ```  
When calling with keyword arguments, there is no need to remember the parameter order when the function is defined. 

##  Default values for parameters 14.2.2 function 

When defining a function, you can set default values for parameters in the syntax form: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957458882
 ```  
default_value represents the default value of the parameter. After setting the default value for the parameter, if the corresponding argument is not passed, the default value will be used instead. 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957458882
 ```  
When defining the default value of a parameter, set the default value in right-to-left argument order, otherwise Python will throw an exception message with a syntax error: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957458882
 ```  
##  14.2.3 function reference type parameters 

A variable in Python is a container that holds a memory address. When the parameter passed is a composite data type, it is a copy of the memory address stored by the variable. When modifying the type of parameter in a function, the value of the same memory space is modified. The so-called reference type parameter refers to the same memory space that the parameters in the function body refer to. 

>  Composite data types in Python: string, list, tuple, dictionary, collection. 

 Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957458882
 ```  
Since the value of the same memory space is modified, even after the function call ends, it will affect variables outside the function body. In the above code example, the output of the numbers table in the front of the calling function is: 

>  [1,2,3] 

In the function body, add the argument 4 to the list numbers, and the output in the function body is: 

>  [1,2,3,4] 

Since the value of the same memory space is modified, after the function call ends, the output of the list numbers is also: 

>  [1,2,3,4] 

When passing a simple data type, simply copy the value: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957458882
 ```  
>  Simple data types in Python: integers, floating-point types, boolean types 

##  Variable parameters of 14.2.4 function 

When defining a function, if you cannot determine the number of parameters to the function, you can use variable parameters. Variable parameters involve a lot of knowledge points. For variable parameters of functions, we will explain in detail in Section 14.3. 

##  14.2.5 knowledge points 

>  (1) Position parameters are related to the position of the parameters, where the position refers to the left-to-right order of parameters when defining a function.

(2) Keyword parameters refer to calling a function, using the parameter name as the key name and the actual parameter as the key value, and calling it in the syntax form of key name = key value.

(3) When defining a function, default values can be set for parameters. Default values must be set in right-to-left parameter order.

When calling a function, if the corresponding argument is not passed, the default value is used instead.

(4) A variable in Python is a container that holds a memory address. When the argument passed is a composite data type, it is a copy of the memory address stored by the variable. The so-called reference type parameter refers to the same memory space as the argument in the function body. 

##  Learn Python 14.2.6 System 

>  About the French fries teacher: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. French fries teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning, quantitative investment. 

