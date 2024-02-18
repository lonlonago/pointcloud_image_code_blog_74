How important is the process thread? When you first started learning Python, you may not have felt it, because the code you write can be executed from top to bottom, but in fact this is very basic. When actually developing and writing projects, in order to make full use of the computer configuration to speed up the program progress, we often use multi-process and multi-threading. 

For example, our crawler, without multi-process and multi-threaded programs, can only work with one hand, and after multi-process and multi-threading is turned on, there are several dozens of hands working. It takes you 10 minutes to crawl through the data, and others may finish it in less than a minute. 

![avatar]( d1631261514d4d2da8acd25b2f34b5d6.jpg) 

The process thread is also the last section of knowledge for getting started with Python. Basically, my series of articles on getting started with Python is about to be updated. 

![avatar]( ece106538abc46bbb975c8b42f001849.png) 

>  Python Beginner Tutorial Series Article Column 

Before we start teaching Python processes and threads, there are some basic concepts that need to be explained. 

###  Multitasking operating system 

The operating system can perform multiple tasks, such as our Windows system. In addition to the few tasks currently being performed that you can see, there are also many tasks being performed in the background. You can use the Ctrl + Alt + Del keys to call up the task manager and take a look. 

![avatar]( 596d59cae7044c06a4df3b00fe1f9039.png) 

My computer configuration often sees the properties of a processor with several cores. For example, my computer has 12 cores, which means that the computer can execute up to 12 tasks simultaneously and run up to 12 processes simultaneously. 

![avatar]( 4c762a939ece4a0e919b019bb37a3195.png) 

But why are our computers capable of running hundreds of tasks simultaneously? 

![avatar]( dc814973184d439bb2b7278bcf0cf0ff.png) 

In fact, this is due to the task scheduling of the operating system, most operating systems are scheduled in the form of preemptive time slices. The system switches between multiple tasks very quickly in an extremely small amount of time. For example, an 8-core operating system can theoretically only execute 8 tasks at the same time within 1 second, but the system may switch between hundreds of tasks within 1 second, A task executes, B task executes, C task executes... As a result, many tasks can be executed within 1 second, resulting in hundreds of tasks that are visible to the naked eye being executed all the time. 

The term is "macroscopic parallelism, microscopic serialization," and in fact computers can only perform no more tasks than the number of cores configured in extreme time, and 8 cores can only perform 8 tasks. 

![avatar]( 53ae334ced4440d082f1e17ea70225a3.jpg) 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

Since we talk about tasks, a process is a task, and a process is equivalent to a task, which is the smallest unit of resources allocated by the operating system. In Python, you can use a process to achieve multitasking, and a process is a way to achieve multitasking. 

The multiple subtasks of a process are called threads. Threads are the smallest unit of execution of a process. A process can have many threads, and each thread performs different tasks. 

![avatar]( 819fc84886574ed08f067480bb5d3cda.jpg) 

Python supports both multiple processes and multiple threads. Next, we will start to learn about Python's processes and threads. 

###  Python's multiprocessing (package) 

If you use multiple processes, your Python code is executed line by line from start to finish, which is essentially executing one process, which should be well understood. 

To make more use of CPU resources, we can make use of multiprocessing. Here is a Python multiprocessing package that is commonly used in multiprocessing. It has many functions, such as child processes, communication, sharing, and execution of different forms. Let's learn about some commonly used ones. 

Process is a process class in multiprocessing, through which multiple processes can be realized. Let's take a look at its usage first, and we will have practical examples to describe it later. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
There are many methods in Process, the most common of which is the start () method to start the process. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
For example, the code written is as follows. I want to see the effect of calling functions with and without multiple processes enabled. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
When multiple processes are not started, the execution effect is as follows: 

![avatar]( e44d56851d28415f9f3a3725c0473fb6.gif) 

As you can see, this is a very normal running situation. The program runs from top to bottom, line by line. If the three loops in music () are not completed, they will not execute the movie (). If these two functions are not completed, they will not execute the last line of print ("The main process has completed execution"). 

Let's take a look at adding multiple processes to the code in the above case: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
Code I added an if statement to determine __name__ this, why? Because in the Windows system, multiprocessing this package will occur recursive phenomenon, that is, will be repeatedly executed between "import module - call module", do not believe you can remove the if statement, put all the code inside the outside to execute will report an error, this is a phenomenon that will occur under the Windows system, mac, linux and other systems do not need to add ifl to judge. 

About __name__ = "main" this knowledge point I have talked about in the initialization of modules and packages, if you don't understand, you can go back and take a look. 

Run effect: 

![avatar]( 9adfbde4ada8429cb6365b3b92d16c8c.gif) 

It can be seen that after the process is started, there are three processes running at the same time when the code is running. One is the main process that executes from top to bottom, and the output "The main process is completed" is executed below. The other two child processes execute the music () and movie () processes. Judging from their execution speed, they are running at the same time, so they don't have to wait for the code in one of the functions to execute three times before starting the second function. 

The same code, your execution effect may be different from mine, because the effect is randomly assigned according to the current state of the system, but it does not affect the fact that you can see that its result is multi-threading. 

Finally, let me add that we mentioned earlier that there are args and kwargs in Process that can be passed as parameters. Args are passed as general parameters, and kwargs are passed as parameters in the form of dictionaries. Let's take the above code as an example to pass more parameters. 

![avatar]( 4faa568f48a84f9ca6c5ee4ccb984e0b.png) 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

We mentioned earlier that there are multiple processes performing tasks at the same time when the code is executed, so how to check the number of the current process to know which processes are currently running? Which are the main processes and which are child processes? There are three methods. Let's take a look at the methods first, and then use them together with examples. 

(1) Get the number of the current process: 

You need to use the getpid () method in the os module, which is used as follows: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
(2) Get the name of the current process 

Here is still the multiprocessing package, which has a current_process () method, the usage is as follows: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
(3) Get the number of the current parent process (main process) 

Which parent process does the child process belong to? This uses the getppid () in the os module, and the usage is as follows: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
![avatar]( 17c59d2259a143d691c7b0ca8804e0eb.jpg) 

Then we have seen the method. Based on the example just now, let's get and print the name, number, and number of the parent process of the current process. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
Run result: 

![avatar]( 266b9c6c438b491ca45829a4e740d3c2.gif) 

The number and name can be printed as long as we use the get thread method. 

###  Multithreaded Threading Module 

Multiple processes can run several tasks simultaneously. As we mentioned earlier, the smallest unit of a process is a thread, so threads can also perform multiple tasks. If a process has only one task (the main process), then it can be said that there is only one thread. For example, when we do not use multiple processes to run code, we can say that there is one main process or one main thread. 

A commonly used module for multi-threading is threading, which has a class that teaches Thread. It is similar to the Process class we used for multi-process. Let's take a look at the usage first: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
Similarly, multiple threads also need to be enabled, similar to the previous one. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
There is also a way to get the thread name: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
With these knowledge points in mind, let's start with an example: using a similar example to the one above to use our multithreading. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
It can be seen that our multi-threading is actually similar to multi-process, and it can also run multiple tasks. Here we also increase the use of parameters. 

![avatar]( b3cb831259f747668720524a418cb726.jpg) 

In addition to using the above methods to implement multi-threaded tasks, we can also use inherited classes to implement multi-threading. 

Example: multithreaded to print "cool" and "hair gone." 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
The MyThread class is created by ourselves, which inherits from the parent class threading. Thread. At the same time, we need to write the initialization method of MyThread, and do a good job of preparation every time it is called. We have also talked about this, and we have talked about it in the previous object oriented. If you don't understand, you can look at the content of the object oriented article. 

Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574570924
 ```  
There are random effects. Your effects may be different from mine. When each computer runs multi-threaded code, whichever thread can grab the time slice will execute first. 

Multithreading can also be achieved through inheritance from the class Thread. 

###  Conclusion 

After the process thread is finished, basically all the knowledge points of getting started with Python are finished, and the rest is an additional chapter. Basically, from the beginning of Python basics to the content of the advanced programming section later, if you finish learning, you can go to any direction of advanced Python. Come on! 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

![avatar]( ca2edc00746f43c890a6892c943e0abd.png) 

>  My official account has finally come out after some preparation. The official account will have all my technical and experience articles, because the types of articles supported by each platform are different, so some articles may not have been seen by you. Welcome to check them out. 

