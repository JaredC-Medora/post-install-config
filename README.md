<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration Guide</h1>
This guide will walk you through setting up key features of your osTicket system, including configuring roles, departments, teams, users, SLAs, and help topics. Follow these steps to manage your help desk efficiently.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Item 1
- Item 2
- Item 3
- Item 4
- Item 5

<h2>Configuration Steps</h2>


1. Access the Admin and End User Pages
   - Admin/Analyst Login Page:
     http://localhost/osTicket/scp/login.php
   - End Users osTicket URL:
     http://localhost/osTicket

<p>
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  
2. Understand Agent Panel vs Admin Panel
   - Agent Panel: Where agents (workers) manage tickets.
   - Admin Panel: Where administrators configure settings, roles, departments, and other system features.
<br />

<p>
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
3. Configure Roles (For Grouping Permissions)
 
   To manage permissions, configure roles for agents
   1. Go to Admin Panel > Agents > Roles.
   2. Create roles such as:
       - Supreme Admin for full access.
       - Other roles based on your requirements.

</p>
<br />

<p>
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
4. Configure Departments (Ticket Visibility)

   Departments control who can see and manage tickets. For example, SysAdmins may see system-related tickets, while Support handles customer service.
   1. Go to Admin Panel > Agents > Departments.
   2. Configure departments such as:
      - SysAdmins
      - Help Desk
      - Networking




5. Configure Teams (Group Agents from Different Departments)
Teams allow agents from different departments to work together on tickets.
   1. Go to Admin Panel > Agents > Teams.
   2. Create teams by selecting agents from different departments, e.g.:
      - Online Banking team with agents from Support and SysAdmins.




6. Allow Ticket Creation by Registered Users Only
To prevent unregistered users from creating tickets:
   1. Go to Admin Panel > Settings > User Settings.
   2. Uncheck the box for Unregistered users can create tickets.
   3. Enable Registration Required: Only registered users can create tickets.




7. Configure Agents (Add Workers)
Add agents to your help desk system:
   1. Go to Admin Panel > Agents > Add New.
   2. Add agents such as:
      - Jane (Department: SysAdmins)
      - John (Department: Support)
     



8. Configure Users (Add Customers)
Add users (customers) who will submit tickets:
   1. Go to Agent Panel > Users > Add New.
   2. Add users such as:
      - Karen
      - Ken




9. Configure SLA (Service Level Agreements)
SLAs define the response times for different severity levels:
   1. Go to Admin Panel > Manage > SLA.
   2. Configure SLAs such as:
       - Sev-A (Grace Period: 1 hour, Schedule: 24/7)
       - Sev-B (Grace Period: 4 hours, Schedule: 24/7)
       - Sev-C (Grace Period: 8 hours, Business Hours)




10. Configure Help Topics (For Ticket Submission)
Help Topics guide users when creating a ticket:
   1. Go to Admin Panel > Manage > Help Topics.
      - Create help topics such as:
      - Business Critical Outage
      - Personal Computer Issues
      - Equipment Request
      - Password Reset
      - Other


<h2>By following these steps, you'll be able to configure your osTicket system to handle roles, departments, teams, agents, users, SLAs, and help topics efficiently.</h2>
      
