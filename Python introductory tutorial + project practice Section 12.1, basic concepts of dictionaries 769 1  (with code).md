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

