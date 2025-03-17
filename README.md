<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Enabling-and-Unlocking-Accounts-and-Resetting-Passwords</h1>
This tutorial teaches you how to handle account lockouts by configuring Group Policy to lock an account after a set number of failed login attempts. It also covers disabling and re-enabling accounts in Active Directory and observing the corresponding error messages when trying to log in. Finally, the tutorial shows how to monitor login activity by reviewing logs on both the Domain Controller and the Client Machine.<br />


<h2>Video Demonstration</h2>

- ### [](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services


<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Log into DC-1 and select a previously created user account. Attempt to log in 10 times with an incorrect password to trigger a lockout.
- Configure Group Policy to set the Account Lockout Threshold to 5 failed login attempts. Afterward, attempt to log in 6 times with an incorrect password and observe the account lockout in Active Directory.
- Unlock the account in Active Directory, reset the password, and attempt to log in with the new credentials.
- Disable the same account in Active Directory and try logging in to observe the error message. Re-enable the account and log in again. Finally, observe the logs on both the Domain Controller and Client Machine.

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
