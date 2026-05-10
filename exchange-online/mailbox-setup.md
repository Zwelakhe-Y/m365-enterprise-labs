<h1>Microsoft Exchange Online Administration & RBAC Lab</h1>

<h2>Description</h2>
This lab demonstrates Microsoft Exchange Online administration within a Microsoft 365 environment. The lab focuses on mailbox administration, shared mailbox configuration, distribution group management, mail flow troubleshooting, and Role-Based Access Control (RBAC) implementation using Exchange Online administrative roles.
<br />

<h2>Utilities Used</h2>

- <b>Microsoft Exchange Online</b>  
- <b>Microsoft 365 Admin Center</b>  
- <b>Microsoft Entra ID</b>  

<h2>Environments Used</h2>

- <b>Windows 11</b>  
- <b>Microsoft 365 E5 Tenant</b>  

<h2>Lab Walkthrough:</h2>

<h3>Step 1: Access Exchange Admin Center</h3>
<p align="center">
Navigate to Microsoft Exchange Admin Center: <br/>

https://admin.exchange.microsoft.com <br/><br/>

<img src="https://github.com/Zwelakhe-Y/m365-enterprise-labs/blob/main/exchange-online/screenshots/1.%20Exchange%20Dashboard.png" height="80%" width="80%" alt="Exchange Admin Center"/>
<br />
</p>

---

<h3>Step 2: Review Existing Mailboxes</h3>
<p align="center">
Navigate to: Recipients → Mailboxes <br/><br/>

Previously created Microsoft 365 user accounts were automatically provisioned with Exchange Online mailboxes after license assignment. Mailbox availability and configuration were verified through Exchange Admin Center. <br/><br/>

<img src="https://github.com/Zwelakhe-Y/m365-enterprise-labs/blob/main/exchange-online/screenshots/2.%20Email-boxes.png" height="80%" width="80%" alt="Mailbox List"/>
<br />
</p>

---

<h3>Step 3: Create Shared Mailbox</h3>
<p align="center">
Navigate to: Recipients → Mailboxes → Add Shared Mailbox <br/><br/>

A shared mailbox was created to simulate centralized IT support communication and collaborative mailbox management. Delegation permissions were assigned to test users for mailbox access and administration. <br/><br/>

<img src="https://github.com/Zwelakhe-Y/m365-enterprise-labs/blob/main/exchange-online/screenshots/3.%20Create%20shared%20email.png" height="80%" width="80%" alt="Shared Mailbox"/>
<br />

<img src="https://github.com/Zwelakhe-Y/m365-enterprise-labs/blob/main/exchange-online/screenshots/3.1%20Add%20user%20into%20shared%20mailbox.png" height="80%" width="80%" alt="Add user to shared Mailbox"/>
<br />
</p>

---

<h3>Step 4: Configure Distribution Group</h3>
<p align="center">
Navigate to: Recipients → Groups → Distribution list <br/><br/>

A standard distribution group was created to simulate organization-wide email communication. Group membership was manually managed to demonstrate controlled access and distribution management practices. <br/><br/>

<img src="https://github.com/Zwelakhe-Y/m365-enterprise-labs/blob/main/exchange-online/screenshots/4.%20Create%20Distribution%20Group.png" height="80%" width="80%" alt="Distribution Group"/>
<br />
</p>

---

<h3>Step 5: Test Mail Flow</h3>
<p align="center">
Mail flow testing was performed using Outlook Web Access (OWA) by sending messages between organizational users, shared mailboxes, and distribution groups. <br/><br/>

Testing included:
- User-to-user email communication  
- Shared mailbox communication  

<br/>

<img src="https://github.com/Zwelakhe-Y/m365-enterprise-labs/blob/main/exchange-online/screenshots/5.%20User%20to%20User%20Mail%20Flow%20Test.png" height="80%" width="80%" alt="User to user Mail Flow Test"/>
<br />

<img src="https://github.com/Zwelakhe-Y/m365-enterprise-labs/blob/main/exchange-online/screenshots/5.0%20User%20shared%20mail%20test.png" height="80%" width="80%" alt="User to shared Mail Flow Test"/>
<br />
</p>

---

<h3>Step 6: Perform Mail Flow Troubleshooting</h3>
<p align="center">
Mail delivery and mailbox access issues were investigated using Exchange administrative troubleshooting techniques. Main issue shared email address not parcing emails to respective members Troubleshooting included:
- Verifying mailbox delegation permissions  
- Reviewing group membership  
- Confirming delivery settings  
- Validating mailbox provisioning status  

<br/>

<img src="https://github.com/Zwelakhe-Y/m365-enterprise-labs/blob/main/exchange-online/screenshots/6.%20Mail%20Trouleshooting.png" height="80%" width="80%" alt="Mail Troubleshooting"/>
<br />

<img src="https://github.com/Zwelakhe-Y/m365-enterprise-labs/blob/main/exchange-online/screenshots/6.0%20Mail%20troubleshooting.png" height="80%" width="80%" alt="Mail Troubleshooting"/>
<br />
</p>

---

<h3>Step 7: Message Trace Investigation</h3>
<p align="center">
Navigate to: Mail Flow → Message Trace <br/><br/>

Message tracing was used to analyze mail delivery activity, identify delivery failures, and review message routing behavior within Exchange Online. <br/><br/>

<img src="https://github.com/Zwelakhe-Y/m365-enterprise-labs/blob/main/exchange-online/screenshots/7.%20Message%20Trace.png" height="80%" width="80%" alt="Message Trace"/>
<br />
</p>

---

<h3>Step 8: Access Exchange RBAC Roles</h3>
<p align="center">
Navigate to: Roles <br/><br/>

Exchange Role-Based Access Control (RBAC) administration was reviewed to analyze built-in administrative roles and delegated access structures. <br/><br/>

<img src="https://github.com/Zwelakhe-Y/m365-enterprise-labs/blob/main/exchange-online/screenshots/8.%20Exchange%20RBAC%20Dashboard.png" height="80%" width="80%" alt="Exchange Roles"/>
<br />
</p>

---

<h3>Step 9: Review Built-In Administrative Role Groups</h3>
<p align="center">
Built-in Exchange administrative role groups were reviewed, including:
- Organization Management  
- Help Desk  
- Recipient Management  
- View-Only Organization Management  

<br/>

<img src="https://github.com/Zwelakhe-Y/m365-enterprise-labs/blob/main/exchange-online/screenshots/9.%20Admin%20Roles%20Group.png" height="80%" width="80%" alt="Role Groups"/>
<br />
</p>

---

<h3>Step 10: Assign Delegated Administrative Role</h3>
<p align="center">
A delegated Exchange administrative role was assigned to a support account to demonstrate least-privilege administrative access and role-based permission delegation. <br/><br/>

<img src="https://github.com/Zwelakhe-Y/m365-enterprise-labs/blob/main/exchange-online/screenshots/10.%20Assign%20help%20desk%20role.png" height="80%" width="80%" alt="Role Assignment"/>
<br />

<img src="https://github.com/Zwelakhe-Y/m365-enterprise-labs/blob/main/exchange-online/screenshots/10.1%20Help%20Desk%20role%20assigned.png" height="80%" width="80%" alt="Role Assigned"/>
<br />
</p>

---

<h3>Step 11: Verify RBAC Assignment</h3>
<p align="center">
Role assignment configuration and delegated administrative permissions were reviewed to confirm successful RBAC implementation. <br/><br/>

<img src="https://github.com/Zwelakhe-Y/m365-enterprise-labs/blob/main/exchange-online/screenshots/11.%20New%20help%20desk%20role%20user%20assigned.png" height="80%" width="80%" alt="RBAC Verification"/>
<br />
</p>

---

<h2>Results / Outcome</h2>

- Successfully administered Exchange Online mailboxes  
- Configured and managed shared mailboxes  
- Performed mail flow troubleshooting and message tracing  
- Applied Exchange RBAC administrative permissions  
- Demonstrated delegated administration and least-privilege access control  

---

<h2>Key Learnings</h2>

- Exchange Online integrates with Microsoft Entra ID identities  
- Shared mailboxes require proper delegation permissions for access  
- Distribution groups enable centralized organizational communication  
- Message Trace assists with mail flow diagnostics and troubleshooting  
- RBAC improves security through delegated administrative access control  

---

<h2>Conclusion</h2>

This lab successfully demonstrated enterprise-level Exchange Online administration and security governance practices. Mailbox management, mail flow troubleshooting, distribution group administration, and RBAC implementation were performed to simulate real-world Microsoft 365 administration scenarios commonly encountered in enterprise IT environments.
