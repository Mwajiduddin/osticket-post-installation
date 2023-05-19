<h1 align="center">osTicket: Post-Installation Configurations</h1>

<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png"/>
</p>

<h1>Introduction</h1>
This tutorial will show the ins and outs and configuration settings osTicket.<br />


<h2>Tutorial Guidelines</h2>

<h3>Step 1: Configuring Roles</h3>

The first thing that we're going to do in osTicket is to configure roles which are the permissions that Agents have access to, here we will create a role named "Supreme Admin." We start by clicking on the "Admin Panel" on the top right, if you see "Agent Panel" instead that means you are already in the Admin Panel. 

 <p align="center">
<img src="https://github.com/Mwajiduddin/Mwajiduddin/blob/main/images/f1.png" />
</p>

Select the "Agents" tab, click on "Roles" then "Add New Role", name it as "Supreme Admin", then go to the "Permissions" tab and tick every box under "Tickets", "Tasks", and "Knowledgebase" and hit "Save Changes."

 <p align="center">
<img src="https://github.com/Mwajiduddin/Mwajiduddin/blob/main/images/f2.png" />
</p>

 <p align="center">
<img src="https://github.com/Mwajiduddin/Mwajiduddin/blob/main/images/f3.png" />
</p>

<h3>Step 2: Configuring Departments</h3>

Tickets are assigned to specific departments or section of a company to be fixed, to create a department go to "Agents" tab, select "Departments" and click on "Add new department." Leave the "Parent" as "Top-Level Department", name it as "System Administrators, leave the rest as is and hit "Create Dept."

 <p align="center">
<img src="https://github.com/Mwajiduddin/Mwajiduddin/blob/main/images/f4.png" />
</p>

 <p align="center">
<img src="https://github.com/Mwajiduddin/Mwajiduddin/blob/main/images/f5.png" />
</p>

<h3>Step 3: Configuring Teams and Ticket Creation</h3>

In Teams you can assign different Agents from different Department to fix a specific problem and to create a Team go to the "Agents" tab, select "Teams", click on "Add new team", name it, go the "Members" tab, select the agent that you made and click on "Create Team." 

 <p align="center">
<img src="https://github.com/Mwajiduddin/Mwajiduddin/blob/main/images/f6.png" />
</p>

 <p align="center">
<img src="https://github.com/Mwajiduddin/Mwajiduddin/blob/main/images/f7.png" />
</p>
Once done go to the "Settings" tab, select "Users" and make sure that the box that reads "Require registration and login to create tickets" is unchecked so that anyone can create a ticket.

 <p align="center">
<img src="https://github.com/Mwajiduddin/Mwajiduddin/blob/main/images/f8.png" />
</p>

<h3>Step 4: Configuring Agents</h3>

Agents are the workers that resolve the tickets and to create an agent go to the "Agents" tab, select "Agents", click on "Add a new agent" and here we will create Jane Doe as our agent. 

 <p align="center">
<img src="https://github.com/Mwajiduddin/Mwajiduddin/blob/main/images/f9.png" />
</p>

Fill in the name, email address, username, click on "Set Password", uncheck the boxes that reads "Send the agent a password reset email" and "Require a password change at the next login", make note of the password you made because later on we will login as an agent then click on "Set." 

 <p align="center">
<img src="https://github.com/Mwajiduddin/Mwajiduddin/blob/main/images/f10.png" />
</p>

 <p align="center">
<img src="https://github.com/Mwajiduddin/Mwajiduddin/blob/main/images/f11.png" />
</p>

Go to the "Access" tab, under "Primary Department" select "System Administrators" under "Select Department" and select "Supreme Admin" under "Select Role". 

 <p align="center">
<img src="https://github.com/Mwajiduddin/Mwajiduddin/blob/main/images/f12.png" />
</p>

Under "Extended Access" select "Support" under "Select Department" and select "Supreme Admin" under "Select Role", go to the "Teams" tab, select "Level II Support" that you made under "Select Team", click "Add" then "Create." 

 <p align="center">
<img src="https://github.com/Mwajiduddin/Mwajiduddin/blob/main/images/f13.png" />
</p>

<h3>Step 4: Configuring Users and Service Level Agreements (SLAs) </h3>

Users are the customers with issue that needs to be fix, in this step we will create to users: Karen Smith and Ken Smith. To add a user, click on "Agent Panel" select "User Directory" under the "Users" tab and click on "Add user." 

 <p align="center">
<img src="https://github.com/Mwajiduddin/Mwajiduddin/blob/main/images/f15.png" />
</p>

 <p align="center">
<img src="https://github.com/Mwajiduddin/Mwajiduddin/blob/main/images/f16.png" />
</p>

 <p align="center">
<img src="https://github.com/Mwajiduddin/Mwajiduddin/blob/main/images/f17.png" />
</p>

Service Level Agreements (SLAs) are the amount of time that a issue needs to be fixed, in this step we will be create three separate SLAs with different grace periods for each to help you get an idea of a ticket's lifecycle. To start, go back to the Admin Panel, select on "SLA" under the "Manage" tab and click "Add New SLA Plan." 

 <p align="center">
<img src="https://github.com/Mwajiduddin/Mwajiduddin/blob/main/images/f18.png" />
</p>

The first SLA plan will have a grace period of one hour then select 24/7 under "Schedule" and click "Add Plan." The second SLA will have a grace period of four hours and a schedule of 24/7. The last SLA will have a grace period of eight hours and choose "Monday-Friday 8am-5pm with U.S. Holidays" for its schedule. 

 <p align="center">
<img src="https://github.com/Mwajiduddin/Mwajiduddin/blob/main/images/f19.png" />
</p>

 <p align="center">
<img src="https://github.com/Mwajiduddin/Mwajiduddin/blob/main/images/f20.png" />
</p>




<h3>Step 5: Configuring Help Topics (SLAs) </h3>

Help Topics are basically categories that an issue can be filed under so that it goes to the appropriate Agents to get fixed, here we will be making two help topics: Business Critical Outage and PC Issues. Go to "Admin Panel", select "Help Topics" under "Manage" and click on "Add New Help Topic." Then type in the name of the topic and hit "Add Topic."

 <p align="center">
<img src="https://github.com/Mwajiduddin/Mwajiduddin/blob/main/images/f21.png" />
</p>
 
  >**Note**: *In the next tutorial we will be playing around wtih osTicket and show how to create a ticket, change its parameters and resolve one so don't tear down your virtual machine just yet.*











