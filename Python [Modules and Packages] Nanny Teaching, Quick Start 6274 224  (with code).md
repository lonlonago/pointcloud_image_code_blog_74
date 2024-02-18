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

