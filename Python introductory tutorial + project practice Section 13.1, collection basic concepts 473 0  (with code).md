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

