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

- Configure Roles
- Configure Departments
- Configure Teams
- Configure Agents
- Configure Users
- Configure SLA
- Configure Help Topics

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

<img width="865" alt="Screenshot 2025-03-12 at 3 13 47 PM" src="https://github.com/user-attachments/assets/f5f4e254-0e5e-4d41-b1fe-f6dd67494dbe" />

   - Admin Panel: Where administrators configure settings, roles, departments, and other system features.

<img width="864" alt="Screenshot 2025-03-12 at 3 14 12 PM" src="https://github.com/user-attachments/assets/c1896072-cc9b-460a-b114-2d9307d493f6" />

<br />

<p>
</p>
<p>
3. Configure Roles (For Grouping Permissions)
 
   To manage permissions, configure roles for agents
   1. Go to Admin Panel > Agents > Roles.
   
   <img width="866" alt="Screenshot 2025-03-12 at 3 14 42 PM" src="https://github.com/user-attachments/assets/283a0427-81b3-4604-ad62-0f6ac40b5113" />

   2. Create roles such as:
       - Supreme Admin for full access.
       - Other roles based on your requirements.

<img width="865" alt="Screenshot 2025-03-12 at 3 14 58 PM" src="https://github.com/user-attachments/assets/f427c541-5089-4993-a5e5-8bacb6f4e05d" />

</p>
<br />

<p>
</p>
<p>
4. Configure Departments (Ticket Visibility)

   Departments control who can see and manage tickets. For example, SysAdmins may see system-related tickets, while Support handles customer service.
   1. Go to Admin Panel > Agents > Departments
   2. Configure departments such as:
      - SysAdmins
      - Help Desk
      - Networking

<img width="865" alt="Screenshot 2025-03-12 at 3 15 26 PM" src="https://github.com/user-attachments/assets/24a298a1-0484-4121-9b50-2bbcc475f62b" />



5. Configure Teams (Group Agents from Different Departments)
Teams allow agents from different departments to work together on tickets.
   1. Go to Admin Panel > Agents > Teams.
   2. Create teams by selecting agents from different departments, e.g.:
      - Online Banking team with agents from Support and SysAdmins.

<img width="865" alt="Screenshot 2025-03-12 at 3 16 21 PM" src="https://github.com/user-attachments/assets/1e2f0e05-e3ae-483d-a896-b41c3660c7fa" />



7. Configure Agents (Add Workers)
Add agents to your help desk system:
   1. Go to Admin Panel > Agents > Add New.
   2. Add agents such as:
      - Jane (Department: SysAdmins)
      - John (Department: Support)
     
<img width="866" alt="Screenshot 2025-03-12 at 3 16 44 PM" src="https://github.com/user-attachments/assets/392d87a9-1abe-4eea-b977-42526aa101f1" />

<img width="862" alt="Screenshot 2025-03-12 at 3 17 14 PM" src="https://github.com/user-attachments/assets/0822abb1-009b-404b-ab16-1c2e96e76a7a" />

<img width="863" alt="Screenshot 2025-03-12 at 3 17 42 PM" src="https://github.com/user-attachments/assets/d7935641-2f27-4fd2-b9d6-264f19b37081" />

<img width="862" alt="Screenshot 2025-03-12 at 3 17 54 PM" src="https://github.com/user-attachments/assets/0647014d-6483-40a1-acf1-70f6f9ccfd01" />

8. Configure Users (Add Customers)
Add users (customers) who will submit tickets:
   1. Go to Agent Panel > Users > Add New.
   2. Add users such as:
      - Karen
      - Ken

<img width="582" alt="Screenshot 2025-03-12 at 3 18 45 PM" src="https://github.com/user-attachments/assets/fe0c1926-fb75-4065-bb61-31862a486a7c" />

<img width="575" alt="Screenshot 2025-03-12 at 3 18 57 PM" src="https://github.com/user-attachments/assets/2976f860-e726-43a1-a660-96e5365f5c65" />


9. Configure SLA (Service Level Agreements)
SLAs define the response times for different severity levels:
   1. Go to Admin Panel > Manage > SLA.
   2. Configure SLAs such as:
       - Sev-A (Grace Period: 1 hour, Schedule: 24/7)
       - Sev-B (Grace Period: 4 hours, Schedule: 24/7)
       - Sev-C (Grace Period: 8 hours, Business Hours)

<img width="864" alt="Screenshot 2025-03-12 at 3 19 15 PM" src="https://github.com/user-attachments/assets/c1ce928f-e0dd-4482-aeab-7789923906ba" />

<img width="861" alt="Screenshot 2025-03-12 at 3 19 27 PM" src="https://github.com/user-attachments/assets/338cd1a2-1ae7-41ee-9e04-a5f4216206d3" />

<img width="862" alt="Screenshot 2025-03-12 at 3 19 39 PM" src="https://github.com/user-attachments/assets/3fb913ec-33aa-4a44-9df7-bab1c13a556d" />

10. Configure Help Topics (For Ticket Submission)
Help Topics guide users when creating a ticket:
   1. Go to Admin Panel > Manage > Help Topics.
      - Create help topics such as:
      - Business Critical Outage
      - Personal Computer Issues
      - Equipment Request
      - Password Reset
      - Other

<img width="861" alt="Screenshot 2025-03-12 at 3 19 56 PM" src="https://github.com/user-attachments/assets/c6e22ec2-7330-410d-b26b-9a6e0fc44046" />

<img width="862" alt="Screenshot 2025-03-12 at 3 20 19 PM" src="https://github.com/user-attachments/assets/8aafa91c-7c71-4b2f-8eec-f76dfa72a9d3" />

<img width="862" alt="Screenshot 2025-03-12 at 3 20 33 PM" src="https://github.com/user-attachments/assets/ea2cb58f-db79-4a73-be83-25bae388a552" />

<h2>By following these steps, you'll be able to configure your osTicket system to handle roles, departments, teams, agents, users, SLAs, and help topics efficiently.</h2>
<h2>PLEASE DO NOT FORGET TO DELETE/PAUSE ALL VMs  IN AZURE TO REDUCE COSTS/CHARGES</h2>     
