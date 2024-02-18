directory 

9.3.1 string Common operation methods 

9.3.2 get string length 

9.3.3 string case operation 

9.3.4 remove whitespace from string 

9.3.5 string substring lookup 

9.3.6 string substring statistics 

Substring substitution 9.3.7 string 

Split function 9.3.8 string 

9.3.9 string prefix and suffix 9.3.10 knowledge points 

Learn Python 9.3.11 System 

##  9.3.1 string Common operation methods 

The string type is an abstract data type. The abstract data type defines the operation methods of the data type. In this section, we focus on the common operation methods of string. 

![avatar]( 65e36930cea499f9b9d6f6d9bef65b56.png) 

##  9.3.2 get string length 

(1) only (p) 

Function description: 

Returns the number of characters contained in string str 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574580007
 ```  
##  9.3.3 string case operation 

(1) str.lower()  

Function description: 

Converts all uppercase and lowercase characters in string str to lowercase, returning a string. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574580007
 ```  
(2) str.upper()  

Function description: 

Converts all uppercase and lowercase characters in string str to uppercase, returning a string. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574580007
 ```  
(3) str.islower()  

Function description: 

>  In Python, the function name or variable name is prefixed with an is, indicating whether it means whether, and returns a boolean type. islower is used to determine whether the upper and lower case characters in the string are lowercase, if they are all lowercase, return True, otherwise return False. The upper and lower case characters here mainly refer to Latin letters. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574580007
 ```  
(4) str.isupper()  

Function description: 

>  The isupper function is used to determine whether the uppercase and lowercase characters in the string are all uppercase. If they are all uppercase, return True, otherwise return False. The uppercase and lowercase characters here mainly refer to Latin letters. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574580007
 ```  
##  9.3.4 remove whitespace from string 

(1) str.strip()  

Function description: 

>  Removes whitespace at the beginning and end of the string, returning a new string that does not contain whitespace at the beginning and end. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574580007
 ```  
(2) str.lstrip()  

Function description: 

>  The prefix l in the function name is shorthand for the word left. This method removes the leftmost whitespace character of the string and returns a new string with no whitespace at the beginning. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574580007
 ```  
(3) str.rstrip()  

Function description: 

>  The prefix r in the function name is shorthand for the word right. This method removes the rightmost whitespace character of the string and returns a new string with no whitespace at the end. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574580007
 ```  
##  9.3.5 string substring lookup 

(1) str.find(sub)  

Function description: 

>  Find the first occurrence of the substring from left to right. If the search is successful, return the index of the beginning position of the substring in the main string. Otherwise, the return value is -1. The index value here is the same as the index value in the string index access. The index value in Python is numbered from 0. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574580007
 ```  
(2) str.rfind(sub)  

Function description: 

>  Find the first occurrence of the substring from right to left. If the search is successful, return the index of the beginning position of the substring in the main string, otherwise the return value is -1. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574580007
 ```  
##  9.3.6 string substring statistics 

(1) str.count(sub)  

Function description: 

>  Counts the number of occurrences sub_str substring in string str and returns an integer value. If there is no corresponding substring, the returned value is 0. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574580007
 ```  
The count method is now implemented through the string's find method, the slice operation, and the while loop structure. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574580007
 ```  
##  Substring substitution 9.3.7 string 

(1) str.replace(old, new)  

Function description: 

>  Replace the substring in string with a new string, returning a new string. Replace the substring represented by the parameter old with the new string new. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574580007
 ```  
Now the replace method is implemented through the string's find method, slicing operation, and while loop structure. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574580007
 ```  
For the above code example, students can understand it in combination with the following diagram: 

![avatar]( d3e9b24085bd9fe8ab18b34855fedc09.png) 

The middle part represents the substring to be replaced, the left part of the starting position of the substring is left, and the right part of the tail of the substring is right. 

##  Split function 9.3.8 string 

(1) str.split(sep=None, maxsplit=-1) 

Function description: 

>  Using sep as the delimited string, returns a list of strings separated by sep string. If maxsplit is given, maxsplit is performed at most. If maxsplit is not specified or -1, there is no limit to the number of splits. The sep argument may consist of multiple characters (e.g. '1 @@2 @@3' .split ('@@') will return ['1',' 2', '3']). 

The output type of the string type after executing the split function is the list type. Students can come back to understand the split function after learning the list type. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574580007
 ```  
##  9.3.9 string prefix and suffix 

(1) str.startswith (prefix) Determines whether the string is prefixed with a prefix substring, and the return value is a Boolean type 

(2) str.endswith (suffix) Determines whether the string is suffixed with a suffix substring, and the return value is a boolean type 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574580007
 ```  
##  9.3.10 knowledge points 

>  (1) The string type is an abstract data type, and the abstract data type defines the operation method of the data type

The len method is a global method that returns the number of elements of a composite data type.

(3) The function name or variable name in Python is prefixed with an is to indicate whether

(4) Carriage returns, line breaks, tabs, spaces, etc. are all whitespace characters 

##  9.3.11 the most powerful small class training 

>  About the French fries teacher: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. French fries teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning, quantitative investment. 



--------------------------------------------------------------------------------

directory 

9.5.1 What is pattern matching? 

9.5.2 naive pattern matching algorithm 

Learn Python 9.5.3 System 

##  9.5.1 What is pattern matching? 

Pattern matching is a basic operation of strings in a data structure: given a substring, it is required to find all substrings that are the same as the substring in the main string, which is pattern matching. For a simple example, the main string is "Chinese people do not bully Chinese people", and the substring is "China". The substring here is the pattern to be matched, and finding all the patterns "China" in the main string "Chinese people do not bully Chinese people" is a pattern matching. 

##  9.5.2 naive pattern matching algorithm 

This section aims to implement a very simple naive pattern matching algorithm. Let's first grasp the basic ideas of the naive pattern matching algorithm: 

>  From the first character of the main string, it is compared with the first character of the pattern string. If it is equal, the subsequent comparison of the characters is continued. Otherwise, it is re-compared with the first character of the pattern string from the second character of the main string. This process is repeated until each character in the pattern string is equal to a consecutive character sequence in the main string. At this time, it is called a match success, otherwise the match fails. 

According to the above ideas, we use the Python language to implement the naive pattern matching algorithm of string: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957452975
 ```  
##  Learn Python 9.5.3 System 

>  About the French fries teacher: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. French fries teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning, quantitative investment. 



--------------------------------------------------------------------------------

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



--------------------------------------------------------------------------------

directory 

9.4.1 understand formatting 

9.4.2 formatting with f-string 

9.4.3 formatting with formatting symbols 

9.4.4 format using the format method 

9.4.5 knowledge points 

Learn Python 9.4.6 System 

##  9.4.1 understand formatting 

Students are more familiar with disk formatting. After formatting the disk, all the files in the disk are cleared. So, what is string formatting? Formatting a string does not clear the characters in the string. String formatting refers to the output of a string according to a specific format. 

![avatar]( b7c700ffd2ec83fbb21fc5f2d7b3af27.png) 

For a simple example, in string "{1} {2} {3}", if the output is an integer at the {1} position, a string at the {2} position, and a floating-point number at the {3} position, then the formatted string output is: "Integer string floating-point number". There are three main ways to format strings in Python: one is through f-string, the other is using the format symbol with the operator%, and the last is through the format method of string. 

##  9.4.2 formatting with f-string 

F-string is a formatting method introduced after Python 3.6 version. This formatting method is simple in syntax and easy to use. It is the most commonly used formatting method when I develop Python programs. French fries teacher also recommends that you use this latest formatting method. Before learning the formatting method of f-string, let's first grasp the basic concept of f-string: the so-called f-string refers to the prefix with an f in front of the quotation marks of the string. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574568062
 ```  
Formatting with f-string is very simple. Formatting can be achieved by using {} in string to output the value of the expression: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574568062
 ```  
##  9.4.3 formatting with formatting symbols 

(1) Formatting basic grammar 

Common formatting symbols in Python: 

![avatar]( afef67e5ce3e85e38b44e6930ecd4071.png) 

>  For more formatting symbols, students can consult the official Python documentation. When learning Python, students only need to master the core concepts and learning methods, and then proceed to further study after understanding the basic principles and operations. 

In Python, use the format symbol with the% operator to format a string, format the string, and return a string of a specific format. The string formatting syntax is: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574568062
 ```  
The string str contains the corresponding formatting symbols. The formatting parameters in the parentheses must correspond to the formatting symbols one by one. The parentheses () in the formatting syntax are not required. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574568062
 ```  
Code explanation: 

>  (1) Format parameters must be consistent with the number of format symbols and the data type represented by the format symbols.

If the types are inconsistent, type matching must be possible through implicit conversion. 

For example, if the% d symbol indicates formatting an integer type, the argument is automatically converted to an integer when it is passed as a floating-point or boolean type. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574568062
 ```  
(2) Specify the precision of floating-point types 

When formatting a string, you can specify the precision of a floating-point decimal. Format notation: 

%m.n f 

M refers to the minimum total width of the display, including the following decimal point. If the width of the formatted content is less than m places, spaces will be filled in the formatted output. N refers to the number of digits displayed after the decimal point, and when the number of digits after the decimal point is greater than n, it will be rounded. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574568062
 ```  
(3) Special formatting symbol:% s  

When formatting a string, if the format symbol is% s, it will be formatted as string regardless of the data type of the format parameter. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574568062
 ```  
##  9.4.4 format using the format method 

When using the format method of string type to format, there are two main methods: 

>  (1) Position placeholder

(2) Keyword placeholder 

The so-called position placeholder refers to specifying the output position of the formatting parameter by the position number, and the position is specified in the form of {index}. For example, in string "{0} {1} {2}", index 0 corresponds to the first parameter in the format method, index 1 corresponds to the second parameter in the format method, and so on. 

For keyword placeholders, it is necessary to explain in detail after learning the dictionary type. 

The basic syntax of keyword placeholders: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574568062
 ```  
The {} symbol in the string to be formatted is required, and the index is numbered from 0 to specify the position of the parameter in the format method. When no position is specified in {}, it is automatically formatted according to the parameter position in the format method. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574568062
 ```  
Code explanation: 

>  (1) In the code example, {0} corresponds to the "Wishful Bride" parameter in the format method, and {1} corresponds to the "Wishful Langjun" parameter in the format method.

(2) When no position is specified in {}, it corresponds to the order (left-to-right) of the arguments in the format method. 

##  9.4.5 knowledge points 

>  (1) String formatting refers to the output of strings in a specific format.

(2) There are two ways to format a string, one is through the format symbol, and the other is through the format method of the string type.

(3) Format parameters must be consistent with the number of format symbols and the data type represented by the format symbols. If the types are inconsistent, type matching must be possible through implicit conversion.

(4) Format using the format method, mainly placeholders and keyword placeholders 

##  Learn Python 9.4.6 System 

>  About the French fries teacher: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. French fries teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning, quantitative investment. 



--------------------------------------------------------------------------------

directory 

12.1.1 understand dictionary types 

12.1.2 type name of the dictionary 

Definition of 12.1.3 Dictionary 

12.1.4 traverse the dictionary in a loop 

12.1.5 key type of dictionary 

12.1.6 knowledge points 

Learn Python 12.1.7 System 

##  12.1.1 understand dictionary types 

In our daily lives, we are often exposed to the data type "dictionary", such as the directory structure of a book, in which you can quickly turn to a specified page by looking up the page number. 

>  If there is no such page number, then we must start from the first page of the book and look it up page by page. Once you have the page number, you can directly turn to the specified page. In Python, you can do a quick search through a dictionary. 

The dictionary type in Python is a collection of data enclosed by the {} symbol, and the elements in the collection are separated by English commas. 

![avatar]( 7c74d227a5e5988214318ba7de2e4321.png) 

The element "in the dictionary is a key-value pair: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574592053
 ```  
In the above code, a dictionary type variable book is defined. There is only one element in book. The elements are separated by the English colon:. The one to the left of the colon is the key name, and the one to the right of the colon is the key value. The key name in book represents the name of the chapter directory of the book, and the key value represents the page number of the chapter directory. The key name in the dictionary is unique, just like in a book, the same directory does not appear. 

>  Key names in dictionaries are unique, and multiple identical element values can be stored in lists and tuples. 

##  12.1.2 type name of the dictionary 

In interactive mode, output the type name of the dictionary via type: 

>  > > > book = {"Chapter 12 - Thoroughly Mastering Python's Dictionary Types": 210}

> >> type(book)

<class 'dict'> 

From the output, the type of the dictionary is named dict. 

##  Definition of 12.1.3 Dictionary 

To define the dictionary, there are mainly object definition method and direct definition method. 

(1) Object definition method 

The type name of the dictionary is dict, and you can directly execute help (dict) in interactive mode to find the definition and usage of dict: 

>  class dict(object)

|  dict() -> new empty dictionary

|  dict(mapping) -> new dictionary initialized from a mapping object's

|      (key, value) pairs

|  dict(iterable) -> new dictionary initialized as if via:

|      d = {}

|      for k, v in iterable:

|          d[k] = v

|  dict(**kwargs) -> new dictionary initialized with the name=value pairs

|      in the keyword argument list.  For example:  dict(one=1, two=2) 

From the output of the interactive mode, you can see the following four constructors that define the dictionary: 

>  (1) dict()

(2) dict(mapping)

(3) dict(iterable)

(4) dict (**kwargs) 

1.dict() 

Use dict () to construct an empty dictionary. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574592053
 ```  
2. dict(mapping) 

Use the (key, value) key-value pairs in the mapping object to construct a dictionary object with values. A mapping object is a mapping object from key names to key values. In Python, you can construct an object in the mapping format by using the zip type, and pass two iterables to the zip constructor, for example: zip (iter1, iter2). The iterable object iter1 on the left represents the key name, and the iterable object iter2 on the right represents the key value. The key name in iter1 corresponds to the key value in iter2 one-to-one. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574592053
 ```  
The dictionary type in Python is a standard mapping object, and we can pass a dictionary object in the dict method to construct a dictionary. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574592053
 ```  
3. dict(iterable) 

The iterable here represents an iterable object. An iterable object stores each key-value pair. The key-value pairs are stored in the iterable object in the form of a list or tuple. An iterable object can be either a list or a tuple. When an iterable object is a list: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574592053
 ```  
When an iterable is a tuple: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574592053
 ```  
Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574592053
 ```  
4.dict (**kwargs) 

This construction method is to directly use the keyword parameter form of name = value to construct the dictionary. Name represents the key name, value represents the key value, name must comply with the rules of variable names, and value must be a legal data type in Python. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574592053
 ```  
(2) Direct definition method 

Direct definition refers to the definition directly through the dictionary alias symbol {}. In {}, key-value pairs are separated by English commas. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574592053
 ```  
##  12.1.4 traverse the dictionary in a loop 

A dictionary is an iterable object that traverses the dictionary's key names in a for loop. Traversing the dictionary's for loop structure: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574592053
 ```  
Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574592053
 ```  
##  12.1.5 key type of dictionary 

The data type of the key name in the dictionary must be a static data type. Why the key type in the dictionary must be a static data type will be explained in detail in Section 12.4. In this section, students only need to master the basic concepts of the dictionary and the definition method. 

>  The static data types I have learned so far are simple data types, strings, and tuples 

##  12.1.6 knowledge points 

>  (1) The dictionary type in Python is a collection of data enclosed by the {} symbol, and the elements in the collection are separated by English commas.

(2) The elements in the dictionary are key-value pairs separated by:, and the key-value pairs are separated by commas

(3) The type name of the dictionary is dict, which can be defined by object definition and direct definition

(4) List, tuple is a linear sequence structure.

(5) The dictionary is also an iterable object, and the key name of the dictionary can be directly traversed in the for loop 

##  12.1.7 the most powerful small class training 

>  About the French fries teacher: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. French fries teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning, quantitative investment. 



--------------------------------------------------------------------------------

directory 

13.1.1 understand collection types 

13.1.2 type name of the collection 

Definition of 13.1.3 collection 

13.1.4 traverse the collection in a loop 

13.1.5 the output order of the elements of the collection 

13.1.6 knowledge points 

Learn Python 13.1.7 System 

##  13.1.1 understand collection types 

The collection type is very similar to the dictionary type. The collection type in Python is also a data collection enclosed by the {} symbol, and the elements in the collection are separated by English commas. 

![avatar]( 551b0608e9b1d4588d2c6c665693e6ac.png) 

Collections, like dictionaries, are based on hash tables. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574591474
 ```  
The above code defines a collection type variable stars, which contains two elements in stars. The elements in the collection are equivalent to the key names in the dictionary, that is, the collection type in Python is the data collection of key names. Since a collection in Python is a data collection of key names, the elements in the collection must be static and hashable data types, which we can verify in interactive mode: 

>  > > > stars = {"Chen Farong", "Chen Derong", ["Li Jiaxin"]}

Traceback (most recent call last):

 File "<stdin>", line 1, in <module>

TypeError: unhashable type: 'list' 

As can be seen from the output, when defining a variable of collection type, the Python interpreter throws an exception message with the wrong type because the element contains a mutable data type (list). 

##  13.1.2 type name of the collection 

In interactive mode, output the type name of the collection via type: 

>  > > > stars = {"Chen Farong", "Chen Derong"}

> >> type(stars)

<class 'set'> 

As can be seen from the output, the type name of the dictionary is set. The key names in the collection are also unique. After explicitly typing the list, duplicate elements can be automatically removed: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574591474
 ```  
##  Definition of 13.1.3 collection 

There are object definition method and direct definition method to define a set. 

(1) Object definition method 

The type name of the collection is set, and you can directly execute help (set) in interactive mode to find the definition and usage of set: 

>  class set(object)

|  set() -> new empty set object

|  set(iterable) -> new set object

|

|  Build an unordered collection of unique elements. 

From the output of the interaction pattern, you can see the following two constructors that define collections: 

>  (1) set()

(2) set(iterable) 

1.set() 

Use set () to construct an empty collection. 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574591474
 ```  
2. set(iterable) 

The iterable here represents an iterable object. The elements in the iterable object must be of immutable data type, otherwise an exception message of wrong type will be thrown. Iterable objects learned so far: string, list, tuple, dictionary, collection 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574591474
 ```  
Elements in an iterable object must be of immutable data type, otherwise an exception message of type error is thrown: 

>  > > > stars = ["Chen Farong", "Chen Derong", ["Chen Farong", "Chen Derong"]

> >> stars = set(stars)

Traceback (most recent call last):

 File "<stdin>", line 1, in <module>

TypeError: unhashable type: 'list' 

Simple data types, strings, tuples are all immutable data types, while lists, dictionaries, collections, etc. are mutable data types. 

(2) Direct definition method 

Direct definition refers to the definition directly through the alias symbol {} of the collection. In {}, key names are separated by English commas. 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574591474
 ```  
##  13.1.4 traverse the collection in a loop 

A collection is an iterable object that traverses the key names of the collection in a for loop. 

Traverse the for loop structure of the collection: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574591474
 ```  
Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574591474
 ```  
##  13.1.5 the output order of the elements of the collection 

Before Python 3.6, the output order of the keys in the dictionary was unordered. After 3.6, the output order of the keys was the same as the insertion order of the elements. But the output order of the keys of the collection is still unordered. 

Code example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574591474
 ```  
Collections in Python are also implemented based on hash tables, and the output order of keys depends on the underlying data structure. 

##  13.1.6 knowledge points 

>  The collection type in Python is a collection of data enclosed by the {} symbol, and the elements in the collection are separated by commas.

(2) The elements in the collection are equivalent to the key names in the dictionary, and the element type must be a static data type.

(3) The type name of the collection is set, and the dictionary can be defined by object definition and direct definition

(4) The collection is also an iterable object, and the key name of the collection can be directly traversed in the for loop 

##  Learn Python 13.1.7 System 

>  About the French fries teacher: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. French fries teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning, quantitative investment. 



--------------------------------------------------------------------------------

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



--------------------------------------------------------------------------------

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



--------------------------------------------------------------------------------

directory 

3.2.1 von Neumann system 

3.2.2 Processor Structure 

3.2.3 memory hierarchy 

3.2.4 knowledge points 

3.2.5 system to learn Python 

##  3.2.1 von Neumann system 

Computers are essentially electronic devices that cannot understand human language instructions. In order to enable such electronic devices to perform certain calculations according to human will, scientists have conceived many theories. The most famous of these is the "von Neumann system". In the von Neumann system, computer hardware consists of five parts: arithmetic units, controllers, memory, input devices, and output devices. The data and instructions processed by the computer are represented by binary numbers. The von Neumann system is shown in the following figure: 

![avatar]( 23f3ed19ef30875d76f8a4267ef161fe.png) 

Modern computers are developed on the basis of the von Neumann system, and understanding their components helps to establish a comprehensive understanding of computers. 

(1) Input devices and output devices 

Input and output devices are also known as I/O devices. 

>  I in IO is the first letter of the English word Input, which means input, and O is the first letter of the English word Output, which means output. IO together is input and output. 

Input devices are used to receive user input and transmit it to a computer. Common input devices include the following: 

Mouse, keyboard, camera. 

The output device is the end point device of the computer, which is mainly used to output and display data. The monitor is the most common type of output device. 

(2) arithmetic unit and controller 

The arithmetic unit and the controller form the core of the computer. The CPU in modern computers includes both the arithmetic unit and the controller. The arithmetic unit is used to perform arithmetic calculations and logic operations, and the controller is used to control the various components to work together. 

>  The basic arithmetic operations are addition, subtraction, multiplication and division, and the logical operations are also called Boolean operations. In logical algebra, there are three basic logical operations: and, or, and non. 

(3) Storage 

Memory, as the name suggests, is used to store information in a computer. Memory in a computer can be divided into main memory and external memory according to its function. Main memory is commonly referred to as memory, which is used to store currently active programs and data, with fast read and write speed and small capacity. External memory is used to store programs and data that need to be stored for a long time, with slow read and write speed and large capacity. The main memory cannot store data permanently. After the machine is powered off, all the information in the main memory will be lost. For persistent storage, data needs to be written to external memory. Common external memory devices: 

>  Hard disks, tapes, USB flash drives and CDs 

##  3.2.2 Processor Structure 

The processor in a computer is commonly referred to as the CPU. CPU is the abbreviation of Central Processing Unit, which means Central Processing Unit, which is the computing core and control core of the computer. The CPU can be logically divided into three modules: Control Unit, Operation Unit and Storage Unit. Each unit is connected by an internal bus. The logic structure of the CPU is shown in the following figure: 

![avatar]( 809c64b82fcb6b4941655384ad034ca5.png) 

(1) Control Unit 

The Control Unit is the command and control center of the CPU, which is mainly composed of a program counter PC, an instruction register IR, an instruction decoder ID, and an operation controller OC. 

![avatar]( e93f1b30b3f44bdc0836f9adb0a07fcf.png) 

The program counter contains the address of the instruction to be executed. When the instruction is fetched by the CPU, the storage address in the program counter is incremented, and the program counter points to the next instruction in the instruction sequence. 

The core task of the CPU is to execute the instructions in the program, and the instructions and data in the program are stored in memory. The program counter initially points to

For the first instruction in the sequence, the CPU obtains the address of the first instruction from the program counter, and then reads the instruction from the memory and executes it.

When the CPU executes an instruction, it synchronously modifies the contents of the program counter so that the program counter always points to the next instruction to be executed.

Computer programs are executed in this manner.

After the CPU fetches the instruction from memory, it places it in the instruction register, and then decodes the instruction through the decoder to determine what operation to perform. 

Program instruction is composed of operation code and address code. It decodes the instruction, that is, extracts the operation code and address code in the instruction.

The opcode indicates which operation to perform, and the address code indicates the address where the operand is stored.

For example, the addition operation 1 + 2 has operands 1 and 2, and the opcode indicates that an addition operation is required.

After the instruction is decoded, the operation controller generates various operation control signals according to the operation code and timing signal of the instruction, thus completing the control of the instruction acquisition and execution of the instruction. 

(2) Storage unit 

It is composed of the on-chip cache and register group in the CPU, which is a unit for the CPU to temporarily store data, which stores data waiting to be processed or has been processed. 

(3) Operating unit 

The core of an arithmetic unit used to perform arithmetic and logic operations. 

##  3.2.3 memory hierarchy 

Registers are the basic storage unit of the CPU, and the CPU takes much less time to access registers than memory access. To reduce the number of times instructions and data are read from memory, a cache is introduced between the CPU and memory. Similarly, memory reads and writes much faster than disk reads and writes. To reduce the number of disk reads and writes, read and write buffers are introduced into computer memory. These memories are organized into a pyramid-shaped hierarchy in the logical structure of the computer according to their access speed and capacity: 

![avatar]( 05e7c3bd40fa40cf7f13a58f3b93a067.png) 

It can be seen from the figure that the access speed of the register is the fastest, and the access speed of the external memory is the slowest. From the perspective of the size of the capacity, the storage capacity of the register is the smallest, while the storage capacity of the external memory is the largest. 

The hierarchical structure of memory shows that although fast storage devices are fast, their capacity is small, and slow storage devices are slow to read and write.

But the storage capacity is large. According to this idea of memory hierarchy, fast storage devices can be used as caches for slow storage devices,

For example, the cache is used as a cache for memory, and the memory is used as a cache for disk.

How to use caching to improve program performance is a core technology that programmers must master, and will be explained in detail in subsequent chapters.

##  3.2.4 knowledge points 

>  (1) Computers are essentially electronic devices that cannot understand human language commands

(2) In the von Neumann system, computer hardware consists of five parts: arithmetic unit, controller, memory, input device, and output device.

(3) Main memory is commonly referred to as memory, which is used to store currently active programs and data, with fast read and write speed and small capacity. External memory is used to store programs and data that need to be stored for a long time, with slow read and write speed and large capacity.

(4) The processor in a computer is commonly referred to as the CPU. CPU is the abbreviation of Central Processing Unit, which means Central Processing Unit, which is the computing core and control core of the computer. The CPU can be logically divided into three modules: Control Unit, Operation Unit and Storage Unit. 

##  3.2.5 system to learn Python 

>  Fries Teacher Profile: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. Fries Teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning 



--------------------------------------------------------------------------------

directory 

5.2.1 build a holistic understanding 

5.2.2 core parts of the Python language 

5.2.3 system to learn Python 

##  5.2.1 build a holistic understanding 

When learning programming for beginners, beginners must first establish an overall understanding of the knowledge they have learned, learn its skeleton, and then explore the details. After establishing an overall understanding and understanding its general structure, they will roughly know what to learn in this programming language. How well you learn, see the real chapter from the details. The details of knowledge can be seen that a person's foundation is not solid. Take variables in Python as an example, most beginners know how to define a Python variable. What are the variables, and ask their essence, but few beginners can answer. 

##  5.2.2 core parts of the Python language 

The purpose of this section is to provide a general introduction to the core components of the Python language, and each learning component will be explained in detail in subsequent chapters. 

(1) Language foundation 

The language foundation in Python mainly covers variable definitions, code comments, expressions, statements, etc. When learning Python, first lay the foundation of this programming language, and then build high-rise buildings. 

>  Learning is layered and a process from easy to difficult. 

(2) Process control 

Flow control mainly learns about control structures in Python. Control structures in the programming language are used to control the execution logic of code. Control structures in Python include conditional control, loop control, and steering control. 

>  In conditional control, the code in the branch is executed by judging whether the condition is true or false. In loop control, the code in the program can be executed repeatedly. In turn control, the execution process of loop structures and functions can be controlled. 

(3) Data types and functions 

When learning data types, first learn the concept of data types, understand what data types are, and then master the definition and usage of data types in programming languages. Data types in Python can be divided into simple data types and composite data types. Simple data types in Python are integer, floating point, and boolean. Composite data types in Python include string, list, tuple, dictionary, and collection. 

>  Integer, floating-point, string, and other data types are built-in data types in Python. Through classes, we can customize data types. 

Functions are also a data type. In programming, code that needs to be reused can be encapsulated into a function, so that it can be called directly the next time it is used, without rewriting. 

>  Students can understand a function as a converter from input to output. For example, a language translator is a function that outputs one language to another. 

(5) object oriented 

In Python, everything is an object. Built-in data types, functions, files, etc. are all objects. Before mastering the knowledge of object oriented, you need to understand what abstract data types are. Abstract data types are abstractions of data, and their core is to define the structure of data and how to operate on it. 

>  The so-called object refers to the instantiation of this abstract data type. In Python, this abstract data type is represented by a class type. 

(6) Document processing 

File processing in programming refers to the use of the interface provided by the operating system to read and write files. 

>  In the section on file processing, students will learn the types of files, their functions, and how to manipulate files through the open method provided by Python. 

(6) Exception handling 

Exceptions occur during program execution, and how to handle them when they occur, as well as how to customize exceptions, are the main topics to be learned in this section. 

(8) Module processing 

Modules are the core content of Python, and a Python script file corresponds to a module. 

>  In Python files, variables, functions, class types, etc. can be defined as attributes of the module. In Python, other modules can be imported inside the module through the import statement. In the actual development process, commonly used attributes and functions can be written into a separate module for use by other modules, thus realizing reuse. 

(9) Concurrent programming 

The concurrent execution of a program refers to having multiple execution units execute simultaneously or alternately to improve overall performance. 

>  In concurrent programming in Python, we will learn the concepts of processes, threads, coroutines, and the IO model. To become a good Python backend programmer, concurrent programming is a knowledge difficulty that must be overcome. 

(10) Network programming 

The concurrent execution of a program refers to having multiple execution units execute simultaneously or alternately to improve overall performance. In Python concurrent programming, we will learn the concepts of processes, threads, coroutines, and the IO model. To become a good Python backend programmer, concurrent programming is a knowledge difficulty that must be overcome. 

(11) Log processing 

Log processing in a program refers to recording the running process of the program and user behavior to a log file to facilitate later error troubleshooting and data statistics. 

(12) unit test 

After the program is developed, as a qualified programmer, you need to perform unit tests on the code. 

>  Unit test refers to the inspection and verification of the smallest unit in the program to test whether the function provided by the unit is correct. Usually a function in Python is used as a minimum test unit. 

(13) Standard Library 

The standard library in python is a built-in module in python. The python standard library is very large, and we only need to learn a few commonly used standard libraries. 

>  System related standard library, time processing standard library, command line related standard library, mathematical processing standard library, data persistence standard library 

##  5.2.3 system to learn Python 

>  Fries Teacher Profile: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. Fries Teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning 



--------------------------------------------------------------------------------

directory 

6.2.1 expressions in human language 

Expressions in 6.2.2 Programming Languages 

6.2.3 statement is an execution process 

6.2.4 system to learn Python 

##  6.2.1 expressions in human language 

In daily life, people often express their feelings through words. Saying "I miss you" or "I like you" is used to directly express love for a lover. "Break up!", "Go away!", "I don't love you anymore" may mean the end of a relationship. Exporting human language through the medium of words enriches the form and meaning of language expression. The following is quoted from the inscription of Tang Xianzu's "Peony Pavilion": 

I don't know what to do, go deeper, the living can die, and the dead can live.

Those who are born but cannot die, and those who die but cannot be resurrected, are not the surest feelings. 

From the text description of the inscription and the tortuous love told in the script, the reader can personally agree with the author's point of view expressed in the opening passage: 

"Women in the world have feelings, not as good as Du Liniang". 

Whether it is an "expression of love" or an "expression of frustration", information is output through language or writing. People can feel the information conveyed from language or writing in the process of listening and reading. 

##  Expressions in 6.2.2 Programming Languages 

(1) The expression has output 

Expressions in programming languages have one thing in common with expressions in human languages: output information. For example, the arithmetic expression "1 + 1" expresses the calculation process of adding 1 and 1, and the output value is 2. The relational operation expression "1 > 1" expresses whether 1 is greater than 1, and the output value is false. 

(2) Common expressions 

Key expressions in programming languages: 

When introducing data types later, we will explain expressions and operators in Python in detail. This section focuses on providing students with an understanding of the concept of expressions. 

Expressions in programming languages can be combined with each other. Any complex expression is composed of simple expressions, and eventually a value is output. When encountering a complex expression, students should learn to decompose the complex expression, calculate the value of each subexpression, and finally convert it into a simple expression. Examples of complex expressions: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957459195
 ```  
The complex expression is broken down first. The expression (number + 1 > 2) and (0 or 1) consist of two subexpressions: 

>  1.(number +1 > 2) 2.(0 or 1) 

In the subexpression number + 1 > 2, the value of number + 1 is evaluated first, and the result is 2. The value of the expression 2 > 2 is false. The subexpression 0 or 1 is a logical expression. 

>  Students should note that in Python, 0 values represent false values, while non-0 values represent true values. 

In the logical OR operation, as long as one of the logical values is true value, the operand of the true value is output, so the value of the expression 0 or 1 is 1. Finally, the values of each subexpression are combined, then the expression (number + 1 > 2) and (0 or 1) are equivalent to "false and 1". In the logical AND operation, as long as one of the logical values is false, a short circuit is triggered, and the operand of the false value is output, so the final value of the expression is "false". 

Expressions in Python will be explained in detail later in the introduction to flow control. This section focuses on enabling students to understand the basic concepts of expressions 

(3) The value of the output expression 

Print is a built-in function in Python that can output the value of an expression to the end point. Basic usage of the print function: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957459195
 ```  
Value represents the value of an expression and can output the values of multiple expressions simultaneously, separated by commas. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957459195
 ```  
##  6.2.3 statement is an execution process 

(1) Conditional control statements 

A statement in a programming language expresses an execution process, usually without output. Take the conditional control statement in Python as an example, which controls the execution process of the code according to the value of the expression. Please take a look at the following Python code first: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957459195
 ```  
Python is an interpreted language that linearly executable code instructions from top to bottom. The output of the final program is: 

happy

unhappy 

>  Students can write the example code to the script file, and then execute the script through pycharm or vs code. Students who are not familiar with IDEs can review the content introduced in Chapter 2 first. 

The conditional control statement in Python is a structure that implements logical control through the if statement. The basic syntax form of the conditional control structure: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957459195
 ```  
Expression represents an expression, and the if statement will determine whether to execute the code below: based on the output of the expression. If the value of the expression is true, the code below the colon will be executed, otherwise it will not be executed. Else expresses that if the value of the expression in the if statement is false, the code below the colon of the else statement will be executed. 

>  If means if, which means what kind of operation to perform if something happens, and else means otherwise, that is, if the conditions specified in the if statement are not satisfied, the corresponding operation will be performed. 

Now rewrite the above code through conditional control, and rewrite the code: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957459195
 ```  
The output of the program is: 

happy 

In the rewritten code, the value of the expression state == 0 is true, because the value pointed to by the variable state is 0, 0 is equal to 0, and the output is true. So the code below the if statement colon is executed: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957459195
 ```  
Therefore, the final output value through the print function is happy. 

(2) Empty statement 

In Python, pass is used to represent an empty statement. An empty statement, as the name implies, does not contain any statements. An empty statement is used to maintain the integrity of the program structure and acts as a placeholder. 

##  6.2.4 system to learn Python 

>  Fries Teacher Profile: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. Fries Teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning 



--------------------------------------------------------------------------------

directory 

6.3.1 understand code comments 

6.3.2 code comment notation 

6.3.3 file encoding comments 

6.3.4 system to learn Python 

##  6.3.1 understand code comments 

In the process of writing a program, comments are usually written to describe key code or complex logic in the program. Code comments are for programmers, that is, they are for programmers to see. The Python interpreter skips the comments in the code when interpreting the instructions in the execution program. 

>  Students should develop the habit of writing code comments at the beginning of learning programming, and record the key logic in the program through text description. This way, in the process of reading later, you can understand the key logic in the program through comments. Of course, don't over-comment, otherwise it will affect the overall readability of the code. 

##  6.3.2 code comment notation 

The comment symbol in Python has three quotation marks in English: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590038
 ```  
And the English #symbol: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590038
 ```  
The #symbol is used for single-line comments, and for multi-line comments in Python, you need to use a pair of English three-quote marks "'" or "", and the content of the comment is enclosed in the three-quote marks. Code examples for multi-line comments using three quotes: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590038
 ```  
The Python interpreter skips comments in the code when interpreting the execution of the script. For the Python interpreter, the code in the program is equivalent to the following form (without any code comments): 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590038
 ```  
##  6.3.3 file encoding comments 

Python source program files are text files. Text files are files composed of text characters. The so-called file encoding refers to the character encoding method in the text file. In Python version 2.X, the default character encoding is ASCII encoding. If non-ASCII characters (such as Chinese characters are non-ASCII characters) are used for comments, Python will throw syntax error exceptions when executing the script. 

>  Computers can only process binary. In order for computers to recognize characters, they need to be represented by a specific number code. Students who are not familiar with this can review the content in Section 5.1. 

ASCII encoding is a character encoding specification in which a maximum of 256 characters can be represented. Interested students can consult relevant materials to see the characters supported by ASCII encoding. In Python version 3.X, the default character encoding of a file is utf-8 encoding, and other characters such as Chinese characters can be used directly in the code for comments. By specifying an encoding comment in the file header, the Python interpreter will decode the content of the file according to the specified encoding method. Encoding comments are mainly written in the following two ways: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590038
 ```  
encoding_name indicates the specific character encoding, for example, specify the encoding according to the gbk encoding, which is written as: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590038
 ```  
The version used in this tutorial is Python 3.11.0, and there is no need to specify the encoding method of characters in the file header. For the Python 2.X series version, students can specify utf-8 encoding in the file header: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574590038
 ```  
GBK encoding, UTF-8 encoding and ASCII encoding are all character encoding standards. Students who are interested can refer to relevant materials and take the main encoding standards of characters as a learning topic after class. 

##  6.3.4 system to learn Python 

>  Fries Teacher Profile: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. Fries Teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning 



--------------------------------------------------------------------------------

As a practical tool for dealing with strings, regular expressions are often used in Python, such as crawlers Crawling the data to retrieve strings and so on. Regular expressions are already embedded in Python and can be used by importing the re module. As newbies to Python, most of them have heard of the term "regular". 

Today, I would like to share with you a more detailed collection of Python regular expressions. After learning it, you will become proficient in regular expressions. 

![avatar]( b0f3f391f36c4c4186afb0c767449760.jpg) 

###  The re-module 

Before we talk about regular expressions, we must first know where to use regular expressions. Regular expressions are used in the findall () method, and most string retrievals can be done through findall (). 

1. Import the re module. Before using the regular expression, you need to import the re module. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
2. the syntax of findall (): 

After importing the re module, you can use the findall () method, so we must be clear about the syntax of findall (). 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
It is not difficult to see that findall () is composed of a regular expression and a target string. The target string is what you want to retrieve, so how to retrieve it is performed through a regular expression, which is our focus today. 

The result returned after using findall () is a list of strings that meet the regularization requirements 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

###  Second, regular expressions 

1. Ordinary characters, most letters and characters can be matched by themselves. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
2. Metacharacters 

Metacharacters refer to special characters such as .^ $ ?+ {} \ [], through which we can personalize the search of the target string and return the result we want. 

Here I will introduce to you 10 commonly used metacharacters and their usage. Here I will give you a simple summary for easy memorization. The following will explain the use of each metacharacter one by one. 

![avatar]( 8c37aa9d37e14e9880b384e5b85721e3.png) 

（1） [] 

[] 的使用方式主要有以下三种： 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
The output is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
For example, to select the abc element in the string "abcabcaccaac": 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
The output is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
For example, to select "caa" in the string "caabcabcaabc": 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
The output is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Note: When in the first position of [], it means that everything except a is matched, such as changing the position of a in []: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
（2）^ 

^ is usually used to match the beginning of a line, for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
![avatar]( 724785f6d8f5422e8c52eaef8b552226.jpg) 

>  Fan exclusive benefits 

(3) $$is usually used to match the end of a line, for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
![avatar]( 8ca641e45b994987a9a23ba070981eee.jpg) 

（4）\ 

After the backslash, different characters can be added to represent different special meanings. Common ones include the following three. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
The output is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
\ can be escaped into normal characters, for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Match any whitespace characters such as: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Matches any alphanumeric and underscore, equivalent to [a-zA-Z0- 9_], for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
![avatar]( 1e9ee27672ed489dafb11d1c71a02a02.jpg) 

（5）{n} 

{N} can avoid repeated writing. For example, we wrote\ w 3 times when we used\ w earlier, but here we need to use {n}. N represents the number of matches, for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
（6）* 

* Means zero or more matches (as many as possible), for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
**（7） + ** 

+ means match one or more times, e.g. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
（8） . 

. is a dot, which is not obvious here. It is used to manipulate any character other than a newline character, such as: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
(9) ？ 

? means one match or zero 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Pay attention to greedy and non-greedy patterns here. 

Greedy pattern: Match as much data as possible, expressed as\ d followed by a metacharacter, such as\ d *: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Non-greedy mode: Match as little data as possible, expressed as\ d followed by?, such as\ d? 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
The output is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
(10) {m, n} m, n refers to a decimal number that is repeated at least m times and at most n times, for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Add? means to match as little as possible 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
There are other flexible ways to write {m, n}, such as: 

![avatar]( 14d7db206f8943418d2a43026521c828.jpg) 

Regarding the commonly used metacharacters and how to use them, let's take a look at the other knowledge of regular rules. 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

###  (2) The use of regular rules 

1. Compile regular 

In Python, the re module can compile regulars through the compile () method, re.compile (regular expression), for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
2. How to use regular objects 

The use of regular objects is not only through the findall () method we introduced earlier, but also through other methods. The effect is different. Here is a simple summary: 

(1) findall () finds all strings that re match and returns a list 

(2) search () scans the string to find the position where the re matches (just the first one found) 

(3) match () determines whether re is at the beginning of the string (matches the beginning of the line) 

Let's take the example of the object returned by compile () after compiling the regular. Instead of findall (), let's use match () to see how the result is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
It can be seen that the result is a match object, the starting subscript position is 0~ 13, and the match is 010-123456789. Since the object is returned, let's talk about some operation methods of this match object. 

![avatar]( 511fa5bb3d9e404398729084f797a7d6.jpg) 

>  Fan benefits 

3. Match object operation method 

Here are the methods first, and I will give examples later. Common methods of using Match objects are as follows: 

(1) group () returns the re-matched string 

(2) start () returns the starting position of the match 

(3) end () returns the position where the match ends 

(4) span () returns the position of a tuple: (start, end) 

Example: Use span () to operate on the object returned by search (): 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
The result is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Functions 4.re module 

In addition to the findall () function introduced above, there are other functions in the re module to provide an introduction: 

(1) findall () returns all the strings that match according to the regular expression. I won't say much about this. I have introduced it earlier. 

(2) sub (regular, new string, original string) The function of sub () is to replace the string, for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
(3) subn (regular, new string, original string) The function of subn () is to replace the string and return the number of replacements 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
(4) split () split () split string, for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
![avatar]( 1b31fa941d2944b8a9131f06c72a5cd8.jpg) 

Regarding regularity, I have said so much. Regularity is an indispensable foundation in almost all directions of Python. I wish you all the best in your Python journey! 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

![avatar]( 884b16d55fc040289932e9f4b3d23c91.png) 



--------------------------------------------------------------------------------

From Python basics to advanced programming, basically the knowledge of Python beginners has been learned. In order to give more beginners who have learned Python beginners to advance to Python (such as crawlers/backend/data analytics, etc.), they have consolidated their basic knowledge and made a special issue on the assignment statement when Python beginners get started. 

In Python, there are many ways to assign values, such as variables, tuples, lists, and so on. Therefore, if the assignment is ambiguous, it is conceivable that the later advanced content will make it difficult for you to write code alone. 

![avatar]( 8f13285edd124748a4403be769111349.jpg) 

Don't say much nonsense, learn and learn from time to time, if there is a change, if not, encourage. 

###  Common Assignment Statements 

Let's take a look at the commonly used assignment statements in Python: 

Sequence is a general term for ordered sets. In Python, strings, lists, tuples, byte arrays, buffers, and Xrange objects all belong to different sequence types, which means that (10, 20) can be said to be either a tuple or a sequence. 

Example 1: Using a tuple to assign a value to another tuple 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
Note: The number of elements on both sides of the equal sign should be equal. If it is a, b = 10 or a = 10, 20, then an error will be reported. 

Example 2: Using a sequence to assign a value to another sequence 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
A, b is a tuple by default, and [20, 30] is a list, which can also be assigned between different sequence types. 

###  Advanced Assignment Statements 

What is a high-level assignment statement? That is, the regular assignment method will report an error, and some more advanced operations must be performed. For example, to assign the characters "SPAM" to a and b, the regular assignment is like this: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
Then after running, an error will be reported. If there are more elements in the string than in the tuple (a, b), a direct copy will report an error. 

In this case, we need to use the slicing operation to assign the value: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
In addition to slicing, we can also assign values to a and b in other ways: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
This operation is equivalent to dividing a small tuple (a, b) into a large tuple ((a, b), c), and then assigning values to a and b. 

Example: Use an assignment statement to reduce the list [1, 2, 3, 4, 5] by one element at a time and output the list. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
There is a two-dimensional list [[[1, 2, 3], [4, 5, 6], [7, 8, 9]], how to use the method of sequence assignment to output each element in the list? The method is as follows: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
(A, b, c) and's are different types of sequence types, which can also be achieved through the method of sequence assignment. 

###  III. Extended sequence unpacking 

In the previous table of common assignment statements, we talked about the extended sequence unpacking operation: 

So how should it be used? First of all, we should know what is the use of * b: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
Example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
As can be seen from this example, a is assigned to the first element, the rest are given to b, and the remaining elements are encapsulated as a list. 

Since we have mentioned above 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
So what if we add an extra element to the assignment? 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
It can be seen that an object is really set aside for c and assigned a value, which can be used flexibly. 

If we swap the positions: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
It can be seen that the last element g of the string is still assigned to a, so it is also possible to swap the position, and the a at this time will be taken from the back. 

If we only give 3 elements, but there are 4 elements to be assigned, can * b get the value? 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
The result b is an empty list, because string has only three characters, which is not enough for b. Likewise, no matter how you swap the position of * b, the result is the same, that is, other elements will be assigned first, b has the lowest priority, and sometimes the value * will not be obtained. 

We need to note that * b cannot be assigned directly: 

![avatar]( 3688c0fab7474f62b4f20092967cd9e6.png) 

The previously assigned object can only be a list or tuple sequence type, and * b alone does not belong to this type. 

How can we correct it at this time? It's simple, just turn the front into a tuple or list: 

![avatar]( 2a450c07f9b242c2a7e967355b72a150.png) 

Even with a comma, * b can be turned into a tuple. 

Then we also come to an example of the extended sequence unpacking. We still use the above-mentioned method to reduce the list [1, 2, 3, 4, 5] by one element and output the list. This time we use the method of sequence unpacking to do it: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
So in the previous high-level assignment statement, we also talked about an example of a for loop outputting a two-dimensional list, so can the for loop also use parameters with * to assign? The answer is also possible: 

![avatar]( 01d1e6671669446882c66480de12cbe7.png) 

###  IV. Multi-objective assignment 

The form of multi-objective assignment: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
This is also a point of Python's elegance. The underlying logic is that the right side of the equal sign is assigned to the left first, and the value is assigned in turn. The common first address is 1, that is to say, 10 is assigned to c first, and the value of c becomes 10. C is then assigned to b, and b is then assigned to a. Their addresses are all the same: 

![avatar]( c1862d3519944486b8ff97a5c2fb4353.png) 

###  V. Enhanced Assignment 

Enhanced assignment operations not only have +=, but we also talked about the basics: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
Their main functions are: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547809
 ```  
I won't give an example here. This is something we often use, and it's very simple. Just know that they have this effect. 

![avatar]( 1caccfde1bfc44d089d5f27fef707943.png) 



--------------------------------------------------------------------------------

Decorators (decorators) are also a very important part of Python, allowing other functions to add extra functionality without any code changes. They are equivalent to a syntactic sugar, which may be difficult for beginners to understand or understand. However, you will encounter or use them more or less later. 

![avatar]( bff125858c124b79834fbf4a65f113fb.png) 

###  The concept and function of modifiers 

A decorator, also known as a decorator, is itself a function that adds additional functionality to an existing function or method. 

In summary, the role of a decorator is to add additional functionality to an existing object. 

For example, this function is a registered function, but sometimes when the user performs this operation, he is a registered user. I have already written this function and don't want to move it. Then we can add a login function to this function through a decorator. 

It is often used in scenarios with tangential requirements, such as: insert log, performance testing, transaction processing, caching, permission verification, etc. Decorators are an excellent design to solve such problems. With decorators, we can extract a lot of identical code that has nothing to do with the function itself and continue to reuse. 

![avatar]( 52fee12ad3ed4d0890da2e167b585f5d.jpg) 

The specific operation of the decorator, let's learn it slowly. 

###  Second, the use of modifiers 

Before using decorators, we need to remember a few instructions for using them: 

(1) The keyword for a decorator is @. As long as it appears in Python code, you can think of it as a decorator. 

(2) Decorators modify functions or methods and cannot modify a class. 

(3) The decorator must appear on the previous line of the function or method being modified, and cannot be defined on the same side of the function. 

Example: 

![avatar]( a55667c8f5854d77a533af9c4ddb0fe4.png) 

Although the decorator itself is a function, its appearance is regulated. The above decorator does not appear in the first line of the modified function or method, so even the print ("Uncle Dragon") line of code cannot be executed. 

(4) The decorator itself is a function that passes the modified function as a parameter to the decorator, performs the functions in the decorator, returns the passed function object, and calls the returned function. 

These points are important, and let's deepen our understanding by exploring the various uses of decorators. 

![avatar]( 36009dafc7d84ffdaf10bfadf96d75b5.jpg) 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

If the modified function is not called, the function following @is executed, and the modified function is passed as a parameter, then the return value of the decorator function can be any value. 

Example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
First of all, we can see that this is a very simple example of using a decorator, using @dec to call the dec () decorator function, while the modified function funA () does nothing. 

Secondly, we can see that the modified function funA () does not call anything, but it is passed as an argument to the decorator function dec (), so dec () needs a parameter to accept the passed value. I used a as a parameter. If you remove a, the system will report an error, because the value returned by the modified function funA () is not accepted. You can try it. 

Finally, there is one more point, the modified function funA () has not been called, have you noticed? So the decorator function dec () returns anything, the above returns None, you can return a "sick", you can return anything, let's look at the situation where the modified function funA () is called. 

![avatar]( fd5b2f6dd50b4ab1bc121b0c379db8b7.jpg) 

If the modified function is called, execute the decorator directly and pass the modified function to the decorator as a parameter, but the return value of the decorator must be the current parameter. 

Example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
There is an error, saying that string str cannot be iterated, why? In fact, the reason is that when a decorator exists and is used, the modified function is called again. At this time, the return value cannot be any value. At this time, the decorator function can only return the passed value. You can try to change the return "sick" to return a to output normally, or you can remove the line of code funA () and do not call the Hughes function, the output is normal. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
Everything is normal. 

Let's take a look at the execution logic of the decorator again: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
From this running result, we can see that the modifier's running logic is: the modified function funA () is called, but it is not directly executed, but directly executes the modifier dec, and passes the modified function funA () as a parameter to the modifier dec, executes the code in the modifier function dec (), returns the code in the modified function funA () that is executed after passing the value a, and finally finishes the modified function funA () before executing the remaining code. 

I'll use a more sketchy diagram to illustrate this: 

![avatar]( 3da35bef75ab42c5ac3a02f6f8bdbc36.png) 

We talked about the basic uses of decorators earlier. There are many ways to use decorators, and you can also use function nesting. 

Let me demonstrate with a simple example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
From the running results, function nesting can also be carried out in the modified function. 

Closures are also a type of function, but they are relatively special. I will not repeat the knowledge about closures here. In [Python Basics], we have talked about closures. If you forget, you can take a look or Baidu. Let's take a look at how closures in modifiers are used. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
It can be seen that closures can also be used normally in decorator functions. 

![avatar]( 92eed7881d6d44dcadb8f04775ff8825.jpg) 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

If the modified function has parameters passed, the parameters can only be passed to the embedded functions in the decorator function. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
It can be seen that although the modified function C () passes parameters to the decorator function A (), the default pass is still the object C (), the decorator function A () accepts the modified function C (), and the parameters are passed to the function B () in the decorator function A (). 

Even if you add two parameters to A (), it will not accept it and will only report an error. We have already said in the instructions for the use of the decorator, "The modified function is passed to the decorator as a parameter", so the decorator function accepts only the object of the modified function. If you want to pass parameters, then there must be other functions in the decorator function to accept the passed parameters. 

If the decorator has parameters but the modified function has no parameters, you can only use the inline function to collect the parameters. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
###  Third, Python's built-in decorators 

The previous ones we talked about are all our custom decorators. In Python, there are built-in decorators. Let's learn about three common Python built-in decorators: staticmethod, classmethod, and property. 

Their function is to transform the methods in the class into static methods, including class attributes and class methods of the class. Let's take a brief look at the specific use. 

Property can change a method into a property. The modified method name must be the same as the method name below the property. Property can only be used for private properties. 

Let's make a comparison. We create a class and use the methods in the class without using properties, as follows: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
No problem, it works fine, so let's try it with the built-in decorator property to see what's different. 

Before using the built-in decorator property, we have to add a point: private properties, properties created inside the function are private properties, and cannot be used outside the function without special treatment. Private properties are represented by two underscores in front of them. For example, the __name in the class represents private properties. Let's take a look at a simple example: 

![avatar]( d688fd8ef22f4eb2ae0c3d5abf61bee8.png) 

It can be seen that private attributes can be accessed within the class, but not externally (they can be accessed after some processing, which will not be introduced here. You can check it online). 

Returning to our built-in decorator properties, in the previous example where we did not use properties, we made a modification to add the built-in decorator properties. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
From this example, we can see that the built-in decorator property can be used for private properties, and methods can be turned into properties. For example, a.age is calling properties instead of methods. Although age () appears many times in the class, it does not report an error because of method coverage. It is also because of the existence of property that the property stipulates that the modified method name must be the same as the method name below the property. 

![avatar]( a3a4a683012f4576ab60b8b2b5bd7f6b.jpg) 

The built-in decorator staticmethod is a static method whose function is to remove the modified method from the class and become an independent function, which cannot access the properties of the class. 

Let's write a simple class first and compare it with staticmethod without using it 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
There is no problem with this. Let's take a look at using the staticmethod and add it directly: 

![avatar]( b3cfd203de7f464cb13b13d7bbc5bdac.png) 

The reason for the error is that after adding @staticmethod, the eat () method becomes an ordinary function. Although its position is in the class, it is actually equivalent to an ordinary function, not a class method. Therefore, you have to pass a value to it, otherwise the parameter self will not be passed and the error will be reported. 

The correct writing should be: 

![avatar]( b67ef6dcacb7404ebe62a0211bd7fe9b.png) 

Let's summarize this staticmethod: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
The difference between a method decorated with classmethod and an instance method is that the first parameter received is not self, but cls (the concrete type of the current class). The modified method cannot access instance properties, but can access class properties. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
From the results, it can be seen that from the objects printed by sleep () and eat (), the object passed by sleep () is the instance object b created, while the function eaten () modified by the decorator passes the class; from the point of view of eating () accessing the properties and instance properties of the class, there is no problem accessing the properties of the class, but an error is reported when accessing the properties of the instance object. 

Therefore, it is verified that the method modified by classmethod is different from the instance method in that the first parameter received is not self, but cls (the specific type of the current class). The modified method cannot access the instance properties, but it can access the class properties. 

~ 

Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574547107
 ```  
From the results, it can be seen that from the objects printed by sleep () and eat (), the object passed by sleep () is the instance object b created, while the function eaten () modified by the decorator passes the class; from the point of view of eating () accessing the properties and instance properties of the class, there is no problem accessing the properties of the class, but an error is reported when accessing the properties of the instance object. 

Therefore, it is verified that the method modified by classmethod is different from the instance method in that the first parameter received is not self, but cls (the specific type of the current class). The modified method cannot access the instance properties, but it can access the class properties. 

Today's sharing is here, welcome to leave a message in the comment area! 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 



--------------------------------------------------------------------------------

###  👳foreword 

![avatar]( b7a326896f11470bada3568966c81743.png) 

 This is the fourth installment of the novice tutorial. The previous installment of Python's basic introduction, object oriented programming, and regularization has been published. Today's content is Python modules and packages. If you haven't read the previous tutorial, you can go back and read it when you have time. Welcome to subscribe to my column. The articles in this series will be placed in the column, and you can learn any direction of Python without barriers. 

>  Python beginner tutorial column 

Modules and packages are used frequently in Python. The reason why Python has a small amount of code and a fast development speed is that modules and packages occupy a large proportion. This is also a skill that beginners must master in advanced crawling, data analytics, web development, and other directions. 

###  👳Module 

Module refers to Python's program files (source files). The file name of the module is the module name plus .py, which contains Python object definitions and Python statements. Module contains defined functions, classes, and executable code, etc. Generally, do not modify the module to avoid module failure. 

In Python, module calls are allowed in the form of imports. Modules in Python are also objects. All global variables defined in a module become attributes of the module after import. 

1. Syntax 1: import module name 

If you want to import multiple modules, you can use only one import to import multiple modules, separated by commas, but in Python's PEP8 style, this is not recommended, so if you want to import several modules, write several imports to import them one by one. 

Example: Import the math module and call the function of sqrt () to square 9 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
As a reminder, operations in Python return a float type by default, so it is 3.0. 

Syntax 2: import function 1 from module name, function 2 

Note that the functions here are not followed by parentheses. 

Example: Import the math module and call the function of sqrt () to square 9 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
3. Syntax 3: import from module name 

Under normal circumstances, this syntax can import all the functions of a module. When you want to use multiple functions of a module, you don't need to write them one by one. I won't give an example here. They are all the same. 

Attention: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Example: (This example requires reading the following custom module to understand) 

A new module called module1 has been created, and the module code has two functions: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Import all the methods in the module using Syntax 3 in another Python file: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
The execution result is only printed out fun1, and then an error is reported, indicating that fun2 () is not defined and cannot be recognized. This is because 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

Some modules or function names within the module are relatively long, which is inconvenient when used multiple times. You can customize the name of the module or function. 

1. Module custom alias: import module name as alias 

Example: Customize the time module to alias t and use it. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
After 3 seconds of execution, the program outputs: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
2. Function custom alias: import function name as alias from module name 

Example: Import the time module and customize the sleep () function to the name s 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
After 5 seconds of execution, the program outputs: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Everyone can generate custom modules to call. Custom modules are Python files, and the Python files created when we write code are equivalent to one module. 

Note: The called module should be placed in the same directory as the current Python file as much as possible, otherwise the folder must be declared before importing. 

Example: Customize a module and call it in another Python file. 

Create a new Python file named module1 with the following code: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Create another Python file in the same directory and call module1.py this module: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Running the current Python file results in: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Each module is executed by default when it is imported, but at the same time there is a lot of dogfooding code inside the module. In order to avoid executing the test code inside the module when importing the module, a method is involved: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
This method can realize a function, if executed in the module, the code of executable code 1 will not be executable code 1 when other files are imported into the module, so the tests inside the general module are placed in the code 1. 

The magic point is that __name__, the result of its execution in the current file is __main__, and the result of execution when other files are imported is the module name, so take advantage of this, use the if statement to determine whether the module is executed in the current file or is imported. 

Example: 

Create a new Python called module1 as a module with the following code: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Execution result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Create a new Python file and import the module1.py module you just built: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Execution result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
The result is different when the current file is executed and when it is imported, so it becomes the dogfooding method of the module. 

Note: In the custom module, it is not recommended to write while cycle, otherwise the while cycle in the module has been executed during the import process, and it may not jump out, that is, the module has been imported, and other code cannot be executed. 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

###  👳II. Package 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Features of the package: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Create a new project file in the Pycharm software. After the creation is completed, open Pycharm to create a project folder → click the folder → right-click the pop-up option → New → Python Package → complete the creation. The new folder created is the package, and the init file is automatically created in it. 

![avatar]( 9c11db668a044f929f462dee134c57d5.png) 

There are two main types of conventional import methods. 

Method 1: import package name. module name. target 

Method 2: import package name, subpackage, module name, target 

The targets mentioned here can be variables, functions, and other objects, as will be discussed below. 

Form of use 1: Regular use 1 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Example: Create a package and use it in another .py file, requiring that the .py file not be included in the created package. 

Step 1, open Pycharm to create a new project, create a package, named demo, create a new .py file in the package, named my_module, the code is as follows: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Step 2, open another .py file and import the created package 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Execution result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Form of use 2: Regular use 2 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Example: I will use the demo package created above, modify the code directly in step 2, and use this new way to import the package and use it. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
The execution result is the same. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Usage Form 3: Create another alias and use it 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
In the above usage form 1, some people may find that it is not very convenient to use the imported module, and the package name and module name are required. Can it be simpler? Of course, you can directly give another shortened alias to the module in the package, and then use the alias directly. 

Following the example of using Form 1 above, I will not change Step 1 here. I will directly create another alias in Step 2. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Execution result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
The result is the same, but using aliases is much more convenient if the code is longer. 

Of course, you can also use Form 2 to import the package and alias it. Just use an alias when using it. I won't give an example of this method. You can try it yourself. 

Usage 4: Import a function 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Here I also use the already created package and use it directly in another .py file. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Execution result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Usage 5: Import all functions 

When importing the module, we introduced the import * method to import all the functions in the module. Here, you can also enter all the functions of the module in the import package. 

For example, there is a module called "hhhh" in the package named "demo". The code of the module is as follows: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Then we call it in another .py file; 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Execution result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
6. About all uses 

The use of __all__ has been introduced in the module, which is to control the list of functions that can be imported, but in the package, __all__ is to control the list of modules that can be imported, that is, to declare which modules can be imported. 

__all__ inside a package are declared in __init__ file, not in which module. 

For example, there are multiple modules in a package, and all declared modules can be imported, and those that are not declared cannot be imported. 

Step 1, there are two modules called hhhh and my_module in the package named demo, but in the int file it is declared that only the hhhh file can be used. The code of the int file is as follows: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Step 2, import the hhhh and my_module modules in the demo package in the new .py file: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Execution result: 

![avatar]( 25dfe63d1afe46d88b875ce537b208ec.png) 

Obviously, although all modules are imported with *, the hhhh modules declared by all can be used, and the my_module modules not declared by all cannot be used and cannot be recognized by the system. 

###  👳III. The role of modules and packages 

1. Improve the reusability of your code. You are not the only one who can use easy-to-use code, but many people can reuse it. 

2. Improve the readability of the code. If all the code is placed in a .py file, the code will be too long, which increases the difficulty of understanding and maintenance. Therefore, some commonly used code can be packaged into packages and modules, with a literal name, and used directly when needed. This reduces the number of codes and improves readability. 

3. Reduce code redundancy. For some methods encapsulated in the module, we can directly use them for parameters. There is no need to write the methods again, which takes up memory and reduces code redundancy. 

###  👳IV. Installation of third-party libraries 

Although Python has many built-in modules and packages, it is not enough to use only built-in modules. After all, built-in modules are limited, and we often use third-party libraries. It is necessary to learn how to install third-party libraries (packages) at this time. 

Today, we will introduce three installation methods for third-party modules and packages. 

You can download and install the third module and package through the package management command pip, provided that the Python you install is installed in the way I mentioned in the article [Python Basics Introduction] earlier, and all options are checked, so that you don't need to configure environment variables. First, check if your pip works. 

>  Method: WIN + R calls up the running window → enter cmd → pip can be used if the following pip information appears 

![avatar]( 2e25d40c315545f694300f3addced1dc.png) 

  If the scarlet letter prompts "pip in cmd is not an internal or external command, nor is it a runnable program or batch file", then you can manually configure the environment variables. If it doesn't work, go back and follow the steps I said to install Python to reinstall it. 

Returning to the question of how pip installs third-party modules and packages, we must first know the name of the third-party modules and packages we want to install, such as Pillow, a third-party library that is a very powerful tool library for processing images in Python. The installation method is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
![avatar]( 2c3368f1c2ba4892bd28e63e9decc337.png) 

Sometimes there will be a lot of scarlet letters prompting that the download failed. This is normal. The reason may be: 

>  (1) The .pip version is too low, upgrade the pip version and enter in the black window: python -m pip install -U pip 

>  (2) The network is not good, just download it a few more times. 

Installing via pip doesn't require opening the software, but we can also install via Pycharm as follows: 

>  Click File → Settings → Project: Project Name → Python interpreter → Click + → Enter the name of the package you want to install, select the one you like → Click Install Package → Wait for download and installation 

![avatar]( f4de08b43dd34e229d9c29dd04437a8d.png) 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

You can search and download the package you want through the official website and other channels. Official website: https://pypi.org/, search for the third-party library you want to download, such as the library Pillow, and search directly: 

![avatar]( 6fc855aaee5542d280ac9835bb1106d7.png) 

Then select the file you want to download, such as Pillow 8.3.2, enter the download page, and click Download files. 

![avatar]( 74154c816ac34fbca10cd0a04c38c0ab.png) 

 ![avatar]( 9ed44106cf5541679a12e92e28dcff49.png) 

 ![avatar]( 9649a983309d406ba533bee70152e544.png) 

  There are many versions and models after entering. It is recommended to choose the version that matches you, otherwise it may not be installed. Pay attention to the number of Python versions, systems and computers here. For example, my Python is installed 3.9.6, so I placed the file Pillow - 8.3.2 - cp39 - cp39 - win_amd64. Whl. After downloading, WIN + R opens the command line and enters CMD. Enter the file name under the pip install file path in the black window. For example, the path I stored after downloading is D:\ Google Chrome, so the code I entered in the black window is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574541545
 ```  
Then enter to install and wait for the installation to complete. 

![avatar]( 6f8b70ce71c043e59a44b5a3468d7633.png) 

###  👳Conclusion 

The modules and packages in Python are mentioned here first. Some fans told me that they don't know how to read this series of blog posts. Let me explain here. The following picture is an overview of the knowledge section of my series of articles. It is mainly divided into basic introductory and advanced programming. You can follow the serial number to learn. 

![avatar]( 598906531a614d10b2fbaadeeec1552a.png) 

  For example, if you have just started learning Python, then you can read the basic introductory articles. I have put all the knowledge in this section into one. After learning, I will read the articles in advanced programming and follow the serial number to find the corresponding articles. Although I have not sorted out some sections, I will update the content of this section one after another. 

>  Python beginner tutorial column 

![avatar]( 3c2806814176450b9d1dc55befc0fb05.png) 



--------------------------------------------------------------------------------

###  foreword 

I have decided to publish a Python teaching column blog to provide a systematic, practical, and instructional blog learning series for every novice who wants to learn Python. The main knowledge sections include the following aspects: 

![avatar]( b2ad7fd96c314d368219bde1ec9acdd7.png) 

These are all knowledge blocks that Python beginners can't get around. Without them, you would be confused if you went directly to learn crawlers and other directions. On the contrary, if you master them, you can choose any direction of Python to advance. There is no problem. 

>  [Python Beginner Introduction Column] 

The content of [Regular Expression] has been published before. If you are interested, you can take a look. Today's content is [Object Oriented Programming]. If you don't accumulate a few steps, you can't reach a thousand miles. If you don't accumulate small streams, you can't make a river or sea. The accumulation of knowledge one by one, sooner or later you will become the kind of person you envy. Next is the formal content. 

![avatar]( 2755d0fbfca546f5947d684ee270c46a.jpg) 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

###  First, object oriented thinking 

Object-oriented is an abstract programming thinking that is shared by many programming languages. Python is a pure object-oriented language that can be understood as focusing on how to solve problems rather than studying how to implement them. 

Object-oriented and process-oriented are two different ideas. Object-oriented programming languages include Python and other languages, while procedural programming languages include C and other languages. The programming thinking in writing code is different. 

To understand these two ideas, take laundry as an example. 

>  Washing clothes by hand is generally dry like this: find a basin - put water - add washing powder - soak clothes - scrub - wring out - rinse - wring out - dry.

This is a process-oriented thinking. Once you don't know what to do in the middle, you won't be able to wash your clothes well. For example, if you don't know how to scrub your clothes, you won't be able to wash them cleanly. For example, if you don't wring them out after scrubbing, you can directly dry them, resulting in water on the ground. If a certain link goes wrong, it won't achieve the desired laundry effect. 

>  Washing clothes in the washing machine is generally dry like this: turn on the washing machine - put the clothes in - add washing powder - press the start button - dry.

This is an object oriented thinking. You don't need to know how the washing machine washes after putting the clothes in. You just need to know how to pour the washing powder after putting the clothes in and then press the button. 

![avatar]( 99c16e9b71704c5c8203e1eed9e2d7ed.gif) 

Similarly, in programming languages, the performance is different. When writing code in C language, you have to pay attention to your memory and other low-level things, but when writing code in Python, we rarely pay attention to the low-level things. The focus is on what method to use to solve the problem. 

Before we get into the code, there is a bit of a conceptual thing that needs to be understood. After understanding these basic concepts, we can better enter object oriented programming. 

![avatar]( 8cb26f456d674623a1ba8d6f610deca6.jpg) 

###  Two important concepts of object oriented: class and object 

These two concepts may be easier to understand together, and can be simply understood as classes are templates for generating objects. 

We mentioned the example of the washing machine above. If the washing machine is an object, then the blueprint for making this washing machine is a class; if the egg is an object, then the hen is a class; if the dog is an object, then the dog is a class. 

In Python, everything is an object, variables are objects, functions are objects, strings, lists, tuples, and so on are all objects. 

![avatar]( f6ccb90aba4348658e08a648add36add.jpg) 

(1) Composition of objects: object = property + method 

Objects are composed of properties and methods. Properties can be understood as what an object has, and methods can be understood as what an object can do. 

(2) What are the characteristics of the object's properties? 

For example, if a washing machine is an object, then the washing machine has color, and color is an attribute, but color is an abstract thing because it can be red, white, black, and so on. 

For example, if a computer is an object, then the computer has a hard disk, and the hard disk is a property of the computer, so the property of the object can be another object. 

For example, the mouse is an object, the mouse wheel is an object, and the microcontroller inside the mouse is an object. You will find that the large object of the mouse is composed of multiple small objects. 

![avatar]( 572e1018fe2949eda113bf74982286aa.jpg) 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

(3) Methods of the object 

There is a rule to understand first. The methods of an object can be called by themselves or by other objects. I will explain in detail later. 

Here we will not talk about code for the time being, because we must first talk about class knowledge in order to better understand the classes and objects in the code, which will be discussed below. 

As mentioned above, a class is a template for generating objects, so a class is an abstraction of an object, and an object is a materialization of a class. 

Since object = property + method, the same is true for class = property + method. 

(1) Create a class 

How to create a class: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
For example, create a student class and use it to create objects 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
Execution result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
In fact, when creating an object of the Student class, the following three lines of code can be written as follows, with the same effect: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
Let's go back and understand what properties and methods are from the perspective of combining code and concepts. 

Class attributes refer to what is in the class. For example, there are name and age in the class, so name and age are attributes of the Student class. 

The class method is what the class can do. For example, the class has the function learn (self), which can execute "the student's learning method has been called", that is, what the class can do, so the function learn (self) is the method of the class. 

![avatar]( c7cb465ad1c9488f831991c23bfe48a3.jpg) 

We have previously introduced the properties of objects and classes, so let's take a look at the differences and characteristics between the two. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
For example, create an object, view the default init execution, and pass multiple values; call a method of a class to confirm that the method was called and execute the passed value. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
The execution result is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

###  Three characteristics of object oriented 

Three characteristics: encapsulation, inheritance, and polymorphism. 

1. Objects have clear boundaries, and properties and methods are protected within the boundaries. (security) 

2. The strength of the package is moderate. 

3. Principles of encapsulation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
Inheritance is the relationship between a parent class and a child class, such as the dog class and Erha, the dog class is the parent class, and Erha is the child class. 

(1) Define the form (the complete form of the class) 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
(2) Superclass: base class, superclass 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
(3) The characteristics of inheritance 

Example: Invoking the properties and methods of the parent class with an object created by a subclass 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
The execution result is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
A child class can inherit from multiple parent classes. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
The execution result is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
Note: Multiple inheritance has both advantages and disadvantages. The advantage is that it enhances scalability. The disadvantage is that it is easy to confuse logic after complex inheritance relationships, making it difficult to understand. It also takes up a lot of resources. For example, the famous diamond inheritance problem mainly involves the MRO and C3 algorithms. If you don't understand, you can Baidu it. 

(4) Method coverage 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
The execution result is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
(5) Method overloading 

Multiple methods (functions) with the same method name appear, and the method is overloaded by default value in Python. 

![avatar]( 1e813d480ba049e387a2ce3929d55dfd.jpg) 

Polymorphism: A class of things has multiple forms, which is a way of using objects. Subclasses overriding the methods of their parent classes and calling the methods of the same parent class of different subclass objects can produce different effects. 

For example, taking Honor of Kings' selection of heroes as an example, the hero class (Hero) is the parent class, and there is a method called stroke (skill) in the parent class; Cheng Yaojin and descendants are two subclasses, and there is also stroke in the two subclasses; the caller is another parent class, and there is a method to select the hero. The method needs to call the stroke class method, and finally call different subclasses (Cheng Yaojin or descendants) objects to get different skill descriptions. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
The execution result is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
Polymorphism: Send different messages to different objects, and different objects will respond differently when they receive the message. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
The execution result is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574515841
 ```  
Conclusion 

I will continue to update this series of Python beginner series blog posts. If I am sometimes delayed by other things, please forgive me. I will keep updating every week until the update is completed. 

Beginners who want to learn Python can subscribe to my column to learn. If there is time later, I will come up with crawlers, data segmentation, etc., so stay tuned! 

>  [Python Beginner Introduction Column] 

![avatar]( cd2c8a5e6b854da1a00e6bd7d3a7b74f.png) 



--------------------------------------------------------------------------------

How important is the process thread? When you first started learning Python, you may not have felt it, because the code you write can be executed from top to bottom, but in fact this is very basic. When actually developing and writing projects, in order to make full use of the computer configuration to speed up the program progress, we often use multi-process and multi-threading. 

For example, our crawler, without multi-process and multi-threaded programs, can only work with one hand, and after multi-process and multi-threading is turned on, there are several dozens of hands working. It takes you 10 minutes to crawl through the data, and others may finish it in less than a minute. 

![avatar]( d1631261514d4d2da8acd25b2f34b5d6.jpg) 

The process thread is also the last section of knowledge for getting started with Python. Basically, my series of articles on getting started with Python is about to be updated. 

![avatar]( ece106538abc46bbb975c8b42f001849.png) 

>  Python Beginner Tutorial Series Article Column 

Before we start teaching Python processes and threads, there are some basic concepts that need to be explained. 

###  Multitasking operating system 

The operating system can perform multiple tasks, such as our Windows system. In addition to the few tasks currently being performed that you can see, there are also many tasks being performed in the background. You can use the Ctrl + Alt + Del keys to call up the task manager and take a look. 

![avatar]( 596d59cae7044c06a4df3b00fe1f9039.png) 

My computer configuration often sees the properties of a processor with several cores. For example, my computer has 12 cores, which means that the computer can execute up to 12 tasks simultaneously and run up to 12 processes simultaneously. 

![avatar]( 4c762a939ece4a0e919b019bb37a3195.png) 

But why are our computers capable of running hundreds of tasks simultaneously? 

![avatar]( dc814973184d439bb2b7278bcf0cf0ff.png) 

In fact, this is due to the task scheduling of the operating system, most operating systems are scheduled in the form of preemptive time slices. The system switches between multiple tasks very quickly in an extremely small amount of time. For example, an 8-core operating system can theoretically only execute 8 tasks at the same time within 1 second, but the system may switch between hundreds of tasks within 1 second, A task executes, B task executes, C task executes... As a result, many tasks can be executed within 1 second, resulting in hundreds of tasks that are visible to the naked eye being executed all the time. 

The term is "macroscopic parallelism, microscopic serialization," and in fact computers can only perform no more tasks than the number of cores configured in extreme time, and 8 cores can only perform 8 tasks. 

![avatar]( 53ae334ced4440d082f1e17ea70225a3.jpg) 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

Since we talk about tasks, a process is a task, and a process is equivalent to a task, which is the smallest unit of resources allocated by the operating system. In Python, you can use a process to achieve multitasking, and a process is a way to achieve multitasking. 

The multiple subtasks of a process are called threads. Threads are the smallest unit of execution of a process. A process can have many threads, and each thread performs different tasks. 

![avatar]( 819fc84886574ed08f067480bb5d3cda.jpg) 

Python supports both multiple processes and multiple threads. Next, we will start to learn about Python's processes and threads. 

###  Python's multiprocessing (package) 

If you use multiple processes, your Python code is executed line by line from start to finish, which is essentially executing one process, which should be well understood. 

To make more use of CPU resources, we can make use of multiprocessing. Here is a Python multiprocessing package that is commonly used in multiprocessing. It has many functions, such as child processes, communication, sharing, and execution of different forms. Let's learn about some commonly used ones. 

Process is a process class in multiprocessing, through which multiple processes can be realized. Let's take a look at its usage first, and we will have practical examples to describe it later. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
There are many methods in Process, the most common of which is the start () method to start the process. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
For example, the code written is as follows. I want to see the effect of calling functions with and without multiple processes enabled. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
When multiple processes are not started, the execution effect is as follows: 

![avatar]( e44d56851d28415f9f3a3725c0473fb6.gif) 

As you can see, this is a very normal running situation. The program runs from top to bottom, line by line. If the three loops in music () are not completed, they will not execute the movie (). If these two functions are not completed, they will not execute the last line of print ("The main process has completed execution"). 

Let's take a look at adding multiple processes to the code in the above case: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
Code I added an if statement to determine __name__ this, why? Because in the Windows system, multiprocessing this package will occur recursive phenomenon, that is, will be repeatedly executed between "import module - call module", do not believe you can remove the if statement, put all the code inside the outside to execute will report an error, this is a phenomenon that will occur under the Windows system, mac, linux and other systems do not need to add ifl to judge. 

About __name__ = "main" this knowledge point I have talked about in the initialization of modules and packages, if you don't understand, you can go back and take a look. 

Run effect: 

![avatar]( 9adfbde4ada8429cb6365b3b92d16c8c.gif) 

It can be seen that after the process is started, there are three processes running at the same time when the code is running. One is the main process that executes from top to bottom, and the output "The main process is completed" is executed below. The other two child processes execute the music () and movie () processes. Judging from their execution speed, they are running at the same time, so they don't have to wait for the code in one of the functions to execute three times before starting the second function. 

The same code, your execution effect may be different from mine, because the effect is randomly assigned according to the current state of the system, but it does not affect the fact that you can see that its result is multi-threading. 

Finally, let me add that we mentioned earlier that there are args and kwargs in Process that can be passed as parameters. Args are passed as general parameters, and kwargs are passed as parameters in the form of dictionaries. Let's take the above code as an example to pass more parameters. 

![avatar]( 4faa568f48a84f9ca6c5ee4ccb984e0b.png) 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

We mentioned earlier that there are multiple processes performing tasks at the same time when the code is executed, so how to check the number of the current process to know which processes are currently running? Which are the main processes and which are child processes? There are three methods. Let's take a look at the methods first, and then use them together with examples. 

(1) Get the number of the current process: 

You need to use the getpid () method in the os module, which is used as follows: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
(2) Get the name of the current process 

Here is still the multiprocessing package, which has a current_process () method, the usage is as follows: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
(3) Get the number of the current parent process (main process) 

Which parent process does the child process belong to? This uses the getppid () in the os module, and the usage is as follows: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
![avatar]( 17c59d2259a143d691c7b0ca8804e0eb.jpg) 

Then we have seen the method. Based on the example just now, let's get and print the name, number, and number of the parent process of the current process. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
Run result: 

![avatar]( 266b9c6c438b491ca45829a4e740d3c2.gif) 

The number and name can be printed as long as we use the get thread method. 

###  Multithreaded Threading Module 

Multiple processes can run several tasks simultaneously. As we mentioned earlier, the smallest unit of a process is a thread, so threads can also perform multiple tasks. If a process has only one task (the main process), then it can be said that there is only one thread. For example, when we do not use multiple processes to run code, we can say that there is one main process or one main thread. 

A commonly used module for multi-threading is threading, which has a class that teaches Thread. It is similar to the Process class we used for multi-process. Let's take a look at the usage first: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
Similarly, multiple threads also need to be enabled, similar to the previous one. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
There is also a way to get the thread name: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
With these knowledge points in mind, let's start with an example: using a similar example to the one above to use our multithreading. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
It can be seen that our multi-threading is actually similar to multi-process, and it can also run multiple tasks. Here we also increase the use of parameters. 

![avatar]( b3cb831259f747668720524a418cb726.jpg) 

In addition to using the above methods to implement multi-threaded tasks, we can also use inherited classes to implement multi-threading. 

Example: multithreaded to print "cool" and "hair gone." 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
The MyThread class is created by ourselves, which inherits from the parent class threading. Thread. At the same time, we need to write the initialization method of MyThread, and do a good job of preparation every time it is called. We have also talked about this, and we have talked about it in the previous object oriented. If you don't understand, you can look at the content of the object oriented article. 

Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
There are random effects. Your effects may be different from mine. When each computer runs multi-threaded code, whichever thread can grab the time slice will execute first. 

Multithreading can also be achieved through inheritance from the class Thread. 

###  Conclusion 

After the process thread is finished, basically all the knowledge points of getting started with Python are finished, and the rest is an additional chapter. Basically, from the beginning of Python basics to the content of the advanced programming section later, if you finish learning, you can go to any direction of advanced Python. Come on! 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

![avatar]( ca2edc00746f43c890a6892c943e0abd.png) 

>  My official account has finally come out after some preparation. The official account will have all my technical and experience articles, because the types of articles supported by each platform are different, so some articles may not have been seen by you. Welcome to check them out. 



--------------------------------------------------------------------------------

###  foreword 

With the advent of the era of big data, more and more technologies have been taken seriously by enterprises in line with the development of the times and have begun to be applied to the field. Crawler technology is undoubtedly one of the best. Many students are learning this technology whether they are employed or interested. 

Reptiles only need to learn reptile knowledge? It's not that simple. Generally, most of the people who tell you these crash ideas have other intentions. As a retired programmer with more than ten years of service, I personally think that mastering reptiles involves 8 aspects of knowledge! 

![avatar]( 20210421161022766.jpg) 

 Today I'm going to tell you, "What skills do a qualified herpetologist need to learn?" What skills should we focus on mastering?  

###  First, the Python language 

Importance ：★★★★★（ top priority) 

Any technology needs language to support. Among the many computer programming languages, Python is undoubtedly the most suitable for crawling. The most suitable does not mean that it is the only one. Other languages such as Java, C, etc. can be used for crawling development, but Python has unique advantages compared with these languages. Here we will not introduce it in detail. Students who do not know can go to the Internet to learn about it. There are many materials. 

![avatar]( 20210421154805718.jpg) 

 The Python language is the foundation. As long as you have a solid grasp of the basic knowledge at this stage, there will be no problem in the later learning. Then one of the more important knowledge points at this stage is the "object-oriented programming idea". This knowledge point is also the most difficult at this stage. Therefore, students can spend more time on this stage of the Python language, and the content of this piece can be spent more time appropriately. Otherwise, you will always feel that you will hate less when you read it.  

###  Front-end knowledge 

Importance: ★ ★ (understand) 

This content is for understanding. Because we are not doing front-end, we don't need to put too much energy into this part of the content, but we must understand the basic page tags and structure. In the future, when grabbing data, it is necessary to analyze the page. Of course, students who have energy can study it a little deeper. After all, the more you master, the more beneficial the development of crawlers will be. The learning of this part of the content is still reasonably arranged according to your own situation 

###  III. Network programming 

Importance: ★ ★ ★ (learning) 

To be honest, network programming is still a relatively important piece of content. If some students sort out this piece of knowledge more clearly, then the entire crawler process will be very clear. 

![avatar]( 20210421155203599.jpg) 

 Returning to the topic, our main job is crawling. So for this part of the content, we only need to learn basic network programming knowledge. For example: network communication protocols (especially http and https), network request methods, network request and response processes, and so on.  

###  IV. Data storage 

Importance ： ★★★★★（ top priority) 

The importance of data storage is self-evident. Crawling development, part of the work is Crawling the data, the other part also requires us to store data. 

![avatar]( 20210421155418358.jpg) 

 In this section, in addition to the common storage methods such as json, txt, html, etc., you must also master csv and mongodb, especially mongodb is almost a storage method that you must know when you go to an enterprise for an interview; there are also mysql and redis, although mongodb can solve most of the needs. But knowing more storage technologies is definitely good for your own competitiveness.  

###  V. data analytics 

Importance ： ★★★☆（ Mastery) 

How to say this? Strictly speaking, it is not our job responsibility for crawler development, but now many companies have such a demand for crawler development engineers, which means that our threshold is getting higher and higher. 

![avatar]( 20210421155632595.jpg) 

 Then about the content of this part, students can put it to the last stage to learn when they study. Probably the technologies that need to be mastered include numpy, pandas, missingno, jieba and so on.  

###  JavaScript language 

Importance: ★ ★ ★ (learning) 

We learn Python language to facilitate the development of crawlers, so why learn js? 

![avatar]( 2021042115583415.jpg) 

 This problem is very simple. Now more and more web pages will have some js encryption. Then it will cause a big obstacle for us to go to Crawling the data. However, we are going to learn a js language, obviously the learning achievement is too high. So giving it 3 stars does not mean that it is not important, but the learning cost is relatively high at present. If there are students who want to learn js reverse, this content can also be learned later. And now enterprises require us to be familiar with js encryption and understand python common execution js methods, such as pyv8. That's it.  

###  Seven, mobile end technology 

Importance ： ★★★★（ Mastery) 

Nowadays, for a qualified crawler development engineer, it is far from enough to simply crawl the data on the web. With the development of the Internet, the data on mobile devices is more valuable. Therefore, the technical points of this piece are still very important. So what technologies do we all learn? 

First of all, the basic knowledge of android needs to be simply learned, such as what controls andrond has, etc.; secondly, it is necessary to master UIAutomator2; finally, master the usage of package capture tools such as fiddler, etc 

![avatar]( 20210421160435221.jpg) 

 Of course, I would like to add that the technical points are only general directions, and there are still many details that need to be learned. Here is just a reference for you to learn.  

###  Eight, reptile knowledge 

Importance ： ★★★★★（ top priority) 

Here comes the most important piece. Reptile technology is the foundation of our survival as reptile development engineers. Then let's talk about what technologies we need to master in general: 

◆ Proficient in web parsing technologies such as regular, Xpath, bs4, etc 

◆ Study crawler strategies and anti-blocking rules, solve difficulties such as blocking accounts, blocking IPs, and page jumps, and improve the efficiency and quality of web crawling 

◆ Familiar with verification code recognition, simulated login, data cleaning, deduplicate, warehousing, etc 

![avatar]( 20210421161329723.jpg) 

 Proficient in the Scrapy framework and distributed crawlers, it is not difficult to find through the above list of knowledge points, which mainly include four aspects: web page analysis, anti-crawl technology, data warehousing, and the Scrapy framework. To learn well in each aspect, there are certain difficulties. This requires us to accumulate more in our usual learning, so as to achieve flexible application of knowledge points. 

![avatar]( 20210420152930243.jpg) 

  The text of the article has ended here. I just want to thank some of the people who read my article. 

I have been learning how to write articles since I retired. To be honest, every time I see some readers' responses in the background, I feel very relieved, so I want to contribute some of my collection of programming dry goods to everyone, giving back to every reader, hoping to help you. 

Dry goods mainly include: 

① More than 2,000 Python e-books (both mainstream and classic books should be available) 

② Python standard library information (the most complete Chinese version) 

③ Project source code (40 or 50 interesting and classic practice projects and source code) 

④ Python basic introductory videos, etc. (suitable for Xiaobai to learn) 

![avatar]( 20210421162557587.png) 

 * If you can use it, you can take it directly and see my personal introduction. *  



--------------------------------------------------------------------------------

If you want to learn programming by yourself, be sure to bookmark these 7 websites. There are many free high-quality tutorials above, which can save you tens of thousands of dollars in tuition! 

Without further ado, go straight to the dry goods! 

###  The first one, W3school. 

A website that focuses on graphic tutorials, whether it is front-end development of HTML, CSS, or databases, or the learning of programming languages such as Python, has everything, and the key is free. I think as a website, it doesn't have to be so good. 

![avatar]( 9549c882ef174a7d8b7268ebbb6f4d80.png) 

Portal: https://www.w3school.com.cn/ 

###  Second, Chinese university MOOCs. 

There are many free national-level programming courses on it. Some university teachers offer free courses on it in order to complete teacher indicators or gain reputation. For example, if you want to learn Python, you can search for it. There are many national high-quality Python courses on it. 

![avatar]( d8f28c322be2429bb82dac58f7e6551b.png) 

  Eh, you can learn high-quality human courses without paying tuition, isn't this better than an enrollment brochure? 

Portal: https://www.icourse163.org/ 

###  Third, Bilibili. 

Also known as Bilibili, although the above is mixed, there are many interesting programmers who teach their own experience, such as technical fat and other up masters. 

Another advantage of Bilibili is that if you are tired and sleepy from studying, you don't need to drink Dongpeng special drink, change the channel to see the dancing up master, and you will feel like you are doing it again. 

![avatar]( 234ed45ae30347ecbf61819bb698359f.png) 

However, I suggest that you should keep your eyes open for the five or six hundred Python courses. Some five or six hundred sections have not yet finished teaching Python functions. How can there be so much content to talk about? It's all cut out to make up the number of courses. 

![avatar]( e103a2637679403f81bd15bf4200f7f0.png) 

###  Fourth, Cainiao tutorial 

This is also a website that focuses on graphic tutorials, and it is also purely free. There are web development and various language learning. I personally feel that the typesetting is more comfortable than W3school, and the content is more detailed. 

I thought W3school was already invincible, but I didn't expect anyone to be braver than him. Whose website is this? 

![avatar]( 9d9df37b55e04953bfef04b6f46df5b2.png) 

Link: https://www.runoob.com/ 

###  Fifth, CSDN. 

Although CSDN was often exposed to a large number of plagiarism and other shortcomings, it did not affect the fact that it was the largest gathering place for domestic programmers. There were also many excellent programmer bloggers who were constantly updating, such as the blogger "Where did the hero come out" in the field of algorithms. 

Of course, you can also go to the Python graphic tutorial written by Uncle Long, which is interesting and not boring. 

![avatar]( 867139b544154edab5e9e0866cf8daf6.png) 

Portal: https://blog.csdn.net/zhiguigu/category_11347049.html?spm=1001.2014.3001.5482 

###  Sixth, the buckle. 

Most programmers learn algorithms here, and there are many different levels of learners posting in the discussion forum. It's a good idea to go here. 

![avatar]( 71a4786791e546e2b2594525c7dd689a.png) 

Portal: https://leetcode-cn.com/ 

###  Number seven, NowCoder. 

Most programmers will come here to brush the questions when looking for a job. Not only are there many pen interview questions from well-known enterprises, but they can also simulate the written test. If you are not confident in finding a job, then brush the questions more! There are also many big names on it, and maybe you can get referrals. 

![avatar]( 16c954730b8e42cba37444061b7493a3.png) 

Portal: https://www.nowcoder.com/ 

###  Conclusion 

Learning programming has never happened overnight. Those who tell you that they can master a language in a few days are all fooling people. 

I like Python very much, and I have collected a lot of technical dry goods, which can be shared with friends who like my articles. If you are willing to take the time to study, they will definitely help you. The dry goods include: 

![avatar]( 17baf34c84e4483f9f9b3d9bb3341c44.png) 

![avatar]( 521e60d8459b40f2bd654b1a410926db.png) 

 Click on the business card at the end of the article to take it away.  



--------------------------------------------------------------------------------

