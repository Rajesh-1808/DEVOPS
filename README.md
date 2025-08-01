# DEVOPS
Devops Notes

Complete software development process:
-------------------------------------
-> Example : facebook 
1. Programing : program written in programming languages, new funtionality, fix bugs
2. Software testing : new features, old code functionality, testers and developers test and automated testing
3. Release of software : build application, run on servers, upgrade existing software
4. Operations : run software in production

Traditional Development vs Operations :
--------------------------------------
- Development -> Release -> Operations
- Development team handle the development and testing  : programming languages, DB etc
- Operations team handle no downtime and handle huge traffic : OS, Linux, Scripts etc
- There is no proper communication between the Devolopment and the operations team.
Result : the solution is Devops Culture

What is DevOps?
==============
DevOps is a combination of Development (Dev) and Operations (Ops).
It is a culture, set of practices, and tools that helps organizations:

- Deliver software faster
- Automate processes
- Improve collaboration between teams

====================================================================================

Waterfall vs Agile:
===================
Traditional waterfall       |             Agile Methodology
----------------------------|---------------------------------------    	
Requirements		    |		Define 
Development		    |		Analyze
Testing		    	    |		Test (CI/CD)
Operations		    |		Design and Deploy
Ineffective process	    |		Effective process
More time		    |		Less time

Software -> Application -> Source Code
	- Helping automate business
	
 Small online tiffin service[Food Ordering website]
 ==================================================

Without Devops:
--------------
- Developer
- Upload to the site(application,code) to a server(Operations)
- works on Developer laptop, but crashes on the server
- waiting for 2 weeks to fix a small change like 'add paytm payments'

Result :  Delays,frustration,blame

What DevOps Brings to this situation
-------------------------------------

DevOps - 'Let's work together, automate the boring stuff and keep improving continuosly'
	- Developer + Operations collaborate from day one
	- Testing happens automatically before deploying [Upload to the server]
	- Updates are sent to the live site with one click
	- You track issues with alerts if site is slowing down
	
End Result: Customers are happy,food get delivered on time 	
=====================================================================================

Why DevOps is important?
------------------------

Without Devops 					     |		      With DevOps
-----------------------------------------------------|----------------------------------------------------------
you cook, others don't know what's cooking	     |	       Everyone helps prepare and serve
you pack late, delivery is delayed		     |          packing and delivery is automated
you don't know if customers got the food	     |          You get live delivery feedback



Developers and operations teams work together , automate the process and ensure
	1. Faster updates
	2. Fewer bugs
	3. Happier users
	
	
Feature				  |  Traditional IT 	|			Devops approach	
----------------|-------------------|---------------------
Delivery Speed	|	 Slow(months)			|	  Fast(hours/days)
Collaboration		|  Siloed teams			|  cross-functional teams
feedback loops	|	 Delayed					|  	Continuos
Manual work			|    High						|    Automated

=====================================================================================

Benefits of DevOps:
-------------------
1. Faster time-to-market(You can release features quickly)
2. Better Quality(Automated testing reduce bugs)
3. Stable systems (Monitoring(Proactive & Reactive) and quick recovery)
4. Cost efficiency(Fewer production issues)
5. Happier teams and customer satisfaction(less stress, more ownership)
6. Early bug detection

=====================================================================================

CI and CD : 
=========
-> CI/CD is a DevOps method that helps you automate the steps involved in developing, testing, and deploying software.

CI - Continuos Integration 
CD - Continuos Deployment

Online coaching class - need add new chapters and corrections often.


Without CI/CD:
	- Manually copy content to the website
	- One typo break entire page
	- students can't access notes
CI/CD	:
	- you upload the content(code)
	- It gets tested(CI) for typos,links
	- Then gets automatically published
	- no downtime, no panic
	
Continuos Integration(CI):
--------------------------
- Developers frequently merge or push (integrate) their code into a shared repository (like GitHub).
- An automated build/test process checks for errors
- Goal: Detect/Catch bugs early and keeping the code in a deployable state
		
Continuos Delivery/Deployment(CD):
---------------------------------
- Automatically deploy the tested code to production environment
- Goal: faster and reliable release
		
Realtime tools:
---------------
- Github/Gitlab - Code repository
- Jenkins/Githubactions - CI/CD pipelines
- Docker -  Packaging apps
- Kubernetes/AWS/GCP  - Deployment platforms

Benefits of CI/CD:
--------------------
- Faster and safer code delivery.
- Fewer bugs in production.
- Less manual work
- Consistent deployment process
- Quick feedback to developers

Examples :
---------
I. 4 freinds are cooking meal for festival . Each person is making a different dish
	1. biryani - Ravi
	2. paneer butter masal - Asha
	3. Gajar halwa -    Neha
	4. Chapathi    -  Arjun
They each prepare their dishes in their own kitchen(seperate branch) 
Once ready, they bring all the dishes to the main table[Shared repository]	and combine them into Thali

II. Online tiffin booking --- Website

Developer 	|	  Feature they work on 		  |    BranchName
------------|-----------------------------|--------------------
Asha		    |      	Login page					  |   login-feature
Ravi			  |      Booking system				  |   booking-feature
Neha			  |      Payment integration		|	   payment-feature
	
Once tested, they merge their branch into the main branch[share repository]	

III. Mobile App Updates :
-> Think of your phone's apps (Instagram, Zomato) updating every week.
-> Behind the scenes, DevOps pipelines:
                        1.Run automated tests
                        2.Build the new version
                        3.Deploy it to the App Store or Google Play

==========================================================================================================================================================================
	

IaC - Infrastructure as Code
============================

College 
	- Computer lab and admin
A new batch of students
	- setup a physical computer
	- Manually install windows
	- setup antivirus, software,network	
It takes almost a week to setup the infrastructure(machines)
	
Instead, I will write a program(Scripts)
	-Language is YAML,JSON kind of languages
	-"Install windows, enable firewall, install antivirus, block youtube,facebook"
	-Now run that program - in 10 mins wholoe 200 machines are ready!!!
		
That's what is IaC for your infrastructure(Servers)
		
Tools used:
	. Terraform 
	. AWS cloud formation

Benefits of IaC:
---------------

Manual Setup 				|			IaC
----------------------------------------|------------------------------------------------------
Click,click, forget settings		|		Script(program) remembers everything
Error happen ofen			|			Reproducible and reliable
Time consuming				|			Automated
Hard to scale				|			one script - 200 machines
					
		
Server
	- Computer, VM[Machines]
	- Software [Yes]	
-> Machine hosting a web application - Web Server	
-> Machine hosting huge data - Database server
				
Go to a restaurant and order Dosa
	. You - client
	. Kitchen - Servers
	. Order(Request) - Http Request
	. Dosa (Response) - Webpage, file

DEVSECOPS:
=========
Scanning of code using SonarQube for vulnerbailities.
Coding, Deployment to server.
-> Security - Application (trading app) security.

Vulnerbilities:
---------------
1. Username password - shouldn't be exposed.
2. Code - Hardcode password.
3. Weak Password
4. Poor Access Control
5. Not allowing developers to write insecure code
6. Unwanted user is trying to access your server [Hacking]

=====================================================================================
   
SRE - Site Reliability Engineering
==================================
SRE is about using code to manage and automate operations, ensuring systems stay up, run fast, and recover quickly.

Practice
-> Maintains the reliablity, availablity and performance of systems(set of servers)
	Reliable (doesn't crash frequently)
	Available (Users can access it anytime)
	Performant (responds quickly)
	SRE = Making sure website/apps work all the time, and work fast
	
	IRCTC
	Railway system = servers + application
	passengers = users
	Train Control system = SRE team
		- IRCTC to book a train ticket
		- Site crash or service unavailable
	SRE steps in
		- Automate operations like monitoring, alerting and scaling
		- track uptime and error rates		

	Managing a water purifier plant 
		- ensure clean water is available 24x7
		- if pressure drops or TDS increases an alarm goes off
		- you fix before people complain it

		
SRE would
	- Add autoscaling more servers spin up when traffic spikes
	- Set Alerts if CPU usage > 80%
	- Track SLOs (eg 99.99% uptime goal)

SRE Tools:
----------
1. Monitoring - Prometheus, Grafana (Used for: Tracking uptime, response times, error rates, etc.)
2. Alerting - AlertManager, PagerDuty (Used for: Notifying the right people when something breaks.)
3. Logging - Splunk ,ELK (Used for: Understanding what happened during failures.)
4. Automation - Ansible , Terraform (Used for: Automating deployment, scaling, and infrastructure provisioning.)


-> Devops - "Let's build and release software efficiently"												   				
-> SRE = "Let's ensure it runs smoothly , all the time"																	

-> Devops emphasize on speed + automation																		
-> SRE emphasize on stability + reliability																		

 DevOps	 						  |			SRE
----------------------------------------------------------|-------------------------------------------------------------
A culture to improve collaboration between dev & ops	  |      An engineering approach to operations reliability
Faster delivery + automation + collaboration	          |  	System reliability, uptime, and performance
Broad (includes CI/CD, IaC, Monitoring)			  |		Focused on SLAs, incident response, and automation
Jenkins, Docker, Terraform, GitHub, etc.		  |	SLOs, SLIs, Error Budgets, Monitoring, Alerting

Swiggy:
------
-> DevOps helps you deploy updates fast and automate the process
-> SRE makes sure the app stays available, fast, and reliable even during peak traffic

SLA (Service Level Agreement) – what you promise to users

SLO (Service Level Objective) – internal goal (e.g., 99.9% uptime)

SLI (Service Level Indicator) – actual measurement (e.g., response time)

Responsibilities of SRE:
-----------------------
1. Ensuring system reliability (Maintain uptime, performance and availability).
2. Define and Monitor SLA,SLO,SLI.
3. Automation of operations.
4. Improves system scalability and performance.
5. Security and Complaince.


   Principle			|			Description
--------------------------------|----------------------------------------------------------------
Embrace Risk			|	Use error budgets to balance speed and safety
SLOs, SLIs, SLAs		|	Set clear targets for reliability
Eliminate Toil			|	Automate repetitive manual tasks
Monitoring & Observability	|	Understand system behavior in real time
Automate Everything		|	Use tools/scripts to manage operations
Incident Management		|	Handle failures and learn from them
Simplicity			|	Build systems that are easy to understand

=====================================================================================

CI/CD:
-----
-> Set of practices to automate building, testing and releasing software quickly and reliably
	
  Principles of CI/CD			|		Meaning
----------------------------------------|----------------------------------------------------------------
 Frequent Code Integration(CI)		|	Developer merge code to a shared repository mutiple times
 Automated Testing			|	Code is automatically tested every time it changes
 Automated Build			|	After testing, the app is compiled and packaged automatically
 Continuos delivery			|	code is ready for deployment
 Fast feedback				|	Developer gets alert if something fails
 Rollback and Recovery			|	can easily undo a bad release
 Continous deployment                 	| 	code is automatically pushed to production after all tests gets passed


=================

CICD strategies:
----------------
1. start with continuos integraion
	- Developers push code to GithUb
	- pipeline(Jenkins) run unit tests automatically
- Goal: Catch bugs early, ensure team code works together.
	 
2. Add testing and quality gates
		- tools like SonarQube or JUnit to check
				* Bugs
				* Code Quality
				* Security vulnerabilities
- Goal: Ensure only high-quality, secure code moves forward.

3. Add Continous Delivery
		- Code that passes all checks is deployed to staging server(Testing environment)
- Goal: Always have a release-ready build with safe, manual control.
   
4. Move to Continous deployment
	- Auto-deploy to production if all test passes
- Goal: Deliver features to users quickly, with full automation.	

==========================================================================================================================================================================
	
JENKINS INSTALLATION : 
====================
CICD pipeline - tool Jenkins
	- Build
 	- Test 
  	- Deploy
	
	
1. JDK 17
2. Admin access on your windows machine
3. Set JAVA_HOME and set path environment variable
4. Download the jenkins from https://www.jenkins.io/download
5. download the  .msi installer(Windows installer)
6. Install Jenkins as a Windows Service
7. Unlock Jenkins initial setup
	http://localhost:8080
8. you'll see a screen asking for the administrator password
9. Go to C:\Program Files\Jenkins\secrets\initialAdminPassword
		open the file and copy the password
		paste it into the browser to unlock Jenkins
10. Install Suggested plugins[Recommended]
11. Create First Admin user
	Provide
		- Username
		- Password
		- FullName
		- Email
	Click Save and Finish
12. Jenkins Dashboard - http://localhost:8080	
	
===========================================================================================================================================================

Vagrant Commands:
=================
For windows:
------------
1. VBoxManage --version
2. vagrant --version
3. mkdir test-vm
4. cd test-vm
5. vagrant init hashicorp/bionic64
6. vagrant up

For Mac:
--------
It is done through Docker.
1. vagrant --version
2. mkdir test-vm
3. cd test-vm
4. nano Vagrantfile
   code :
   # Vagrantfile

Vagrant.configure("2") do |config|
  config.vm.provider "docker" do |d|
    d.image = "rastasheep/ubuntu-sshd:22.04"
    d.remains_running = true
  end

  config.vm.hostname = "docker-vm"
  config.vm.network "forwarded_port", guest: 22, host: 2222
end
5. vagrant up --provider=docker
6. vagrant ssh
7. It is used to connect to the VM through Vagrant and acces the linux to work on the commands.

=======================================================================================================================================

Operating System:
=================
- An Operating System is software that manages computer hardware and software resources, providing common services for computer programs.
- It is mainly used to do the communication between the hardware and the applications (translator)
- Managers resources among applications
- Isolates the contents of the application or resource management

Tasks of an OS:
---------------
1. Resource Allocation and Management (Process management, Memory management, Storage management
2. Manage File System
3. Management of I/O Devices
4. Security and Networking

OS Components:
-------------
- Hardware
- Kernel (different for each device like MacOS :Darwin and Android : Linux)
- Application layers
- User Apps

===================================================

Linux :
======
- Mostly used OS for servers
- Everything in linux is a file
- Knowing Linus is must for Devops Engineer
	- You need to work with servers
   	- Installing and configuring servers
   	- Lunix native Technologies (Ubuntu is most popularly used)

Virtualization:
==============
- No separate hardware needed beacause we use Virtual Machine: that is we can use windows+Linus or Mac+Linus
- The VM's can be accessed through Hypervisor(Virtual Box)
- VirtualBox takes hardware resources from Host OS
- Creates virtual CPU, virtual RAM, virtual storage for each virtual machine
- Hardware resources are shared
- Virtual Machines are completely isolated (Dont see Each other) 
	- If VM has damaged it does not effect our host Machines or our main os
  	- Learn and Experiment
  	- Test your app on different OS
- Why are comapnies adopting virtualization?
  	- Abstraction of the OS from the hardware
  	- Backups of entire OS
  	- Secure
  	- Portable
  	- Not Dependant

Linux File System:
------------------
1. Heirarchical Tree Structure
2. Each user has its own place and configuration if multiple users
3. Programs installed system wide are available for all users on that computer including applications and commands
4. Binary : Compuyter readable format (bin : cp, mv, etc)
5. System related commands (sbin : adduser, pswd, etc)
6. All users on the sytsem can use the installed applications (usr : bin, sbin, lib, etc)
7. Third party programs (opt)
8. Applications like Docker, java, python (local)
9. Contains files required for booting (boot) it is onky for system nit for users
10. System-wide Configurations are stored (etc)
11. Location of devices (dev : Drivers)
12. Contains log files (var -> log)
13. External media (media)
14. Hidden files are also called as Dot files in UNIX(.dot) they are automatically generated at the time of installing applications.
15. Every files has 2 owners one is user and the group

GUI vs CLI
----------
- GUI = A graphical user interface, where we have graphical elements that you can interact with, like buttons (terminal) (not on servers)
- CLI = Command line interface, where users type in commands and see the results on the screen (Command prompt) (present on servers)
- Terminal = The GUI window that you see on the screen. It takes commands and shows output.
- There are 3 types of user in Linux : 
- $ means normal user (Standard user)
- # means root user Super user (administrator)
- Service user (Linux server distributors)

Directory Functions:
--------------------
1. pwd - show current directory (present working directory)
2. ls - list
3. cd - change directory
4. mkdir - make directory
5. touch - create a file which is empty
6. rm - remove file
7. rmdir (rm -r) - remove directory
8. cd .. - back to home directory or main folder
9. cd / - going to root folder
10. clear - clean terminal
11. cd ~ - home directory
12. mv - moving files from folder to folder
13. cp - copyt file
14. ls -R - documents in every directory come
15. history - command you used in that session
16. ctrl + r (keys) - search for commands
17. ctrl + c (keys) - kill current command
18. history 20 - gives last 20 commands
19. ls -a - all the files and folders are displayed including hidden files
20. cat - display file content
21. uname -a - show system and kernel
22. adduser - to add a user or create a new user
23. sudo - Allows regular users to run programs with the security privilages of the superuser or root
24. groupadd - to create a group or add group
25. su - admin - used to sign as admin user (change admin to username for switching users)
26. apt - used to install softwares
27. apt update - used to update the applications
28. nano - used to create and edit the content in a file
29. passwd - change password for user
30. deluser - to delete a user
31. sudo usermod -g devops tom - makes devops primary group to tom
32. delgroup - delete the group
33. sudo usermod -G admin tom - to make tom admin
34. groups - displays the groups that the user is a member
35. ls -l - print files in a long list format
36. chown <username>:<groupname> <filename> - used to change owner
37. chgrp : used to change group
38. chmod -x <filename> - to change file to executable file
39. chmod g-w & g+w - removing and adding group write permissions
40. | - pipe command : it is the concept of passing the output to next command
41. grep - globally stand for Regualar expression and print. Search for a particular pattern of characters and display all lines that contain the pattern
42. history | grep sudo - gives all the commands that has sudo
43. > - redirector operator, we can move the commands to new file (history | grep sudo > sudo-commands.txt - all these sudo commands are moved and redirected to this file)
44. >> - append text to end of the file
45. less - is a powerful pager program used to view the contents of a text file or the output of another command, one screen at a time

Permissions:
------------
  d              rwx      rwx        -       x
file type	owner    group		   other

- + : add permission
- - : remove permission
- u - user
- g - group
- o - other
- a - all users

Binary format for permissions :
7  0   0
- 7 : user - 4(write) + 2(read) + 1(execute)
- 0 : group - 0(no permisiion)
- 0 : other users - 0(no permisiion)

1. d : directory(file type)
2. - : no permission
3. r : read
4. w : write
5. x : execute
 
When to use CLI over GUI?
-----------------------
- Work more efficient
- Easir for bulk operations like create, move, etc
- CLI is more powerful

How to install software on Linux?
--------------------------------
- Using a package manager
	- Software package contains all the dependencies required by the software in different files and folders
   	- downloads, updates and installs all the required files and dependencies for the software
   	- Easy upgrading of the software
   	- Package manager is in-built in Linux (ubuntu : apt - advance package tool)
   	- Pacakge manager fetches the packages from Repository(warehouse) this is most popularly used by Linux
 - sudo apt - for installation of software from root
 - sudo apt remove - for uninstalling of software from root
 - apt-Get is also a package manager but some complicated than apt because apt is more user friendly
 - apt is mostly used package manager in Linux. apt dependencies are shared and has manual updates and smaller installation sizes than any other package managers
 - intellijIDEA and snap are alternate package manager for Linux id apt doesn't work
 - Debian based : Ubuntu, Debian, Mint :- apt, apt-get
 - Red had based : RHEL, CentOS, Fedora :- yum

VIM editor:
----------
- It is an in-built Unix text editor
- It is popularly called as VI(visual instrument) or VIM(modified version of VI)
- Used in CLI
	- Faster to create and edit at same time
 	- Supports multiple formats
    	- Small modifications can be faster
- sudo apt install vim - to install the vim
- vim has 2 modes
  	1. Command mode : default, cant edit text
  	   	- dd - delete an entire line
  	   	- d10 + d -  to delete 10 line
  	   	- u - undo the changes
  	   	- A - Jumping to the end of the line of program
  	   	- 0 - Jumping to the begining of the line of program
  	   	- $ - end of the line
  	   	- 12G - to goto line 12
  	   	- /pattern - to search in the editor(pattern place name what you want to serach)
  	   	- n - jump to next match
  	   	- N - search in opposite direction
  	   	- :%s/old/new - replace the string old with new throughout the file
  	   	- :wq - to write, save and quit
  	2. Insert mode : allows to enter text. By pressing i on opening the file in vim we enter into the insert mode
- You can create any kind of file format by using this text editor

======================================================================================================

Shell Scripting:
===============
- It contains a bunch of commands in file that need to be executed at a time to avoid repetitive work and those commands can be shared just by sharing the file. Such files are called as Shell Scripts.
- Shell scripts have .sh file externsion
- Shell : The program that interprets and executes the various commands that we type in the terminal and translates our command that the OS kernel can understand
- sh : Bourne shell
- Bash : Bourne again shell. Improved versions of sh and is default shell program for most Unix like systems. Bash is a shell program and It is a programming language.
- #!/bin/bash : It is known as shebang. Basically it access the interpreter of the shell.
- echo : It is similar to print statement
- chmod +x setup.sh -> ./setup.sh (or) sh setup.sh : used to execute the bash file
- variable_name=value : Assigns the value to the variable
- $variable_name : used to reference the variables
- variable_name=$(command) : Store output of a command in a variable
- if [ -d "condition" ] then (after the statement) elif [ -d "condition" ] then (after the statement) else (after the statement) fi : -d means test if exists. It is for ifelse or elseif statement.
- File test Operators - to test various properties associated with a file and below all are booleans(if yes returns as true)
  	- -b file : cheks if file is a block special file
  	- -c file : check if file is a character special file
  	- -d file : check if file is a directory
  	- -f file : check if file is a ordinary file
  	- -g file : check if file has its group id bit set
  	- -k file : check if file has its sticky
  	- -p file : check if file is a named pipe
  	- -t file : check if file descriptor is openend and associated with a terminal
  	- -u file : check if file has its Set User id
  	- -r file : check if file is readable
  	- -w file : check if file is writable
  	- -x file : check if file is executable
  	- -s file : check if file has size greater than 0
- Operator used on numbers:
	- -eq : equal operator (condition becomes true)
	- -ne : not equal operator(condition becomes true)
	- -gt : checks if left operand is greater than the right operand
	- -lt : checks if left operand is less than the right operand
	- -ge : checks if left operand is greater than or equal to the right operand
	- -le : checks if left operand is less than or equal to the right operand
- Operator used on String :
  	- = : equal operator(condition becomes true)
  	- != : not equal operator(condition becomes true)
  	- -z : checks if given string operand size is zero
  	- -n : checks if given string operand size is non-zero
  	- str : checks if str is not empty string
- user_group=$1 : argument parameter that is passed to the bash script at the time of executing file $1 represents the 1st argument
- coonfig_dir=$2 : argument parameter that is passed to the bash script at the time of executing file $2 represents the 1st argument
- sh setup.sh bin config : examle of executing the file with argument parameters where 1st argument is bin and the 2nd argument is config
- read -p user_pwd : used to read the argument parameters in the file and the user_pwd stores the password.The -p option allows you to specify a prompt.
- echo "all parms $*" : argument parameter that is passed to the bash script at the time of executing file $* takes ample number of parameters
- Loops(to execute a command repeated no. of times) in Linux :
	- break : exist form a for, while, select or until loop 
	- For loop :
   		- for param in $* (next line) do (next line) echo $param (next line) done : execute all the parameters until nothing is left in the list. $# is a special variable that 		expands to the number of positional parameters (arguments) passed to a script or a function.
        - While loop : Executes a set of commands repeatedly until some comdition is matched
         	- while condition (next line) do (next line) statements to be executed if command is true (next line) done
         	- Infinite loop : while true (next line) do (next line) read -p "enter score" $score (next line) sum=$sum+$score (next line) done
         	
       		






	




			











