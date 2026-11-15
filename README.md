# BRG-31-ISEA-Labs

BRG-31 Lab Activities

Lab 1a-1 Reflection Questions:
Q1: What challenges did you encounter during the virtual machine setup?
I was not used to the UI for creating a VM as I was more used to VMWare's UI. However, this challenge was not hard to overcome.

Q2: What did you learn about virtualisation tools and their differences?
I learned that tools like VirtualBox, VMware and UTM allow users to run different operating systems on a single computer. They may vary in performance, compatibility and available features.

Q3: How confident do you feel using Ubuntu after completing this lab?
I feel quite confident navigating Ubuntu, performing basic operations and understanding how to install and configure a Linux environment. However, I still need more time to practice CLI as it is not always the most intuitive.

Q4: In what ways can a virtualised Linux environment help in industry scenarios?
It allows developers and IT professionals to test applications, run servers and experiment with different operating systems without affecting their main system. It also provides a more cost-effective option for development and testing.

Q5: What would you do differently if setting up another VM?
I would plan the resource allocation beforehand. I would also ensure my network settings are pre-configured correctly.

Lab 1a-2 Reflection Questions:

Q1: Which file editors are best for remote access and why?
VS Code is best for general remote access because it supports SSH, has an integrated terminal and offers useful development tools and extensions. Vim and Nano are also useful for editing files directly through a remote Linux terminal, especially on servers due to their lightweight nature.

Q2: Compare software installation methods: SaaS vs binaries vs repositories vs source code.
SaaS is convenient because software is hosted online and maintained by the provider. Binaries are precompiled files that are easy to install and run. Repositories simplify installation, updates and dependency management through package managers. Source code provides the most flexibility and customization but requires more technical knowledge to compile and maintain.

Q3: What are the pros and cons of each method from user and developer perspectives?
From a user's perspective, SaaS and binaries are generally easier to use, while repositories offer convenient software management and source code provides greater control. From a developer's perspective, SaaS allows centralized updates, binaries simplify distribution, repositories provide structured distribution, and source code encourages collaboration. However, each method comes with different maintenance, security and compatibility challenges.

Q4: How did using CLI improve your understanding of Linux?
Using CLI helped me understand Linux by teaching me how to navigate directories, manage files, control permissions, install software and troubleshoot system issues. It also improved my confidence in using Linux without relying on a graphical interface which is important when executing commands or completing tasks with speed in mind on a lightweight, GUI-less setup.

Lab 1b-1 Reflection Questions:

Q1: What’s the role of a firewall in managing services?
A firewall controls incoming and outgoing network traffic. This serves to prevent unauthorized access while allowing necessary connections.

Q2: How did SSH access deepen your understanding of Linux as a server?
My usage of SSH showcased how Linux servers can be remotely accessed and managed through the CLI without requiring physical access. This is important for server administrators because managing multiple servers is inconvenient if the only way to access or configure them is to be physically present.

Q3: Why is file compression important in server contexts?
Compression reduces file sizes, saving storage space and making file transfers faster and more efficient. File sharing and storage will be forced to scale too much to accommodate uncompressed files accumulated over a long period of time.

Q4: How does user privilege management help secure systems?
It limits user access based on their permissions, preventing unauthorized changes and reducing security risks stemming from malicious intended access or accidental access.

Lab 1b-2 Reflection Questions:

Q1: How do Linux permissions differ from Windows ACL?
Linux uses read, write and execute permissions assigned to the file owner, group and others whereas Windows ACL provides more detailed control by allowing specific permissions to be assigned to individual users and groups. This is due to how Linux prioritizes simplicity and efficient permissions management in server environments over Windows' more flexible and complex environments where different users require varying levels of access or permissions.

Q2: What's the effect of chmod 770 vs 750?
770 gives the owner and their group full permissions to read, write, and execute. 0 refers to the access permissions given to others, which is none/deny.
750 gives the owner full rwx permissions, their group read and execute permissions, and deny all for others.

Q3: What is the risk of adding users to the sudo group?
Users in the sudo group can execute commands with administrative privileges. If it is misused or its security is compromised, they could modify system files or processes, access sensitive information, or damage the system completely.

Q4: Why is it important to verify with su and whoami?
su stands for switch user, and it is an important command to allow you to select which user you want to execute a command with. whoami confirms which user you're currently active on, which is important to run before important commands to ensure that you're on the intended user.

Lab 1b-3 Reflection Questions:

Q1: Which command-line tool was the most useful in solving the questions?
I found grep the most useful because it allowed me to search for specific words and phrases across multiple text files quickly. It made locating relevant information much easier.

Q2: How might these search tools help in cybersecurity investigations?
Tools like find and grep help investigators locate suspicious files, search for malicious code or keywords, and identify important information in system logs. They make analysing large amounts of data more efficient.

Q3: How could scripting improve repetitive search tasks?
Scripting can automate repetitive commands, allowing multiple files and directories to be searched automatically. This saves time, reduces human error and makes the investigation process more consistent.

Q4: What limitations did you encounter using grep and find?
grep may struggle with binary files, complex search patterns or different text formats. find can also return too many results when searching large directories, making it harder to identify relevant files. Both tools require familiarity with command syntax to use effectively.

Lab 2a-2 Reflection Questions:

<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/240e70f3-af8d-4c59-8265-b3ae794f6f56" />

Q1: What were the benefits of cloud deployment over local virtualisation?
Cloud deployment allows servers to be accessed from anywhere with an internet connection without relying on personal computer resources. It also offers scalability, flexibility and easier resource management compared to running a local virtual machine.

Q2: How does Apache serve files, and how did you verify this?
Apache acts as a web server that receives HTTP requests from users and delivers the requested website files, such as HTML, CSS and images. I verified this by entering the EC2 instance's public IP address into a browser and checking that my webpage loaded successfully.

Q3: What did you learn about file ownership and permissions?
I learned that Linux uses file ownership and permissions to control who can read, write or execute files. I also learned that administrative privileges using sudo may be required to modify protected directories such as /var/www/html/.

Q4: What risks are associated with leaving instances running?
Leaving EC2 instances running can result in unnecessary AWS charges, even when they are not being used. It can also create security risks if the instance is not properly configured or maintained. Therefore, unused instances should be stopped or terminated.

Q5: How would you explain the difference between DNS and /etc/hosts to a client?
DNS translates domain names into IP addresses using a network-wide naming system, allowing users to visit websites/servers using memorable and readable names, whereas /etc/hosts is a local file that manually maps domain names to IP addresses on an individual computer. DNS provides name resolution across networks, while /etc/hosts provides local name resolution and can override DNS results.
