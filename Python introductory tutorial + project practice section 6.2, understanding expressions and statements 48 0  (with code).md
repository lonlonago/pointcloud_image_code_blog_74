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

