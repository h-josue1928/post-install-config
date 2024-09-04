# post-install-config

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



<h2>Configuration Steps</h2>


Step 1: Configure Roles

- Ensure you're under Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel') -> Agents -> Roles -> Add New role
- Add Name (Supreme Admin)
- Click the 'Permissions' tab and Check all boxes under Tickets\Tasks\Knowledgebase
- Click Add Role

![image](https://github.com/user-attachments/assets/4a4b7dde-e828-413a-827c-d6ed64d7faeb)

![image](https://github.com/user-attachments/assets/bee62109-4db3-4d8b-81e4-da2337e53a53)

![image](https://github.com/user-attachments/assets/9881cbf8-dbb7-49b8-87f4-9def8d4a0c2a)


  



Step 2: Configure Departments

- Ensure you're under Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel') -> Agents -> Departments
- Click 'Add New Department'
- In the name field enter System Administrators'
- Click 'Create Dept' at the bottom of the webpage

  ![image](https://github.com/user-attachments/assets/345bc221-80e4-4a41-81ae-11af1abe7518)



Step 3: Configure Teams

- Ensure you're under Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel') -> Agents -> Teams
- Click 'Add New Team'
- In the name field enter 'Level II Support' (Note: There should already be a 'Level I Support' team there)
- Click the 'Members' tab and add yourself to the team
- Click 'Create Team' at the bottom of the webpage






Step 4: Configure to allow anyone to create tickets

-  Ensure you're under Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel') -> Settings -> Users -> Settings
-  Make sure the 'Require registration and login to create tickets' box is unchecked




Step 5: Configure Agents (Help Desk Professionals)

- Ensure you're under Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel') -> Agents -> Add New Agent
- Add Agents Name\ Email Address\ Username
- Click 'Set Password' and deselect 'Send the agent a password reset email'
- Enter the Password (create your own) -> deselect 'Require password change at next login' -> click 'set'
- Assgin the department for the agent by click the 'Access' tab
- Select the department and the role
- Add the agent to the 'Level II Support' team that was created under the teams tab
- Click 'Create'
- Repeat steps to add a second agent
- Assign the second agent to the 'Support' department and 'View only' role under the 'Access' tab



Step 6: Configure Users (Customers)

- Switch to the Agent Panel (top right should say Admin Panel, which means you're in the 'Agent Panel') -> Users -> Add User
- Enter a made up email address and name -> Add User
- Go back to the 'User Directory' and add a second user by repeating the exact same steps
![image](https://github.com/user-attachments/assets/dd989cab-a9ed-47b0-b808-cc616442e3c4)


Step 7: Configure SLA

- Switch back to the Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel')  -> Manage -> SLA
- Click 'Add New SLA Plan'
- Add SEV-A (Grace Period: 1 hour) (Schedule: 24/7)
- Add SEV-B (Grace Period: 4 hours) (Schedule: 24/7)
- Add SEV-C (Grace Period: 8 hours) (Schedule: Business Hours M-F)
- Click 'Add Plam' at the bottom of the webpage


Step 8: Configure Help Topics

- Ensure you're under Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel') -> Manage -> Help Topics
- Click 'Add New Help Topic'
- The following topics:
    - Business Critical Outage
    - Personal Computer Issues
    - Password Reset
