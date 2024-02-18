directory 

14.4.1 understand anonymous functions 

14.4.2 lambda expression 

14.4.3 lambda expressions and named functions 

14.4.4 knowledge points 

Learn Python 14.4.5 System 

##  14.4.1 understand anonymous functions 

Anonymous function, from its literal meaning to understand. The so-called anonymous is not named, no name. Anonymous function, that is, no function name function. 

![avatar]( e0768b8e896d12a03de4e24350451b6f.png) 

In Python, anonymous functions are defined through lambda expressions. 

##  14.4.2 lambda expression 

Regarding lambda expressions, you can execute help ("lambda") in interactive mode to view their definition: 

>  >>> help("lambda")

Lambda

*******

  lambda_expr        ::= "lambda" [parameter_list] ":" expression

  lambda_expr_nocond ::= "lambda" [parameter_list] ":" expression_nocond

Lambda expressions (sometimes called lambda forms) are used to create

anonymous functions. The expression "lambda parameters: expression"

yields a function object.  The unnamed object behaves like a function

object defined with:

  def <lambda>(parameters):

      return expression

See section Function definitions for the syntax of parameter lists.

Note that functions created with lambda expressions cannot contain

statements or annotations.

Related help topics: FUNCTIONS 

From the output of help ("lambda"), we can see that the lambda expression is used to create an anonymous function: 

>  Lambda expressions (sometimes called lambda forms) are used to create anonymous functions. 

Syntax structure of lambda expression: 

>  lambda parameters: expression 

Parameters represents the list of parameters of the function, the parameters are separated by commas, and the list of parameters can be empty like named functions. expression represents the code logic of the expression you want to implement, and the value of the expression will be returned directly to the function caller without returning it through return. 

>  A named function is a function with a function name. A function defined by def is called a named function. 

In order to facilitate students' understanding of anonymous functions, we now use named functions and anonymous functions to write code with the same logic: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574578365
 ```  
An anonymous function is defined in the above code and then assigned to the variable anonymous_accumulate. A variable in Python is a container that stores the memory address, and the variable anonymous_accumulate actually stores the memory address of the anonymous function. When Python executes an anonymous function, it first fetches the memory address of the anonymous function from the variable, and then calls it. 

##  14.4.3 lambda expressions and named functions 

Compared with named functions, lambda expressions are simpler in form and can be done with just one line of code. But it also limits the ability of lambda expressions to implement complex code logic. To implement complex code logic, named functions should also be used. Lambda expressions are flexible to use, and can be passed as parameters, returned to the caller as a return value, or directly embedded in other data structures. 

(1) Use lambda expressions as default values for arguments 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574578365
 ```  
If you use named functions, there is no such flexibility. Of course, we can also pass named functions directly as parameters when calling: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574578365
 ```  
Embedding lambda expressions into a dictionary structure 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574578365
 ```  
(3) Use lambda expressions as return values 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574578365
 ```  
Of course, you can also directly return a named function as a return value, but it is not as concise as an anonymous function. 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574578365
 ```  
In the code example above, the define accumulate is actually a closure function. Closure functions are explained in detail in Advanced Usage of Functions. 

##  14.4.4 knowledge points 

>  (1) Anonymous functions, that is, unnamed functions without a function name.

(2) Define anonymous functions through lambda expressions in Python. When using an anonymous function, first save the address of the anonymous function through a variable. This can be called below.

(3) Lambda expressions are simpler in form than named functions, requiring only one line of code. 

##  Learn Python 14.4.5 System 

>  About the French fries teacher: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. French fries teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning, quantitative investment. 

