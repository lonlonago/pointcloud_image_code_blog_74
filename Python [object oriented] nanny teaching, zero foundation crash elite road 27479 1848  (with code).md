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

