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

- Windows 10</b> (21H2)

<h2>Prerequisites</h2>

- Resource Group
- Virtual Machine
- Remote Desktop Connection
- Internet Information Services (IIS)
- osTicket

<h2>Post-Install Configuration Objectives</h2>

- In this section we will create and configure the osTicket environment.
- We will setup stuff as an admin.
- We will create role, department, team, agents and users.
- We will setup different SLA’s and create some help topics.

<h2>Configuration Steps</h2>
</p>
<p>
Login to the osTicket as an admin. Note that you can also switch between admin and agents panel by clicking on the top right corner of the screen.
</p>
<br />
<p>
<img src="https://i.imgur.com/ShJmDqO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
A role is the permission granted to agents (the person who will take care of the ticket) in the department that they have access to. Each role has a different set of permissions that can be checked or unchecked for the agent. Now we will create a role called “supreme admin” and will give people who have this “supreme admin” role access to everything.  
  
Admin Panel -> Agents -> Roles
Add new role>Supreme admin
  

After adding a new role go to the permission and check all of the boxes, click task and check all of the boxes, click knowledgebase and check the box.

</p>
<br />

<p>
<img src="https://i.imgur.com/gL3PXY1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
The ticket gets associated with a department, and that specific department will take care the ticket  
  
Admin Panel -> Agents -> Departments
Add new department>System Administrator

</p>
<br />

<p>
<img src="https://i.imgur.com/X9CgYtn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  
Every department can have multiple teams
  

Admin Panel -> Agents -> Teams
  
  
Level I Support
  
  
Level II Support
  

Add level II support and in members add yourself.


</p>
<br />

<p>
<img src="https://i.imgur.com/CBGcTRq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Admin Panel -> Settings -> User Settings
  
  
Next, click require registration and login to create tickets  
  
</p>
<br />
<p>
<img src="https://i.imgur.com/tXl04pT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>



Agent is the person solve the ticket.


Admin Panel -> Agents -> Add new 


you can add anyone to the agent list by creating their usernames, emails, and passwords. In this case I added Jane Doe and John Doe as agents
  

  
Jane Doe  
Access> Set to System Administrators>Set role to supreme admin>check permission>check teams and to level II support and create
  
  
John Doe 
Access>support>role set to view only>Extended Access set to support and create


</p>
<br />

<p>
<img src="https://i.imgur.com/uwwXNBM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

We can also add End Users. End Users (also known as the customer) are the people who can create their own tickets.
  
  
Agent Panel -> Users -> Add New

Karen 
 

  
</p>
<br />

<p>
<img src="https://i.imgur.com/hgxaaOQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Add karen and ken to the end user.
</p>
<br />

<p>
<img src="https://i.imgur.com/TTGKh4f.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

SLA is the amount of time given to open, solve the problem, and close the ticket.

  
Admin Panel -> Manage -> SLA


</p>
<br />
<p>
<img src="https://i.imgur.com/1GRonhI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Add these three SLA's
  
Sev-A (1 hour, 24/7)
  
  
Sev-B (4 hours, 24/7)

  
Sev-C (8 hours, business hours)
  
</p>
<br />

<p>
<img src="https://i.imgur.com/7yNI5Gi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>


End users can choose the problem they need help with. To do this go to the Admin Panel -> Manage -> Help Topics

  
Business Critical Outage

  
Personal Computer Issues

  
Equipment Request

  
Password Reset

</p>
<br />

<p>
