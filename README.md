# -(L)(A)(M)(P)-

What is a LAMP stack?
Linux: The "L" in LAMP represents the operating system, which is typically some flavor of the Linux operating system. Linux provides the foundational infrastructure for hosting web applications.

Apache: The "A" in LAMP stands for Apache, which is a widely-used open-source web server software. Apache is responsible for handling HTTP requests from clients (such as web browsers) and serving web pages and other content to them.🌐

MySQL: The "M" in LAMP represents MySQL, a relational database management system (RDBMS). MySQL is used to store and manage the structured data of your web application. It is known for its reliability, performance, and ease of use.🏡

PHP: The "P" in LAMP stands for PHP, which is a server-side scripting language used for building dynamic web pages and web applications. PHP is embedded within HTML code and allows developers to interact with databases, handle form submissions, and perform various server-side tasks.🚀

These are the basic components that make up a website/web application. Of course theirs other variations of the LAMP stack but this is just the basics.🌟



 BASH Chronicles: AWS & The LAMP Acension Saga
 
 I've been working on a project where I use a Bash script to setup a LAMP (Linux, Apache, MySQL, PHP) stack on a AWS instance that you freshly created. Instead of remoting into and installing everything one by one this script would do all that for you.

Purpose🎯
The main goal was to automate the task of sshing  into a AWS instance and configure it as a LAMP server.

Issues Encountered🤯
Waiting for Instance to Run: The first major hurdle was dealing with the wait time for the EC2 instance. It took forever and eventually just timed out.

SSH Connection Hiccups💡
Make sure to wait for the instance to pass its checks, just because it says its running when you launch it doesn't mean its ready yet. 
I thought I was tripping because I could SSH into via the AWS CLI but I couldn't get the script to do it all at once

Public IP Mystery❓
The script was supposed to fetch the public IP of the instance, but all I got was 'None'. After some digging, I realized it was because the instance wasn't running yet when the script tried to retrieve the IP. HAHA its true when they say patience is key 😅 



Solutions and Learnings

Patience with AWS⏳
Sometimes instances just take their sweet time to start up. I learned to check the AWS Console for any specific issues and extended the wait time in the script.

Testing🛠️
I eventually started to play around with the script to see what works and doesn't. Thats where i found out that I could completely take out portions of the Bash script and it would still run fine. It took me so many attempts.

SSH Nuances🚪
During this project, I honed my understanding of SSH intricacies, emphasizing patience and precision.
One crucial insight was the importance of instance readiness. A running instance doesn't guarantee it's ready for SSH. Waiting for initialization is key to seamless connections.



Final Thoughts
At first, I was a little intimidated by this project because I tend to overthink things and sometimes get stuck in analysis paralysis. However, after completing it, I realized it wasn't as daunting as I had initially thought. From now on, I'm going to dive headfirst into projects and figure out the rest as I go along.




