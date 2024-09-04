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

  ![image](https://github.com/user-attachments/assets/36e9eab5-e52c-4187-bfa9-2415c9efc967)




Step 3: Configure Teams

- Ensure you're under Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel') -> Agents -> Teams
- Click 'Add New Team'
- In the name field enter 'Level II Support' (Note: There should already be a 'Level I Support' team there)
- Click the 'Members' tab and add yourself to the team
- Click 'Create Team' at the bottom of the webpage

  ![image](https://github.com/user-attachments/assets/4e179d13-0573-4a59-9814-be6ac2210de8)

  ![image](https://github.com/user-attachments/assets/94d7ea55-f2fd-4da0-9270-5e642e7005ca)

  ![image](https://github.com/user-attachments/assets/abd838bd-32e0-4157-be11-78ae76d8c93a)




Step 4: Configure to allow anyone to create tickets

-  Ensure you're under Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel') -> Settings -> Users -> Settings
-  Make sure the 'Require registration and login to create tickets' box is unchecked

  ![image](https://github.com/user-attachments/assets/c25c0d0f-7f3a-48df-8e40-fc93e7afce32)




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

  ![image](https://github.com/user-attachments/assets/5c058061-5fbc-4b2b-8e57-891d2d71acb8)


![image](https://github.com/user-attachments/assets/ffa63b87-6803-443e-9d7b-67e5e26993c2)

  
  ![image](https://github.com/user-attachments/assets/83ec12c8-8240-4530-8ec5-43a2a5c23570)

  
  ![image](https://github.com/user-attachments/assets/2a62cc5f-a2b7-489c-92e4-764441466367)


  ![image](https://github.com/user-attachments/assets/c6180f56-bea6-45b4-97ec-e65ae08fd131)





Step 6: Configure Users (Customers)

- Switch to the Agent Panel (top right should say Admin Panel, which means you're in the 'Agent Panel') -> Users -> Add User
- Enter a made up email address and name -> Add User
- Go back to the 'User Directory' and add a second user by repeating the exact same steps

![image](https://github.com/user-attachments/assets/39171cd4-e7f8-4371-80af-3bd2893147fb)

![image](https://github.com/user-attachments/assets/500e4023-450f-4d60-bf3b-806afa0922f8)

![image](https://github.com/user-attachments/assets/8ff892ae-47f8-4186-8329-9246deb35794)




Step 7: Configure SLA

- Switch back to the Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel')  -> Manage -> SLA
- Click 'Add New SLA Plan'
- Add SEV-A (Grace Period: 1 hour) (Schedule: 24/7)
- Add SEV-B (Grace Period: 4 hours) (Schedule: 24/7)
- Add SEV-C (Grace Period: 8 hours) (Schedule: Business Hours M-F)
- Click 'Add Plam' at the bottom of the webpage

![image](https://github.com/user-attachments/assets/4f247231-564a-4a98-a9ea-d4aa9e0cedb6)

![image](https://github.com/user-attachments/assets/286c6b02-cc08-46df-b6d5-41921227c298)

![image](https://github.com/user-attachments/assets/1904cfe6-9d2c-4e96-b96c-b76461c37b67)


Step 8: Configure Help Topics

- Ensure you're under Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel') -> Manage -> Help Topics
- Click 'Add New Help Topic'
- The following topics:
    - Business Critical Outage
    - Personal Computer Issues
    - Password Reset
 
  ![image](https://github.com/user-attachments/assets/b15ebee6-64b0-4205-8c52-d0d9c75db27d)

  ![image](https://github.com/user-attachments/assets/48cdd96f-9281-498b136-7d7bb8eeb3e8)

  ![image](https://github.com/user-attachments/assets/94b0d379-85de-4c5e-bd0b-d9dff717a634)

  ![image](https://github.com/user-attachments/assets/f08d86d4-7cf3-4e8d-a46e-f37de5250803)




