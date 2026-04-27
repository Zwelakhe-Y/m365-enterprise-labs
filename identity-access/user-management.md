<h1>Microsoft 365 Identity & Access Management Lab</h1>

<h2>Description</h2>
This lab demonstrates how to configure and manage identity and access controls within a Microsoft 365 E5 environment. It covers user creation, group management, role-based access control (RBAC), Multi-Factor Authentication (MFA), Conditional Access policies, and basic automation using PowerShell. The goal is to simulate a real-world enterprise onboarding and security implementation scenario.
<br />


<h2>Utilities Used</h2>

- <b>Microsoft 365 E5</b>  
- <b>Microsoft Entra ID (Azure AD)</b>  
- <b>PowerShell (Microsoft Graph)</b>  


<h2>Environments Used </h2>

- <b>Windows 11</b>  
- <b>Microsoft 365 Admin Center</b>  


<h2>Labs walk-through:</h2>

<h3>Microsoft 365 Admin Center Access:</h3>
<p align="center">
To begin, log in to the Microsoft 365 Admin Center using your E5 account: <br/>
<img src="YOUR_SCREENSHOT_LINK_HERE" height="80%" width="80%" alt="Admin Dashboard"/>
<br />
<br />
This dashboard is where all users, roles, and services are managed. <br/>
</p>


<h3>User Creation:</h3>
<p align="center">
Navigate to <b>Users → Active Users</b> and click <b>Add a user</b>: <br/>
<img src="YOUR_SCREENSHOT_LINK_HERE" height="80%" width="80%" alt="Create User"/>
<br />
<br />
Fill in user details such as name and username (e.g., hr@yourdomain.onmicrosoft.com): <br/>
<img src="YOUR_SCREENSHOT_LINK_HERE" height="80%" width="80%" alt="User Details"/>
<br />
<br />
After creating users, confirm they appear in the Active Users list: <br/>
<img src="YOUR_SCREENSHOT_LINK_HERE" height="80%" width="80%" alt="Users List"/>
<br />
<br />
</p>


<h3>Group Creation and Management:</h3>
<p align="center">
Navigate to <b>Teams & Groups → Active Teams & Groups</b> and create new Security Groups: <br/>
<img src="YOUR_SCREENSHOT_LINK_HERE" height="80%" width="80%" alt="Create Groups"/>
<br />
<br />
Assign users to their respective groups (HR, IT, Finance): <br/>
<img src="YOUR_SCREENSHOT_LINK_HERE" height="80%" width="80%" alt="Group Members"/>
<br />
<br />
</p>


<h3>Role-Based Access Control (RBAC):</h3>
<p align="center">
Navigate to <b>Roles → Admin Roles</b> and assign administrative roles: <br/>
<img src="YOUR_SCREENSHOT_LINK_HERE" height="80%" width="80%" alt="Assign Roles"/>
<br />
<br />
Assign Global Administrator role to IT user for demonstration purposes: <br/>
<img src="YOUR_SCREENSHOT_LINK_HERE" height="80%" width="80%" alt="Admin Role Assigned"/>
<br />
<br />
</p>


<h3>Multi-Factor Authentication (MFA):</h3>
<p align="center">
Navigate to user settings and enable Multi-Factor Authentication: <br/>
<img src="YOUR_SCREENSHOT_LINK_HERE" height="80%" width="80%" alt="Enable MFA"/>
<br />
<br />
Confirm MFA status is enabled for users: <br/>
<img src="YOUR_SCREENSHOT_LINK_HERE" height="80%" width="80%" alt="MFA Enabled"/>
<br />
<br />
</p>


<h3>Conditional Access Policy Configuration:</h3>
<p align="center">
Go to Microsoft Entra ID portal and navigate to <b>Protection → Conditional Access</b>: <br/>
<img src="YOUR_SCREENSHOT_LINK_HERE" height="80%" width="80%" alt="Conditional Access"/>
<br />
<br />
Create a policy to block access outside South Africa: <br/>
<img src="YOUR_SCREENSHOT_LINK_HERE" height="80%" width="80%" alt="Create Policy"/>
<br />
<br />
Enable and review the policy settings: <br/>
<img src="YOUR_SCREENSHOT_LINK_HERE" height="80%" width="80%" alt="Policy Enabled"/>
<br />
<br />
</p>


<h3>Self-Service Password Reset (SSPR):</h3>
<p align="center">
Navigate to Password Reset settings in Entra ID and enable for all users: <br/>
<img src="YOUR_SCREENSHOT_LINK_HERE" height="80%" width="80%" alt="SSPR Settings"/>
<br />
<br />
</p>


<h3>PowerShell Automation (User Creation):</h3>
<p align="center">
Open PowerShell and connect to Microsoft Graph: <br/>
<img src="YOUR_SCREENSHOT_LINK_HERE" height="80%" width="80%" alt="PowerShell Connect"/>
<br />
<br />
Run the following script to automate user creation: <br/>
</p>

<pre>
<code>
Connect-MgGraph -Scopes "User.ReadWrite.All"

New-MgUser -DisplayName "John Doe" `
  -UserPrincipalName "john@yourtenant.onmicrosoft.com" `
  -MailNickname "john" `
  -AccountEnabled $true `
  -PasswordProfile @{
    Password = "TempPassword123!"
    ForceChangePasswordNextSignIn = $true
  }
</code>
</pre>

<p align="center">
Verify that the user was successfully created in the Admin Center: <br/>
<img src="YOUR_SCREENSHOT_LINK_HERE" height="80%" width="80%" alt="User Created via Script"/>
<br />
<br />
</p>


<h3>Conclusion:</h3>
<p align="center">
This lab successfully demonstrated how to implement identity and access management in a Microsoft 365 environment. By combining user management, security policies, and automation, a secure and scalable system was created that reflects real-world enterprise practices. <br/>
</p>


<!--
 ```diff
- Weak authentication increases security risks
+ MFA and Conditional Access improve security posture
! Automation reduces manual workload
# Identity is the new security perimeter
@@ Zero Trust model implemented @@
