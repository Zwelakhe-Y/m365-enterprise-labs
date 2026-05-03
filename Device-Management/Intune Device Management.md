<h1>Microsoft Intune Device Enrollment & Management Lab</h1>

<h2>Description</h2>
This lab demonstrates how to enroll a Windows device into Microsoft Intune, configure automatic enrollment via Microsoft Entra ID, and apply compliance, configuration, and application deployment policies. It simulates real-world enterprise endpoint management used by IT administrators to secure and manage corporate devices.
<br />

<h2>Utilities Used</h2>

- <b>Microsoft Intune</b>  
- <b>Microsoft Entra ID</b>  
- <b>Windows 10/11</b>  

<h2>Environments Used</h2>

- <b>Windows 11 (Local Machine or VM)</b>  

<h2>Lab Walkthrough:</h2>

<h3>Step 1: Access Intune Admin Center</h3>
<p align="center">
Navigate to Microsoft Intune Admin Center: <br/>

https://endpoint.microsoft.com <br/><br/>

<img src="https://github.com/YOUR-REPO/Intune-Lab/blob/main/intune-dashboard.png" height="80%" width="80%" alt="Intune Dashboard"/>
<br />
</p>

---

<h3>Step 2: Enable Automatic Enrollment</h3>
<p align="center">
Go to: Devices → Enroll devices → Automatic Enrollment <br/><br/>

Set: <b>MDM user scope = All</b> <br/><br/>

<img src="https://github.com/YOUR-REPO/Intune-Lab/blob/main/mdm-scope-all.png" height="80%" width="80%" alt="MDM Scope All"/>
<br />
</p>

---

<h3>Step 3: Add Work Account to Device</h3>
<p align="center">
On Windows device: <br/>

Settings → Accounts → Access work or school → Connect <br/>
Sign in with test user account <br/><br/>

<img src="https://github.com/YOUR-REPO/Intune-Lab/blob/main/device-connected.png" height="80%" width="80%" alt="Device Connected"/>
<br />
</p>

---

<h3>Step 4: Confirm Device in Intune</h3>
<p align="center">
Go to: Devices → All Devices <br/><br/>

Verify that the enrolled device appears in the Devices list in intune <br/><br/>
<br />
</p>

---

<h3>Step 5: Create Compliance Policy</h3>
<p align="center">
Go to: Devices → Compliance Policies → Create Policy <br/><br/>

Configure:
- Require password  
- Minimum password length  
- Require BitLocker encryption <br/><br/>

<b>Note:</b>
You will need either the P1+P2 Intune products or the Intune Suite in your account to be able to create a policy

<img src="https://github.com/YOUR-REPO/Intune-Lab/blob/main/compliance-policy.png" height="80%" width="80%" alt="Compliance Policy"/>
<br /><br/>

Policy assigned to user/device to enforce security standards.
</p>

---

<h3>Step 6: Create Configuration Profile</h3>
<p align="center">
Go to: Devices → Configuration → Policy → Create <br/><br/>

Configure:
- Password complexity rules  ( Under Device Lock )
- Device restrictions  

<br/>

<img src="https://github.com/YOUR-REPO/Intune-Lab/blob/main/config-profile.png" height="80%" width="80%" alt="Configuration Profile"/>
<br />
</p>

---

<h3>Step 7: Deploy an Application</h3>
<p align="center">
Go to: Apps → Windows → Create <br/><br/>

Select application (e.g., Microsoft Edge) and assign to user/device group <br/><br/>

<img src="https://github.com/YOUR-REPO/Intune-Lab/blob/main/app-deployment.png" height="80%" width="80%" alt="App Deployment"/>
<br />
</p>


---

<h2>Conclusion</h2>
This lab demonstrates successful device enrollment into Microsoft Intune, configuration of security policies, and application deployment. These skills reflect real-world enterprise endpoint administration practices used in modern IT environments.
