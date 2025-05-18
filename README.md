<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system, osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- What is osTicket
- How to install osTicket requirements
- Web server configurations for osTicket
- How to install osTicket

<h2>What is osTicket</h2>

<p>
<img src="https://github.com/user-attachments/assets/ce64d354-d74d-4a52-8af8-51b8cdb9344e" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<a href="https://osticket.com/">osTicket</a> is a free tool that makes it easier for businesses to handle their customer service requests. It allows users to submit support tickets via email, web forms, or phone, and consolidates them into a centralized system for efficient management.  Agents can effectively manage support requests by tracking, responding to, and resolving issues with ease. Its intuitive design and customizable features make it well-suited for small teams and users new to support platforms.

<h2>How to install osTicket requirements</h2>

</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/0cde3aae-7d4b-4fb1-9eb5-a9c84481b1d0" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To start <a href="https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD">download the osTicket-Installation-Files.zip</a> and unzip it onto your desktop. 
</p>Name the folder 'osTicket-Installation-Files.' We’ll use the files inside this folder to install osTicket and its necessary dependencies.
<br />

<p>
<img src="https://github.com/user-attachments/assets/c0b45d48-013b-432e-983c-3f8498a98a60" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, you'll install PHP Manager for IIS. In the 'osTicket-installation-files' folder, locate PHPManagerForIIS_V1.5.0.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/d65f90dd-13d8-440e-b59f-2fe6747805b2" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, install the Rewrite Module named rewrite_amd64_en-US.msi from the 'osTicket-Installation-Files' folder.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/b2506de4-625c-4fb4-9cfc-af718a480e36" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Before proceeding with the installation of the required programs, we need to create a folder named 'PHP' on our C drive.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/7d432ddd-020c-4a2b-ba1a-aaaa115501f7" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now that we have the PHP folder on our C drive, we can extract the files from 'php-7.3.8-nts-Win32-VC15-x86.zip' into it. This file is located in the 'osTicket-Installation-Files' folder we’ve been working with.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/d4a401ed-3efc-4c6d-b75f-2a71aa17b5e5" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, install VC_redist.x86.exe from the 'osTicket-Installation-Files' folder.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/a4488044-4381-4339-aef9-788d134b1358" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
You’ll also need to install MySQL 5.5.62 (mysql-5.5.62-win32.msi) from the 'osTicket-Installation-Files' folder. Please follow these steps.
  
- Typical Setup
- Launch Configuration Wizard (after install)
- Standard Configuration
- Password: root

Note*Using 'root' as your password is highly insecure and should only be done in virtual machines for educational or training purposes.
</p>
<br />

<h2>Web server configurations for osTicket</h2>
  
<p>
<img src="https://github.com/user-attachments/assets/c21ccb3b-fb70-44b9-9414-303f8e9361e3" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To begin configuring your web server, you will need to run Internet Information Services (IIS) Manager as an admin.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/cb7bff16-cb5d-433d-804f-e8e1d0914416" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From the IIS admin, you will need to register PHP from within IIS (PHP Manager -> C:\PHP\php-cgi.exe). Make sure you stop and restart IIS after you register your PHP to the C drive. 
</p>
<br />

<h2>How to install osTicket</h2>

<p>
<img src="https://github.com/user-attachments/assets/01906213-972c-4e5f-bc50-fa4d4fc920cf" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From the “osTicket-Installation-Files” folder, unzip “osTicket-v1.15.8.zip”
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/e55b7b8e-9f84-42ca-b553-6588e9ea0e28" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Copy the “upload” folder into “c:\inetpub\wwwroot”
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/ba22e9e1-09b1-4639-949d-a7a03c6ebc3d" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Within “c:\inetpub\wwwroot”, rename “upload” to “osTicket”. This must be done exactly as shown; any deviation from the spelling of osTicket will result in the program not functioning. 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/d2314d34-49fe-4bf7-8a6c-9ce2d49f1322" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Finally, stop and restart IIS again. 
</p>
<br />
