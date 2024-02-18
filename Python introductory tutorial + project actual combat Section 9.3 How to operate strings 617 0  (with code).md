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

