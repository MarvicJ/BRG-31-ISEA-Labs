Lab 2b-1 Reflection Questions:

Q1: What command did you use to create a new directory? I used the mkdir command to create a new directory. mkdir myfolder creates a folder named myfolder in the current working directory (showcased by running the pwd command).

Q2: How can you view the contents of a file without opening it in a GUI? Commands such as cat, less or head allow you to view file contents directly in the terminal without needing a graphical text editor.

Q3: What is the purpose of chmod 777? chmod 777 gives the file owner, group and other users full read, write and execute permissions. However, it can create security risks because anyone with access can modify or execute the file.

Q4: What does #!/bin/bash do at the start of a script? It is called a shebang. It tells the operating system to use the bash interpreter to execute the script. Changing this changes which interpreter is used. For example, you can use #!/bin/sh to run the script using POSIX or #!/usr/bin/python3 to use Python.

Q5: What happens when invalid input is entered into a script? The script may show an error, produce unexpected or incorrect results, or stop executing. Coding in 'if and else' statements can help handle invalid inputs.

Q6: What output does free -h show? It displays the system's memory usage, including total, used and available RAM, as well as swap memory. The -h option makes the values easier to read by using units such as MB and GB.

Q7: How would you monitor network bandwidth in a Bash script? I could use commands such as vnstat or ifstat to monitor network traffic and measure upload and download speeds. A Bash script could run these commands at regular intervals using a while loop and sleep to track bandwidth usage over time.

Using Duck DNS to Host my Apache Page: 
<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/04ccd104-6445-4d6b-9cde-e48205bc520d" />

Lab 2b-2: 
Hello World script: 
<img width="642" height="566" alt="image" src="https://github.com/user-attachments/assets/0ad67107-20b0-4e54-afb5-bf4e1753e168" />

System Info script: 
<img width="642" height="566" alt="image" src="https://github.com/user-attachments/assets/b01138dc-c58b-4572-8c55-8aed71179fdf" />

System Monitoring: 
<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/c4f8ea9c-5056-42ba-a35c-1582ed1b7c83" />


Lab 2b-2 Reflection Questions: 
What command did you use to create a new directory? 
mkdir is the command that is used to create directories. mkdir -p creates a directory and all missing parent folders needed to create the path.

How can you view the contents of a file without opening it in a GUI besed text editor? 
Use the 'cat' command to print the whole text file. 'less' to scroll through longer files, or 'head'/'tail' to inspect the first or last lines.

What is the difference between cp and mv commands? 
'cp' copies a file or directory, leaving the original in its place. mv moves a file or directory into a new path, or if the path is in the same directory, will rename the file instead.

What is the purpose of the chmod +x command? 
It adds an execute permission to allow a script to be executed. 

Why do we use the shebang (#!/bin/bash) at the beginning of scripts? 
It specifies what interpreter to use for the script. This shebang is using the bash interpreter. This ensures that the script runs Bash-specific syntax regardless of what shell is being used to launch it.

How can you modify the script to display a personalized message? 
Capture inputs with the 'read -p' (-p stands for prompt) line and then reference it in an echo. For example: 
read -p "Enter your name: " name
echo "Welcome, $name!"

How does the for loop in the script operate? 
It repeats a command for each item in a specified list or while a condition is in place which initializes a countdown.

What happens if a user enters a number greater than 10? 
The number would return as Out of range, as per the lab. 

How can you modify the script to handle invalid inputs gracefully? 
Validate the input before it is used, like checking for regex patterns using '^[0-9]+$' or using ranges like if/elif/else statements. You can then print/echo error messages accordingly and re-prompt the loop instead of letting the script exit.


What information does the free -h command provide? 
Information on Total, used, free, shared, buff/cache, and available memory

How can you modify the script to monitor network usage?
Read cumulative byte/packet counters from '/proc/net/dev', sample before and after a sleep interval, and divide the byte difference by the elapsed seconds to get transfer rates.

Why is automating system monitoring beneficial for administrators? 
It helps catch resource bottlenecking early and collects snapshots of the system information without manual effort. This allows the admins to focus on finding and fixing root-cause issues.
