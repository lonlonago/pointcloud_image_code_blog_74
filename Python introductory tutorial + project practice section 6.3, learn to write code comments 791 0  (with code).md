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

