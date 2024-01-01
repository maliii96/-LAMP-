# -(L)(A)(M)(P)-

BASH Chronicles: AWS & The LAMP Acension Saga

'WHATS GOOD' I've been working on a project where I use a Bash script to set a LAMP (Linux, Apache, MySQL, PHP) stack on a AWS instance that your freshly created. Instead of remoting into and installing everything one by one this script would do all that for you.

The Challenge
The main goal was to automate the creation of an Ubuntu VM in AWS and configure it as a LAMP server. I'm not going to lie I thought it would be simple.

Issues Encountered
Waiting for Instance to Run: The first major hurdle was dealing with the wait time for the EC2 instance. It took forever and eventually just timed out.

SSH Connection Hiccups: Make sure to wait for the instance to pass its checks, just because it says its running when you launch it doesn't mean its ready yet. 

I thought I was tripping because I could SSH into via the AWS CLI but I couldn't get the script to do it all at once

Public IP Mystery: The script was supposed to fetch the public IP of the instance, but all I got was 'None'. After some digging, I realized it was because the instance wasn't running yet when the script tried to retrieve the IP. HAHA its true when they say patience is key lol




Solutions and Learnings
Patience with AWS: Sometimes, instances just take their sweet time to start up. I learned to check the AWS Console for any specific issues and extended the wait time in the script.

I eventually started to play around with the script to see what works and doesn't. Thats where i found out that I could completely take out portions of the Bash script and it would still run fine.

SSH Nuances: I got a better handle on SSH connection intricacies, like ensuring the instance is ready and the public IP is correctly fetched before attempting to connect.

Final Thoughts
This project was a great learning experience! It had its frustrating moments, but overcoming these challenges was super rewarding. I'm now more comfortable with AWS, Bash scripting, and troubleshooting.





