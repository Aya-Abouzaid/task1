# task1 OOP DisAdvantages 
https://www.aplustopper.com/advantages-and-disadvantages-of-oop/

Dis of OOP:
1- It is slower than other programs
2- Size is larger than other programs
3- It required a lot of effort to create
4- It is not suitable for some sorts of problems


# task2 whats the diffrence between multithreading & multiprocessing

Multithreading is a programming technique that assigns multiple code segments to a single process. These code segments, also referred to as threads, run concurrently and parallel to each other. These threads share the same memory space within a parent process. This saves system memory, increases computing speed and improves application performance.

For example, if you're working on your computer, you might have multiple browser tabs open while searching the internet. You might also be listening to music through a desktop application at the same time. The internet browser and music application represent two different processes, even though they are operating simultaneously. However, the multiple tabs you have open while browsing the internet represent threads of your internet browser, which is the parent process.


Multiprocessing refers to a system that has more than two central processing units (CPUs). Every additional CPU added to a system increases its speed, power and memory. This allows users to run multiple processes simultaneously. Each CPU may also function independently, and some CPUs may remain idle if they don't have anything to process. This can improve the reliability of a system because unused CPUs can act as a backup if technical issues arise. 


# task3
Tabulation Meaning:
Tabulation is a systematic and logical representation of numeric data in rows and columns to facilitate comparison and statistical analysis. It facilitates comparison by bringing related information close to each other and helps in statistical analysis and interpretation.

In other words, the method of placing organised data into a tabular form is known as tabulation. It may be complex, double, or simple, depending upon the nature of categorisation.

Objectives Of Tabulation:
(1) To simplify complex data

It reduces the bulk of information, i.e., it reduces raw data in a simplified and meaningful form so that it can be easily interpreted by a common man in less time.
(2) To bring out essential features of data

It brings out the chief/main characteristics of data.
It presents facts clearly and precisely without textual explanation.
(3) To facilitate comparison

The representation of data in rows and columns is helpful in simultaneous detailed comparison on the basis of several parameters.
(4) To facilitate statistical analysis

Tables serve as the best source of organised data for statistical analysis.
The task of computing average, dispersion, correlation, etc., becomes easier if data is presented in the form of a table.
(5) To save space

A table presents facts in a better way than the textual form.
It saves space without sacrificing the quality and quantity of data.


# task4 clean code https://blog.unosquare.com/10-tips-for-writing-cleaner-code-in-any-programming-language


1. Use descriptive names

Make the names of the variables and the names of the functions must be as descriptive as they can be. For example, suppose you want to make some references to the character and last name. In that case, you might use a variable that calls "namePhysician" and "lastNamePhysician" instead of using "name." Even worse if you use "n." Why? Because with that syntax, anybody can understand what value the variable contains.

And what about a function? Well, the name of a function must start with a verb. For example, if I have a function that returns the physician's name, I can create a function that calls "getPhysicianName" instead of using a function that only calls "name."




2. Use empty lines to create a readable code

With empty lines, we can add legibility to our code. An extra line will be beneficial to identify in an easy way where the functions end. Also, we can use empty lines to separate the variable's declaration from the function's operation. Finally, we might add an extra line before the returned value if you want.




3. Do not send more than three parameters into a function

Remember, we must make a readable function. It is easier to have three parameters and follow their logic inside the function than to have a bunch of parameters and try to find where the parameters are used.

If we need to use more than three parameters, we can send one object to the function and use the keys of the object as we need. Review the following point if you need to send many parameters into a function.




4. Remember the functions must do only one thing

I know that sometimes we are in a hurry or want to solve our problem with one function, and we write a function that does many things. Avoid doing that. A function must do one thing. It is better to have two or more short and easy functions than to have one complex function.




5. Functions must be small

If you need to do a function with many lines, you must consider that maybe it is more accurate to use a class instead of a function. Remember your function must do only one thing.

6. Reduce the number of characters in a line

Keep in mind that we want to create a code that is easy to read. Avoid having long lines of code. The size of a line must fit in your screen so that you don't need to do a horizontal scroll. Remember, there are a lot of tools like prettier that allow you to control the format of the code.

7. Avoid using comments

Sometimes it is difficult to maintain the code. Imagine if we have to maintain the comments too! How can we avoid using a comment? We can use descriptive names. If our code is understandable, we don't need a comment. If we create a comment and somebody has to change the code, we cannot confirm that this person updated the comment. Remember that if you are using a comment, it is because our code is not clear enough. But maybe you think it is sometimes necessary to add a comment, if that's the case, use comments but only in some exceptional cases.

8. Create a descriptive message when you create a commit

When we create a commit, we have to write a descriptive message. That message could be helpful if we want to remember what our code is doing some months later. Avoid messages that do not give us much information. If you only write messages like "refactoring," perhaps this could not be clear enough for the following developers.




9. Use Unit Test and practice Test Driven Development

I know that sometimes we think that unit tests are a waste of time. But believe me, it is false. Indeed, unit tests do work. Imagine that somebody is working with the code you created some months ago, and the new developer creates a code that is solving a thing, but it is breaking other functionality. How can you or the other developer know that the code is breaking? Well, if the project has unit tests, it could be easy to identify those problems. Yes, I know that sometimes we have to deliver many things in a very short time, but this extra time that you invest in unit tests can save a lot of time in the future.

As a good practice, first, create your unit test; obviously, it will fail, continue creating your routine or update the code, and finally rerun your unit test; this will run successfully. The advantage of working in that way is that you can have a better approach to solving the problem you are facing.

10. Learn Design Patterns

"Design Patterns" is a very broad topic. As an introduction, if you study Design Patterns, you can know the solutions that some master developers had found when facing some common problems in their software. And it lets us avoid reinventing the wheel.

So I highly recommend reading the book: Design Patterns, Elements of Reusable Object-Oriented Software, written by Erich Gamma, Richard Helm, Ralph Johnson, and John Vlissides.


# task5 API in Python
https://www.dataquest.io/blog/python-api-tutorial/

What is an API?
An API, or Application Programming Interface, is a server that you can use to retrieve and send data to using code. APIs are most commonly used to retrieve data, and that will be the focus of this beginner tutorial.

When we want to receive data from an API, we need to make a request. Requests are used all over the web. For instance, when you visited this blog post, your web browser made a request to the Dataquest web server, which responded with the content of this web page.


r api tutorial api request
 

API requests work in exactly the same way – you make a request to an API server for data, and it responds to your request.

Making API Requests in Python
In order to work with APIs in Python, we need tools that will make those requests. In Python, the most common library for making requests and working with APIs is the requests library. The requests library isn’t part of the standard Python library, so you’ll need to install it to get started.

If you use pip to manage your Python packages, you can install requests using the following command:

pip install requests
If you use conda, the command you’ll need is:

conda install requests
Once you’ve installed the library, you’ll need to import it. Let’s start with that important step:

import requests
Now that we’ve installed and imported the requests library, let’s start using it.

Making Our First API Request
There are many different types of requests. The most commonly used one, a GET request, is used to retrieve data. Because we’ll just be working with retrieving data, our focus will be on making ‘get’ requests.

When we make a request, the response from the API comes with a response code which tells us whether our request was successful. Response codes are important because they immediately tell us if something went wrong.

To make a ‘GET’ request, we’ll use the requests.get() function, which requires one argument — the URL we want to make the request to. We’ll start by making a request to an API endpoint that doesn’t exist, so we can see what that response code looks like.

response = requests.get("https://api.open-notify.org/this-api-doesnt-exist")
The get() function returns a response object. We can use the response.status_code attribute to receive the status code for our request:

print(response.status_code)
404
The ‘404’ status code might be familiar to you — it’s the status code that a server returns if it can’t find the file we requested. In this case, we asked for this-api-doesnt-exist which (surprise, surprise) didn’t exist!

Let’s learn a little more about common status codes.

API Status Codes
Status codes are returned with every request that is made to a web server. Status codes indicate information about what happened with a request. Here are some codes that are relevant to GET requests:

200: Everything went okay, and the result has been returned (if any).
301: The server is redirecting you to a different endpoint. This can happen when a company switches domain names, or an endpoint name is changed.
400: The server thinks you made a bad request. This can happen when you don’t send along the right data, among other things.
401: The server thinks you’re not authenticated. Many APIs require login ccredentials, so this happens when you don’t send the right credentials to access an API.
403: The resource you’re trying to access is forbidden: you don’t have the right perlessons to see it.
404: The resource you tried to access wasn’t found on the server.
503: The server is not ready to handle the request.
You might notice that all of the status codes that begin with a ‘4’ indicate some sort of error. The first number of status codes indicate their categorization. This is useful — you can know that if your status code starts with a ‘2’ it was successful and if it starts with a ‘4’ or ‘5’ there was an error. 

# task6  cron jobs
https://www.hivelocity.net/kb/what-is-cron-job/

What is Cron Job?
A cron job is a Linux command used for scheduling tasks to be executed sometime in the future. This is normally used to schedule a job that is executed periodically – for example, to send out a notice every morning. Some scripts, such as Drupal and WHMCS may require you to set up cron jobs to perform certain functions.

For most cron jobs, there are three components present:

The script that is to be called or executed.
 
The command that executes the script on a reoccurring basis. This is typically set in cPanel.
 
The action or output of the script, which depends on what the script being called does. Frequently, scripts called as cron jobs modify files or databases. However, they can perform other tasks that do not modify data on the server as well, such as sending out email notifications.
Most scripts that require the use of a cron job will give you specific instructions on what needs to be setup, frequently giving examples.

 
# task7  c++ frameworks used in ML
https://geekflare.com/ai-frameworks/

Here is the list of the top 10 C++ frameworks for machine learning

Microsoft CNTK	
CAFFE
TensorFlow. ...
Caffe from Berkeley. ...
Microsoft Cognitive Toolkit (CNTK) ...
mlpack Library. ...
SHARK Library. ...
Armadillo. ...
Faisis. ...
OpenNN.

 
# task8  Design patterns
