# DEVOPS
Devops Notes

What is DevOps?
==============
DevOps is a combination of Development (Dev) and Operations (Ops).
It is a culture, set of practices, and tools that helps organizations:

-> Deliver software faster
-> Automate processes
-> Improve collaboration between teams

====================================================================================

Software -> Application -> Source Code
	->Helping automate business
	
 Small online tiffin service[Food Ordering website]
 ==================================================

Without Devops:
--------------
-> Developer
-> Upload to the site(application,code) to a server(Operations)
-> works on Developer laptop, but crashes on the server
-> waiting for 2 weeks to fix a small change like 'add paytm payments'

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

-> Developers frequently merge or push (integrate) their code into a shared repository (like GitHub).
-> An automated build/test process checks for errors
-> Goal: Detect/Catch bugs early and keeping the code in a deployable state
		
Continuos Delivery/Deployment(CD):
---------------------------------
-> Automatically deploy the tested code to production environment
-> Goal: faster and reliable release
		
Realtime tools:
			Github/Gitlab - Code repository
			Jenkins/Githubactions - CI/CD pipelines
			Docker -  Packaging apps
			Kubernetes/AWS/GCP  - Deployment platforms

✅ Benefits of CI/CD:
--------------------
-> Faster and safer code delivery
-> Fewer bugs in production
-> Less manual work
-> Consistent deployment process
-> Quick feedback to developers

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
	Language is YAML,JSON kind of languages
	-"Install windows, enable firewall, install antivirus, block youtube,facebook"
	Now run that program - in 10 mins wholoe 200 machines are ready!!!
		
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
	
Machine 
	- Web Server
		- hosting a web application 
	- Database server
		- hosting huge data
		
Go to a restaurant and order Dosa
	. You - client
	. Kitchen - Servers
	. Order(Request) - Http Request
	. Dosa (Response) - Webpage, file
			
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
------------------------
   1.Ensuring system reliability (Maintain uptime, performance and availability)                											
   2.Define and SLA,SLO,SLI																				
   3.Automation of operations																				
   4.Improves system scalability and performance																	
   5.Security and Complaince																				

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
	
	
	
	
	








	




			











