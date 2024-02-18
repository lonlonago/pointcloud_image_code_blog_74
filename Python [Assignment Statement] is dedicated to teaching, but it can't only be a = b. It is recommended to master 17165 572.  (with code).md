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

