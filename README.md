<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial provides the steps to complete the post-install configuration of the osTicket help desk ticketing system.<br />

<h2>Technologies and Tools Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop Protocol (RDP)
- Internet Information Services (IIS)

<h2>Operating System</h2>

- Windows 10 (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Understand the difference between the Agent Panel and Admin Panel.
- Set up Roles to define agent permissions.
- Configure Departments to organize tickets by responsibility areas.
- Create Teams to include agents from multiple departments.
- Adjust user settings to control ticket creation access.
- Add Agents (staff) and Users (customers).
- Establish Service Level Agreements (SLAs) for ticket response times.
- Define Help Topics for ticket categorization.

<h2>Configuration Steps</h2>

<h3>1.) Understand Agent Panel vs Admin Panel</h3>

- The **Agent Panel** is used by agents to manage and respond to tickets.
- The **Admin Panel** is for managing system configurations, settings, and permissions.

<h3>2.) Set Up Roles</h3>

- Navigate to **Admin Panel -> Agents -> Roles**.
- Add a new role called **Supreme Admin**.
  - Assign permissions based on the role, such as access to Tickets, Tasks, and Knowledgebase.

<p>
<img src="https://i.imgur.com/9dJCITM.png" height="80%" width="80%" alt="Configure Roles"/>
</p>

<p>
<img src="https://i.imgur.com/LH17Nqu.png" height="80%" width="80%" alt="Configure Roles"/>
</p>

<h3>3.) Configure Departments</h3>

- Navigate to **Admin Panel -> Agents -> Departments**.
- Add a new department named **SysAdmins**.
  - Use departments to control ticket visibility and assign responsibilities (e.g., Help Desk, SysAdmins, Networking).

<p>
<img src="https://i.imgur.com/WmvPMtk.png" height="80%" width="80%" alt="Configure Departments"/>
</p>

<h3>4.) Set Up Teams</h3>

- Navigate to **Admin Panel -> Agents -> Teams**.
- Create a new team called **Online Banking**.
  - Form teams by including agents from different departments.

<p>
<img src="https://i.imgur.com/4FEa6Y1.png" height="80%" width="80%" alt="Configure Teams"/>
</p>

<h3>5.) Allow Public Ticket Creation</h3>

- Navigate to **Admin Panel -> Settings -> User Settings**.
- Uncheck **Require registration and login to create tickets** to allow anyone to create tickets.
- Enable **Public - Anyone can register** to remove the requirement for users to register and log in before creating tickets.

<p>
<img src="https://i.imgur.com/zwlsNTN.png" height="80%" width="80%" alt="User Settings"/>
</p>

<h3>6.) Add Agents (Staff)</h3>

- Navigate to **Admin Panel -> Agents -> Add New**.
- Add the following agents:
  - **Jane**: Assigned to the **SysAdmins** department.
  - **John**: Assigned to the **Support** department.

<p>
<img src="https://i.imgur.com/0Yyr2vR.png" height="80%" width="80%" alt="Add Agents"/>
</p>

<p>
<img src="https://i.imgur.com/uCV94g6.png" height="80%" width="80%" alt="Add Agents"/>
</p>

<p>
<img src="https://i.imgur.com/nALrgaJ.png" height="80%" width="80%" alt="Add Agents"/>
</p>

<p>
<img src="https://i.imgur.com/yzZof2X.png" height="80%" width="80%" alt="Add Agents"/>
</p>

<h3>7.) Add Users (Customers)</h3>

- Navigate to **Agent Panel -> Users -> Add New**.
- Add the following users:
  - **Karen**
  - **Ken**

<p>
<img src="https://i.imgur.com/xrJ8gm6.png" height="80%" width="80%" alt="Add Users"/>
</p>

<h3>8.) Set Up SLA (Service Level Agreements)</h3>

- Navigate to **Admin Panel -> Manage -> SLA**.
- Add these SLAs:
  - **Sev-A**: Grace Period = 1 hour, Schedule = 24/7.
  - **Sev-B**: Grace Period = 4 hours, Schedule = 24/7.
  - **Sev-C**: Grace Period = 8 hours, Schedule = Business Hours.

<p>
<img src="https://i.imgur.com/cLC1cDs.png" height="80%" width="80%" alt="Configure SLA"/>
</p>

<p>
<img src="https://i.imgur.com/scM2F5T.png" height="80%" width="80%" alt="Configure SLA"/>
</p>

<p>
<img src="https://i.imgur.com/PGe4b44.png" height="80%" width="80%" alt="Configure SLA"/>
</p>

<h3>9.) Define Help Topics</h3>

- Navigate to **Admin Panel -> Manage -> Help Topics**.
- Add the following help topics for users to categorize their tickets:
  - **Business Critical Outage**
  - **Personal Computer Issues**
  - **Equipment Request**
  - **Password Reset**
  - **Other**

<p>
<img src="https://i.imgur.com/QkUOKCA.png" height="80%" width="80%" alt="Configure Help Topics"/>
</p>

<h2>Conclusion</h2>

By following these post-install configuration steps, you have successfully customized osTicket to meet your organization's needs. Your help desk system is now ready to efficiently manage and resolve customer issues.
