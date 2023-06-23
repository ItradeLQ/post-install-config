<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)

<h2>Prerequisites</h2>

- Resource Group
- Virtual Machine
- Remote Desktop Connection
- Internet Information Services (IIS)
- osTicket

<h2>Post-Install Configuration Objectives</h2>

- In this section we will create and configure the osTicket environment.
- We will setup configurations as an admin.
- We will create roles, departments, teams, agents, and users.
- We will set up different SLAs and create help topics.

<h2>Configuration Steps</h2>

Login to the osTicket as an admin. Note that you can also switch between the admin and agent panel by clicking on the top right corner of the screen.

<a href="https://imgur.com/j27WMAA"><img src="https://i.imgur.com/j27WMAA.png" title="source: imgur.com" /></a>

A role is permission granted to agents (the person who will take care of the ticket) in the department that they have access to. Each role has a different set of permissions that can be checked or unchecked for the agent. Now we will create a role called “supreme admin” and will assign it to a user who will have access to everything.  
  
Admin Panel -> Agents -> Roles ->Add new role -> Supreme admin
  

After adding a new role go to the permission, check all of the boxes, click the task and check all of the boxes, click knowledgebase and check the box.


<a href="https://imgur.com/Cbo36IX"><img src="https://i.imgur.com/Cbo36IX.png" title="source: imgur.com" /></a>

The ticket gets associated with a department, and that specific department will take care of the ticket  
  
Admin Panel -> Agents -> Departments -> Add new department -> System Administrator


<a href="https://imgur.com/eU00iSZ"><img src="https://i.imgur.com/eU00iSZ.png" title="source: imgur.com" /></a>

  
Every department can have multiple teams
  

Admin Panel -> Agents -> Teams
  
  
Level I Support
  
  
Level II Support
  

Add level II support and in members add yourself.


<a href="https://imgur.com/wvt6qX4"><img src="https://i.imgur.com/wvt6qX4.png" title="source: imgur.com" /></a>


Admin Panel -> Settings -> User Settings
  
  
Next, click require registration and login to create tickets  
  

<a href="https://imgur.com/qfuh2o8"><img src="https://i.imgur.com/qfuh2o8.png" title="source: imgur.com" /></a>




An Agent is the person who solves the ticket.


Admin Panel -> Agents -> Add new 


You can add anyone to the agent list by creating their usernames, emails, and passwords. In this case I added Jane Doe and John Doe as agents
  

  
Jane Doe -> Access -> Set to System Administrators -> Set role to supreme admin -> Check permission -> Check teams and to level II support and create
  
  
John Doe -> Access -> support -> role set to view only -> Extended Access set to support and create



<a href="https://imgur.com/c06bGbH"><img src="https://i.imgur.com/c06bGbH.png" title="source: imgur.com" /></a>

We can also add End Users. End Users (also known as the customer) are the people who can create their own tickets.
  
  
Agent Panel -> Users -> Add New -> Ken 
 


<a href="https://imgur.com/QNtSqxQ"><img src="https://i.imgur.com/QNtSqxQ.png" title="source: imgur.com" /></a>

Add Karen and Ken to the end user.


<p><a href="https://imgur.com/deCKJZO"><img src="https://i.imgur.com/deCKJZO.png" title="source: imgur.com" /></a>


Service Level Agreement is the amount of time given to open, solve the problem, and close the ticket.

  
Admin Panel -> Manage -> SLA


<a href="https://imgur.com/LuAWyPz"><img src="https://i.imgur.com/LuAWyPz.png" title="source: imgur.com" /></a>

Add these three SLAs
  
Sev-A (1 hour, 24/7)
  
  
Sev-B (4 hours, 24/7)

  
Sev-C (8 hours, business hours, Monday - Friday 8am -5pm with Canada Holidays)
  

<a href="https://imgur.com/MBwi4Nn"><img src="https://i.imgur.com/MBwi4Nn.png" title="source: imgur.com" /></a>



End users can choose the problem they need help with. To do this go to the Admin Panel -> Manage -> Help Topics

Select from the list below:
  
- Business Critical Outage

- Personal Computer Issues

- Equipment Request

- Password Reset
</p>

Good job for making it this far into the osTicket Tutorial. In the [next tutorial](https://github.com/ItradeLQ/ticket-lifecycle.git), we will wrap up our mini-series on osTicket focusing on ticket-lifecycle.
