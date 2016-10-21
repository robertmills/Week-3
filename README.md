# Week-3
Week 3 Project for TCMG 412

Project requirements
GROUP PROJECT #3: Building an app in Ruby
For this project, you will be working individually or in pairs (at your discretion). If you work in a pair group, you will each receive the same grade for the project.

The goal of this project is to familiarize yourself with Ruby syntax, and some basic tasks that are common in systems programming and administration. The program will be invoked from the command line on a fresh Linux machine, so if you introduce any library dependencies beyond the Ruby Standard Library (not recommended), you must provide very clear instructions to recreate your environment. I would suggest using vagrant to develop in Linux if you are on a Windows machine. It is your responsibility to ensure the program runs as expected in the operational environment described. 

STEPS

Your program will be parsing and analyzing log files from an Apache web server. The first thing your program must do is retrieve the log file across the network. It is available here: https://s3.amazonaws.com/tcmg412-fall2016/http_access_log

Once you download the file, you will be parsing the file in order to answer several questions:
How many total requests were made in the time period represented in the log?
How many requests were made on each day?
What percentage of the requests were not successful (any 4xx status code)?
What percentage of the requests were redirected elsewhere (any 3xx codes)?
What was the most-requested file?
What was the least-requested file?
 
You will need to output this data to the screen. The format you choose to do this is up to you (human readable, machine readable, plain text, JSON, etc), but your decisions and the implementation should be logical and consistent. 

Finally, it was decided that the logs should be broken into separate files by day. Your program should split the log file into 14 smaller files, where the data stored in each file are the log events for a single day. These should be written to disk in the same directory as your program file, in a logical and consistent manner. 
Your program should be created and developed using GitHub (I will be examining the commit logs to see your work). When the project is due, you will add me (https://github.com/amikeal) to your repository so I can clone the repo and test your program. The project is due by 5pm on Friday, Oct 14th. 
