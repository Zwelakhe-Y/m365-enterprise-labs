<h1>Microsoft Entra ID Security & Conditional Access Lab</h1>

<h2>Description</h2>
This lab demonstrates identity protection and access control using Microsoft Entra ID and Conditional Access policies. The lab focuses on enforcing Multi-Factor Authentication (MFA), restricting access to non-compliant devices, monitoring authentication activity, and simulating real-world enterprise security configurations.
<br />

<h2>Utilities Used</h2>

- <b>Microsoft Entra ID</b>  
- <b>Microsoft Intune</b>  
- <b>Microsoft 365 E5</b>  

<h2>Environments Used</h2>

- <b>Windows 11</b>  
- <b>Microsoft 365 E5 Tenant</b>  

<h2>Lab Walkthrough:</h2>

<h3>Step 1: Access Microsoft Entra Admin Center</h3>
<p align="center">
Navigate to Microsoft Entra Admin Center: <br/>

https://entra.microsoft.com <br/><br/>

<img src="https://github.com/Zwelakhe-Y/m365-enterprise-labs/blob/main/Identity%20Security%20%2B%20Conditional%20Access/Screenshots/1.%20MFA%20Enabled.png" height="80%" width="80%" alt="Entra Dashboard"/>
<br />
</p>

---

<h3>Step 2: Enable Multi-Factor Authentication (MFA)</h3>
<p align="center">
Navigate to: Users → All Users → Choose any Test user → Authentication Methods <br/><br/>

Enable Multi-Factor Authentication (MFA) for the test user account. <br/><br/>

<img src="" height="80%" width="80%" alt="Enable"/>

<br />

</p>

---

<h3>Step 3: Create Conditional Access Policy</h3>
<p align="center">
Navigate to: ID Protection → Dashboard → Conditional Access → New Policy <br/><br/>

Create a policy requiring MFA for all users accessing cloud applications. <br/><br/>

Policy Settings:
- Users: All Users  
- Resources <b> ( Previously Cloud Apps ) </b>: All resources <b>( Previously All Cloud Apps )</b>  
- Grant Access: Require MFA  

<br/>

<img src="https://github.com/Zwelakhe-Y/m365-enterprise-labs/blob/main/Identity%20Security%20%2B%20Conditional%20Access/Screenshots/2.%20Require%20MFA%20for%20all%20users.png" height="80%" width="80%" alt="MFA Policy Settings"/>
<br />

<img src="https://github.com/Zwelakhe-Y/m365-enterprise-labs/blob/main/Identity%20Security%20%2B%20Conditional%20Access/Screenshots/2.1%20Require%20MFA%20for%20all%20users.png" height="80%" width="80%" alt="Require MFA Settings"/>
<br />
</p>

---

<h3>Step 4: Create Device Compliance Access Policy</h3>
<p align="center">
Create an additional Conditional Access policy requiring compliant devices for access. <br/><br/>

Policy Settings:
- Users: All Users  
- Resources <b> ( Previously Cloud Apps ) </b>: All resources <b>( Previously All Cloud Apps )</b>  
- Grant Access: Require Device to be Marked as Compliant  

<br/>

<img src="https://github.com/Zwelakhe-Y/m365-enterprise-labs/blob/main/Identity%20Security%20%2B%20Conditional%20Access/Screenshots/3.%20Require%20Device%20to%20be%20compliant.png" height="80%" width="80%" alt="Device Compliance Policy"/>
<br />
</p>

---

<h3>Step 5: Review Sign-In Logs</h3>
<p align="center">
Navigate to: Monitoring → Sign-in Logs <br/><br/>

Review authentication activity, including:
- Successful sign-ins  
- Failed authentication attempts  
- MFA requirements  
- Device and browser information  

<br/>

<img src="https://github.com/Zwelakhe-Y/m365-enterprise-labs/blob/main/Identity%20Security%20%2B%20Conditional%20Access/Screenshots/4.%20Review%20sign%20in%20Logs.png" height="80%" width="80%" alt="Sign In Logs"/>
<br />
</p>

---

<h3>Step 6: Test MFA & Conditional Access Enforcement</h3>
<p align="center">
Authentication policies were tested using a private browser session. During sign-in, Microsoft Entra ID enforced additional authentication requirements and blocked access from non-compliant devices according to organizational security policies. <br/><br/>

Security behaviors tested:
- MFA enforcement  
- Device compliance enforcement  
- Access restriction policies  

<br/>

<img src="https://github.com/Zwelakhe-Y/m365-enterprise-labs/blob/main/Identity%20Security%20%2B%20Conditional%20Access/Screenshots/5.%20MFA%20Challenge%20screen.png" height="80%" width="80%" alt="MFA Challenge"/>
<br /><br/>

<img src="https://github.com/Zwelakhe-Y/m365-enterprise-labs/blob/main/Identity%20Security%20%2B%20Conditional%20Access/Screenshots/5.1%20MFA%20Challenge%20screen.png" height="80%" width="80%" alt="Compliance Restriction"/>
<br />
</p>

---

<h2>Results / Outcome</h2>

- Successfully configured Multi-Factor Authentication (MFA)  
- Implemented Conditional Access security policies  
- Enforced device compliance restrictions  
- Monitored authentication activity using sign-in logs  
- Simulated enterprise identity protection scenarios  

---

<h2>Key Learnings</h2>

- Conditional Access strengthens organizational security posture  
- MFA reduces the risk of account compromise  
- Device compliance policies restrict unauthorized device access  
- Sign-in monitoring assists with security auditing and investigation  

---

<h2>Conclusion</h2>

This lab successfully demonstrated enterprise-level identity security using Microsoft Entra ID and Conditional Access policies. MFA enforcement, compliance-based restrictions, and authentication monitoring were implemented to simulate real-world Zero Trust security practices used in modern organizations.
