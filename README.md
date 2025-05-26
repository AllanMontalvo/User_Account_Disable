# User_Account_Disable
Procedure on how to disable account and reset account password in Active Directory on Azure.


<h2>Environments and Technologies Used</h2>

**Technologies and Servies**
- Microsoft Azure
- Active Directory Domain Services

**Environment/Operating System**
- Windows Server 2022
- Windows 10

<h2>High-Level Deployment and Configuration Steps</h2>

**Step 1: Disable Account**
- Login to DC-1 as admin (jane.doe).
- Go to "Active Directory Users and Computers"
- Select a user and go to "Account" tab.
- In "Account Options", check "Account is disable" box and click apply.  

![Account Disable](https://github.com/user-attachments/assets/4c0de5cc-2fff-4f53-949d-fd507b77d18f)

**Step 2: Login to Account**
- Attempt to login to Client-1 of the select user.
- Will receive a prompt indicated that account is disable.

![Disable message](https://github.com/user-attachments/assets/35f69741-66f6-48ac-beb4-92cc67b05346)

**Step 3: Enable Account**
- Go back to DC-1.
- Go to Active Directory Users and Computer".
- Right-click your domain name (mydomain.net) and select "Find".
- Type user's name.
- Select a user and go to "Account" tab.
- In "Account Options", uncheck "Account is disable" box and click apply.

![Enable Account](https://github.com/user-attachments/assets/1d7d3ee3-d7e9-4e48-9843-1c8e67bd4c20)

- Login to Client-1 as user.

