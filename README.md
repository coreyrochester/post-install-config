<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Make Some configuration changes that will aid us to actually use osTicket
- Build an intuition on how the software works 


<h2>Configuration Steps</h2>

<p>
<img src="![image](https://github.com/user-attachments/assets/456a404a-cab5-4f01-b902-22bfb96f934d)
"/>
</p>
<p>
1. Configure Roles (for grouping permissions)
  Once logged into osTicket Click and Follow the tabs on screen in the oder shown down below 
Go to Admin Panel -> Agents -> Roles
Supreme Admin

2. Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)
Go to Admin Panel -> Agents -> Departments
SysAdmins


3. Configure Teams
Go to Admin Panel -> Agents -> Teams (Pull Agents from different Departments)
Online Banking


4. Configure Agents (workers) This step you're going to create some "Agents" follow the tabs down below and name them accordingly and group them with the dept. 
Go to Admin Panel -> Agents -> Add New
Jane (Dept: SysAdmins)
John (Dept: Support)

5.Configure Users (customers)
Go to Agent Panel -> Users -> Add New
Karen
Ken


</p>
<br />

<p>
<img src="![image](https://github.com/user-attachments/assets/45b4e407-0e4c-49c6-926e-80a36d461388)
"/>
</p>
<p>
Once you've configured all the roles, departments, teams, agents, and users it's time to make and configure the SLAs (Service Level Agreements) 
  again by clicking and following the tabs its says down below. You will be creating three DIFFERENT SLAs all with different levels severity and response times

 Go to  Admin Panel -> Manage -> SLA
create Sev-A (Grace Period: 1 hour, Schedule: 24/7)
create Sev-B (Grace Period: 4 hours, Schedule: 24/7)
create Sev-C (Grace Period: 8 hours, Business Hours)

  
</p>
<br />

<p>
<img src="![image](https://github.com/user-attachments/assets/c71127ec-a2b5-472a-9e8f-9eaf11168dc9)
"/>
</p>
<p>
Lastly, we're going to make it so that anyone can create a ticket and also configure the help topics to more accurately fit what our services provide. Once again follow the tabs and steps down below! 

 To Allow anyone to create tickets
Go to Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets)
Registration Required: Require registration and login to create tickets 

To Configure Help Topics (For when users create a ticket)
Go to Admin Panel -> Manage -> Help Topics
Make Sure you have the following help topics enabled: 
Business Critical Outage
Personal Computer Issues
Equipment Request
Password Reset
Other


</p>
<br />
