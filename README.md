<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Enabling-and-Unlocking-Accounts-and-Resetting-Passwords</h1>
This tutorial teaches you how to handle account lockouts by configuring Group Policy to lock an account after a set number of failed login attempts. It also covers disabling and re-enabling accounts in Active Directory and observing the corresponding error messages when trying to log in. Finally, the tutorial shows how to monitor login activity by reviewing logs on both the Domain Controller and the Client Machine.<br />


<h2>Video Demonstration</h2>

- ### [Enabling-and-Unlocking-Accounts-and-Resetting-Passwords](https://youtu.be/mQrzdTbR4ow?si=wkTwGXYv1dokEdKX)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- Group Policy


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


![Part4Part1](https://github.com/user-attachments/assets/7766f28b-4dce-4fcc-b974-5abc081dc6b1)



</p>
<p>
Log into DC-1 and select a random user account.

Configure Group Policy to lock the account after 5 failed login attempts.

You can wait for the Group Policy to propagate automatically, or you can force an update immediately.
On a client machine or server, open Command Prompt and type gpupdate /force, then press Enter.

Try logging in with the wrong password 6 times to trigger the account lockout.

Observe that the account is locked in Active Directory.

Unlock the account, reset the password, and attempt to log in again.
</p>
<br />

<p>


![Part4Part2](https://github.com/user-attachments/assets/62d6d874-9610-41c5-bb3c-24c3156c2343)



</p>
<p>
Disable the same user account in Active Directory.
  
Attempt to log in and observe the error message indicating the account is disabled.

Re-enable the account and attempt to log in again.

</p>
<br />


![Part4Part3](https://github.com/user-attachments/assets/5028d2d2-cdfd-4f2a-bca6-54a469e015bb)



</p>
<p>
Check the logs on the Domain Controller for account lockout events.
  
Review logs on the client machine to observe login-related events.
</p>
<br />
