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

- Create Roles
- Create Departments
- Create Agents
- Create SLAs
- Create Help Topics

<h2>Configuration Steps</h2>

<p>
</p>
<p>

We will be using both the Admin Panel and Agent Panel for the post-configuration set-up.
![Lab2-1](https://github.com/user-attachments/assets/67e80ce4-f05e-4219-9a56-7e600bdf41da)

![Lab2-2](https://github.com/user-attachments/assets/9d5bbb1d-3ddb-4a5b-9ee1-5b8870ba338f)

Create a new role, click Agents -> click Roles -> click Add a new Role. Set name as Administrator and give permission to everything in Tickets, Tasks, and Knowledgebase then Add Role!

![Lab2-3 1](https://github.com/user-attachments/assets/6f07438c-1fff-495d-a5b2-66a99dc69a81)

![Lab2-3 2](https://github.com/user-attachments/assets/e7dff6c1-c14e-4a03-b7cd-823ac943c6e1)

Create a new Department, click Department -> click Add a new Department. Set the name as SystemAdmins and add the new department!

![Lab2-4](https://github.com/user-attachments/assets/b84c79e2-2ed8-4284-97c7-bb2445e9ff67)

Create a new Team, click Teams -> click Add a new Team. Set the name as Online Banking and create the team!

![Lab2-5](https://github.com/user-attachments/assets/73757119-51cb-45e6-a1b4-ab3b65485542)

Now lets configure our Users Settings, click Settings -> click Users. Uncheck "Registration Required" and click save changes. This will let anyone create a ticket and that's what we want!

![Lab2-6](https://github.com/user-attachments/assets/ac3dc4b6-1948-42c8-816d-031c450227a1)

Create a new Administrator Agent, click Agents -> click Add a new Agent. The "Agents" will simulate IT help desks and resolve/elevate tickets. Jot down the username and password just in case as we will be logging on the "Agents" account to finish tickets. Continue configuring by clicking Access and give Administrator Role in the department of SystemAdmins. Finally, assign their team into Online Banking and click Create. This specific account will be used to handle any escalated tickets!

![Lab2-7 1](https://github.com/user-attachments/assets/6e43a3bd-b70b-49eb-a98f-d4c098441c5d)

![Lab2-7 2](https://github.com/user-attachments/assets/947d07c6-4f04-4c8e-b738-63a2ac35a069)

![Lab2-7 3](https://github.com/user-attachments/assets/1fd04db8-0191-4b5d-8edc-c0b64752b4cd)

Create a new Support Agent, click Agents -> click Add a new Agent. Continue configuring by clicking Access and give Support role with View Only and click Create. This account will simulate our IT Help Desk 1!

![Lab2-8 1](https://github.com/user-attachments/assets/e8183562-a99c-47e7-8911-ab8f7ddcedf4)

![Lab2-8 2](https://github.com/user-attachments/assets/d315efdc-41eb-4a37-a108-6dc21b2c4db8)

In the Agent Panel create a new User, click Users -> and click Add User. Create two different user accounts and they will act as our clients issuing tickets!
![Lab2-9](https://github.com/user-attachments/assets/9f52b43e-0011-4e4d-89f7-589e034e296f)
![Lab2-10](https://github.com/user-attachments/assets/1b6f78f9-a9fd-4ea4-8a27-e34b8d765a3f)
![Lab2-11](https://github.com/user-attachments/assets/24686c54-d40c-4cb9-9aa8-c2e76d9017e8)

Next lets add 3 SLAs (Service Level Agreement), Go back to Admin Panel -> click Manage -> click SLA -> click Add New SLA Plan. Name:Sev-A, Grace Period: 1, Schedule:24/7 and click Add Plan. Name:Sev-B, Grace Period: 4, Schedule: 24/7. Name:Sev-C, Grace Period: 8, Schedule: Monday - Friday 8am - 5pm with U.S Holidays. We will use these SLAs and assign them accordingly when determining the severity of the issue as Help Desk 1.

![Lab2-11 1](https://github.com/user-attachments/assets/1e3b006e-f254-413f-a753-6e6cec1549ec)

![Lab2-11 2](https://github.com/user-attachments/assets/03509a28-e644-427a-aaf6-806d18e239c6)

![Lab2-11 3](https://github.com/user-attachments/assets/0ed484ab-5c59-47c6-a419-e41c0c53fa46)

Finally we will create some Help Topics for our clients to select when creating a ticket. Click Help Topics -> click Add New Help Topic. 

![Lab2-12 1](https://github.com/user-attachments/assets/bdf46734-51e0-406f-961e-4d19ba3e6f9b)

![Lab2-12 2](https://github.com/user-attachments/assets/cd228a7c-8cb5-4119-bcc3-51b386816ffa)

![Lab2-12 3](https://github.com/user-attachments/assets/ec3fc65d-c8f6-491d-832e-a9be8d1c81a3)

![Lab2-12 4](https://github.com/user-attachments/assets/80d4dcc6-6755-4466-bfd4-c9f94e516375)

![Lab2-12 5](https://github.com/user-attachments/assets/d9b32244-9ad2-4e60-a0c1-5cdfec2a0529)

This will conclude the tutorial on the Post-Installation of osTicket! Now that we have the guidelines and intuition on how to navigate osTicket we wil finally get to the ticket-lifecycle from start to finish.






