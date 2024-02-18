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

