<h1>Microsoft Defender XDR & Vulnerability Management Lab</h1>

<h2>Description</h2>
This lab demonstrates enterprise security monitoring and security posture analysis using Microsoft Defender XDR and Microsoft Defender Vulnerability Management. The lab focuses on security recommendations, Secure Score analysis, email protection policies, identity security posture, incident investigation, and vulnerability management within a Microsoft 365 environment.
<br />

<h2>Utilities Used</h2>

- <b>Microsoft Defender XDR</b>  
- <b>Microsoft Defender Vulnerability Management</b>  
- <b>Microsoft Entra ID</b>  
- <b>Microsoft Defender for Office 365</b>  

<h2>Environments Used</h2>

- <b>Windows 11</b>  
- <b>Microsoft 365 E5 Tenant</b>  

<h2>Lab Walk-through:</h2>

<h3>Step 1: Access Microsoft Defender Portal</h3>
<p align="center">
Navigate to Microsoft Defender Portal: <br/>

https://security.microsoft.com <br/><br/>

Review:
- Security dashboard  
- Exposure management  
- Recommendations  
- Incident monitoring interface  

<br/>

<img src="https://github.com/YOUR-REPO/Lab-6/blob/main/defender-dashboard.png" height="80%" width="80%" alt="Microsoft Defender Dashboard"/>
<br />
</p>

---

<h3>Step 2: Review Microsoft Secure Score</h3>
<p align="center">
Navigate to: Secure Score <br/><br/>

The Microsoft Secure Score dashboard was reviewed to analyze organizational security posture, recommended actions, and identity protection improvements. <br/><br/>

<img src="https://github.com/YOUR-REPO/Lab-6/blob/main/secure-score.png" height="80%" width="80%" alt="Secure Score"/>
<br />
</p>

---

<h3>Step 3: Review Exposure Management Recommendations</h3>
<p align="center">
Navigate to: Exposure Management → Recommendations <br/><br/>

Security recommendations and exposure insights were reviewed to identify potential security risks and hardening opportunities within the Microsoft 365 environment. <br/><br/>

<img src="https://github.com/YOUR-REPO/Lab-6/blob/main/exposure-management.png" height="80%" width="80%" alt="Exposure Management"/>
<br />
</p>

---

<h3>Step 4: Review Vulnerability Management Dashboard</h3>
<p align="center">
Navigate to: Exposure Management → Overview → Vulnerability Management <br/><br/>

Microsoft Defender Vulnerability Management was reviewed to analyze exposure monitoring, vulnerability assessment capabilities, and remediation workflows available within Microsoft Defender XDR.  

The tenant environment did not yet contain onboarded devices required for active vulnerability telemetry collection; however, the platform configuration interface, onboarding workflow, and vulnerability management features were successfully reviewed. <br/><br/>

<img src="https://github.com/YOUR-REPO/Lab-6/blob/main/vulnerability-management.png" height="80%" width="80%" alt="Vulnerability Management"/>
<br />
</p>

---

<h3>Step 5: Review Incidents & Alerts</h3>
<p align="center">
Navigate to: Incidents & Alerts → Incidents <br/><br/>

The incidents dashboard was reviewed to analyze alert severity levels, investigation workflows, and incident monitoring capabilities available within Microsoft Defender XDR. <br/><br/>

<img src="https://github.com/YOUR-REPO/Lab-6/blob/main/incidents-dashboard.png" height="80%" width="80%" alt="Incidents Dashboard"/>
<br />
</p>

---

<h3>Step 6: Review Identity Security Recommendations</h3>
<p align="center">
Navigate to: Recommendations → Identities <br/><br/>

Identity security recommendations were reviewed to analyze authentication security posture improvements, multifactor authentication recommendations, and identity protection guidance. <br/><br/>

<img src="https://github.com/YOUR-REPO/Lab-6/blob/main/identity-recommendations.png" height="80%" width="80%" alt="Identity Recommendations"/>
<br />
</p>

---

<h3>Step 7: Review Email & Collaboration Protection</h3>
<p align="center">
Navigate to: Email & Collaboration → Policies & Rules <br/><br/>

Email security protection settings were reviewed, including anti-phishing protections, anti-spam policies, Safe Links, and Safe Attachments configuration options available within Microsoft Defender for Office 365. <br/><br/>

<img src="https://github.com/YOUR-REPO/Lab-6/blob/main/email-security.png" height="80%" width="80%" alt="Email Security Policies"/>
<br />
</p>

---

<h3>Step 8: Review Attack Simulation Training (Optional)</h3>
<p align="center">
Navigate to: Email & Collaboration → Attack Simulation Training <br/><br/>

Attack simulation and phishing awareness training capabilities were reviewed to analyze organizational user awareness and phishing simulation functionality. <br/><br/>

<img src="https://github.com/YOUR-REPO/Lab-6/blob/main/attack-simulation.png" height="80%" width="80%" alt="Attack Simulation Training"/>
<br />
</p>

---

<h3>Step 9: Security Recommendations & Remediation Review</h3>
<p align="center">

<h4>Enabled MFA for All Users</h4>

<b>Recommendation:</b> Enable multifactor authentication (MFA) for all organizational users. <br/><br/>

<b>Risk:</b> Accounts protected only by passwords are vulnerable to credential theft, password spraying, phishing attacks, and unauthorized access attempts. <br/><br/>

<b>Suggested Action:</b> Configure Conditional Access policies within Microsoft Entra ID to require MFA for all users, especially privileged administrative accounts and cloud application access. <br/><br/>

<img src="https://github.com/YOUR-REPO/Lab-6/blob/main/mfa-recommendation.png" height="80%" width="80%" alt="MFA Recommendation"/>
<br /><br />

<h4>Ensure User Consent for Apps Access on Company Data is Blocked</h4>

<b>Recommendation:</b> Restrict user consent permissions for third-party applications requesting access to organizational data. <br/><br/>

<b>Risk:</b> Unauthorized or malicious applications may gain access to sensitive company information through excessive delegated permissions granted by users. <br/><br/>

<b>Suggested Action:</b> Configure Microsoft Entra ID user consent settings to block unauthorized application consent requests and require administrator approval for application access permissions. <br/><br/>

<img src="https://github.com/YOUR-REPO/Lab-6/blob/main/app-consent-policy.png" height="80%" width="80%" alt="App Consent Restriction"/>
<br /><br />

<h4>Enable Microsoft Entra ID Identity Protection Sign-In Risk Policies</h4>

<b>Recommendation:</b> Enable Identity Protection sign-in risk policies to monitor and respond to risky authentication attempts. <br/><br/>

<b>Risk:</b> Suspicious sign-in activity, impossible travel events, unfamiliar login properties, and risky authentication attempts may go undetected without automated identity protection monitoring. <br/><br/>

<b>Suggested Action:</b> Configure Microsoft Entra ID Identity Protection policies to automatically require MFA, block risky sign-ins, and monitor suspicious authentication behavior across organizational accounts. <br/><br/>

<img src="https://github.com/YOUR-REPO/Lab-6/blob/main/signin-risk-policy.png" height="80%" width="80%" alt="Sign-In Risk Policy"/>
<br />
</p>

---

<h2>Results / Outcome</h2>

- Successfully reviewed Microsoft Defender XDR security posture dashboards  
- Analyzed Secure Score recommendations and exposure management insights  
- Reviewed vulnerability management functionality and remediation guidance  
- Investigated incident monitoring and alert management workflows  
- Reviewed email and identity protection recommendations  
- Documented security remediation recommendations aligned with enterprise security best practices  

---

<h2>Key Learnings</h2>

- Microsoft Secure Score assists with organizational security posture improvement  
- Exposure Management provides actionable remediation recommendations  
- Identity protection policies improve authentication security monitoring  
- Restricting application consent reduces organizational data exposure risks  
- Microsoft Defender XDR centralizes security monitoring and incident investigation workflows  

---

<h2>Conclusion</h2>

This lab successfully demonstrated enterprise security operations concepts using Microsoft Defender XDR and Microsoft Defender Vulnerability Management. Security posture analysis, remediation planning, identity protection recommendations, vulnerability monitoring, and email security governance were reviewed to simulate real-world enterprise security administration and monitoring workflows.
