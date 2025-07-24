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

Without Devops 							                                               With DevOps
---------------                                                            -------------
you cook, others don't know what's cooking		                	        Everyone helps prepare and serve

you pack late, delivery is delayed		                                  packing and delivery is automated

you don't know if customers got the food	                      	      You get live delivery feedback



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
	












