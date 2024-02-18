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

