As a practical tool for dealing with strings, regular expressions are often used in Python, such as crawlers Crawling the data to retrieve strings and so on. Regular expressions are already embedded in Python and can be used by importing the re module. As newbies to Python, most of them have heard of the term "regular". 

Today, I would like to share with you a more detailed collection of Python regular expressions. After learning it, you will become proficient in regular expressions. 

![avatar]( b0f3f391f36c4c4186afb0c767449760.jpg) 

###  The re-module 

Before we talk about regular expressions, we must first know where to use regular expressions. Regular expressions are used in the findall () method, and most string retrievals can be done through findall (). 

1. Import the re module. Before using the regular expression, you need to import the re module. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
2. the syntax of findall (): 

After importing the re module, you can use the findall () method, so we must be clear about the syntax of findall (). 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
It is not difficult to see that findall () is composed of a regular expression and a target string. The target string is what you want to retrieve, so how to retrieve it is performed through a regular expression, which is our focus today. 

The result returned after using findall () is a list of strings that meet the regularization requirements 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

###  Second, regular expressions 

1. Ordinary characters, most letters and characters can be matched by themselves. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
2. Metacharacters 

Metacharacters refer to special characters such as .^ $ ?+ {} \ [], through which we can personalize the search of the target string and return the result we want. 

Here I will introduce to you 10 commonly used metacharacters and their usage. Here I will give you a simple summary for easy memorization. The following will explain the use of each metacharacter one by one. 

![avatar]( 8c37aa9d37e14e9880b384e5b85721e3.png) 

（1） [] 

[] 的使用方式主要有以下三种： 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
The output is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
For example, to select the abc element in the string "abcabcaccaac": 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
The output is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
For example, to select "caa" in the string "caabcabcaabc": 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
The output is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Note: When in the first position of [], it means that everything except a is matched, such as changing the position of a in []: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
（2）^ 

^ is usually used to match the beginning of a line, for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
![avatar]( 724785f6d8f5422e8c52eaef8b552226.jpg) 

>  Fan exclusive benefits 

(3) $$is usually used to match the end of a line, for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
![avatar]( 8ca641e45b994987a9a23ba070981eee.jpg) 

（4）\ 

After the backslash, different characters can be added to represent different special meanings. Common ones include the following three. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
The output is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
\ can be escaped into normal characters, for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Match any whitespace characters such as: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Matches any alphanumeric and underscore, equivalent to [a-zA-Z0- 9_], for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
![avatar]( 1e9ee27672ed489dafb11d1c71a02a02.jpg) 

（5）{n} 

{N} can avoid repeated writing. For example, we wrote\ w 3 times when we used\ w earlier, but here we need to use {n}. N represents the number of matches, for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
（6）* 

* Means zero or more matches (as many as possible), for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
**（7） + ** 

+ means match one or more times, e.g. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
（8） . 

. is a dot, which is not obvious here. It is used to manipulate any character other than a newline character, such as: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
(9) ？ 

? means one match or zero 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Pay attention to greedy and non-greedy patterns here. 

Greedy pattern: Match as much data as possible, expressed as\ d followed by a metacharacter, such as\ d *: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Non-greedy mode: Match as little data as possible, expressed as\ d followed by?, such as\ d? 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
The output is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
(10) {m, n} m, n refers to a decimal number that is repeated at least m times and at most n times, for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Add? means to match as little as possible 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
There are other flexible ways to write {m, n}, such as: 

![avatar]( 14d7db206f8943418d2a43026521c828.jpg) 

Regarding the commonly used metacharacters and how to use them, let's take a look at the other knowledge of regular rules. 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

###  (2) The use of regular rules 

1. Compile regular 

In Python, the re module can compile regulars through the compile () method, re.compile (regular expression), for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
2. How to use regular objects 

The use of regular objects is not only through the findall () method we introduced earlier, but also through other methods. The effect is different. Here is a simple summary: 

(1) findall () finds all strings that re match and returns a list 

(2) search () scans the string to find the position where the re matches (just the first one found) 

(3) match () determines whether re is at the beginning of the string (matches the beginning of the line) 

Let's take the example of the object returned by compile () after compiling the regular. Instead of findall (), let's use match () to see how the result is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
It can be seen that the result is a match object, the starting subscript position is 0~ 13, and the match is 010-123456789. Since the object is returned, let's talk about some operation methods of this match object. 

![avatar]( 511fa5bb3d9e404398729084f797a7d6.jpg) 

>  Fan benefits 

3. Match object operation method 

Here are the methods first, and I will give examples later. Common methods of using Match objects are as follows: 

(1) group () returns the re-matched string 

(2) start () returns the starting position of the match 

(3) end () returns the position where the match ends 

(4) span () returns the position of a tuple: (start, end) 

Example: Use span () to operate on the object returned by search (): 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
The result is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Functions 4.re module 

In addition to the findall () function introduced above, there are other functions in the re module to provide an introduction: 

(1) findall () returns all the strings that match according to the regular expression. I won't say much about this. I have introduced it earlier. 

(2) sub (regular, new string, original string) The function of sub () is to replace the string, for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
(3) subn (regular, new string, original string) The function of subn () is to replace the string and return the number of replacements 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
(4) split () split () split string, for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
Output result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574598613
 ```  
![avatar]( 1b31fa941d2944b8a9131f06c72a5cd8.jpg) 

Regarding regularity, I have said so much. Regularity is an indispensable foundation in almost all directions of Python. I wish you all the best in your Python journey! 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

![avatar]( 884b16d55fc040289932e9f4b3d23c91.png) 

