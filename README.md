<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites]([https://www.youtube.com](https://www.youtube.com/watch?v=dEvGaxOgqf0))

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

Open this: <a href="https://drive.google.com/drive/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6">Installation Files


These are the installation files that will be used to install osTicket and some of the dependencies.

1. Install / Enable IIS in Windows WITH
CGI and Common HTTP Features
  - World Wide Web Services -> Application Development Features ->
  [X] CGI
  [X] Common HTTP Features
<br>
  AND IIS Management Console
  - Internet Information Services -> Web Management Tools -> IIS Management Console
  [X] IIS Management Console

2. Download/Install PHP Manager for IIS

3. Download/Install Rewrite Module

4. Create the directory C:\PHP

5. Download/Install PHP 7.3.8 and unzip contents into C:\PHP

6. Download/Install VC_redist.x86.exe

7. Download/Install MySql 5.5.62
  - Typical Setup ->
  - Launch Configuration Wizard (after install) ->
  - Standard Configuration ->
  - Take note of username: root
  - Example Password: Password1

8. Open IIS as an Admin

9. Register PHP from within IIS

10. Reload IIS (Open IIS, Stop and Start the server)
   - Download/Install osTicket
   - Extract and copy “upload” folder to c:\inetpub\wwwroot
   - Within c:\inetpub\wwwroot, Rename “upload” to “osTicket”

11. Reload IIS (Open IIS, Stop and Start the server)

12. Go to sites -> Default -> osTicket
   - Click "Browse *.80" on the right

13. Enable extensions that are off
   - Go back to IIS, sites -> Default -> osTicket
   - Double-click PHP Manager
   - Click “Enable or disable an extension”
	- Enable: php_imap.dll
	- Enable: php_intl.dll
	- Enable: php_opcache.dll
14. Refresh the osTicket site to view updates

15. Rename: ostsample-config.php to ost-config.php
   - From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php
   - To: C:\inetpub\wwwroot\osTicket\include\ost-config.php

16. Assign Permissions: ost-config.php
   - Right click ost-config.php
   - Click security -> Advanced settings
   - Disable inheritance -> Remove All
   - Click Select a principal
   - New Permissions -> Everyone -> All
   - Apply -> Ok

17. Download and install HeidiSQL
- Open Heidi SQL
- Create a new session, root/Password1
- Connect to the session
- Right click and create a database called “osTicket”

19. Continue Setting up osticket in the browser
   - MySQL Database: osTicket
   - MySQL Username: root
   - MySQL Ex. Password: Password1
   - Click “Install Now!”

19. Congratulations! osTicket should be installed without any errors.

20. Clean up
   - Delete: C:\inetpub\wwwroot\osTicket\setup
   - Set Permissions to “Read” only: C:\inetpub\wwwroot\osTicket\include\ost-config.php


<h2>Installation Steps</h2>

Below are a few visual steps to help assist with installation.


<p>
1. Open control panel, click programs then "Turn Windows features on or off" Follow directions for step one. 
Install / Enable IIS in Windows WITH
CGI and Common HTTP Features
  - World Wide Web Services -> Application Development Features ->
   	- [X] CGI
  	- [X] Common HTTP Features
</p>


  <img width="376" alt="image" src="https://github.com/nkgarrett/osticket-prereqs/assets/156832893/6eac08b3-39eb-488e-a86d-4e9f27218738">


<p>	 
  AND IIS Management Console
  - Internet Information Services -> Web Management Tools -> IIS Management Console
	- [X] IIS Management Console
</p>
<img width="376" alt="image" src="https://github.com/nkgarrett/osticket-prereqs/assets/156832893/12e8a8cc-cb9e-43b0-8156-af50bee10b8e">
<br>
<br>
<p>
4. Create the directory C:\PHP
</p>	
 	<img width="465" alt="image" src="https://github.com/nkgarrett/osticket-prereqs/assets/156832893/f21d6cf5-7e4c-414f-9cf5-565ccbf3a7ec">
<br>
<br>
<p>
5. Download/Install PHP 7.3.8 and Unzip contents into C:\PHP
</p>	
	<img width="569" alt="image" src="https://github.com/nkgarrett/osticket-prereqs/assets/156832893/7af6fae8-cb43-4d5a-82e7-dfb5179794a5">
 <br>
 <br>
<p>
8. Open IIS as an Admin. Click start menu, search IIS and right click it to "run as administrator"
</p>
	 <img width="320" alt="image" src="https://github.com/nkgarrett/osticket-prereqs/assets/156832893/fee3bb64-4a61-4466-a648-93fdc1f4da77">
  <br>
  <br>
<p>
9. Register PHP from within IIS
   - Go to PHP Manager
   - Click Register new PHP version
</p>	
   <img width="508" alt="image" src="https://github.com/nkgarrett/osticket-prereqs/assets/156832893/19e9868f-7e6c-46a5-b318-71f0d190c444">
<br>
<br>
<p>
13. Enable extensions that are off
</p>	
    <p>Before: </p>
    <img width="508" alt="image" src="https://github.com/nkgarrett/osticket-prereqs/assets/156832893/f8846350-35bf-446a-b3a1-9adb7791e2d4"> 
<br>
<br>
<p>   
14. Refresh the osTicket site to view updates
</p>
    <p>After: </p>
    <img width="508" alt="image" src="https://github.com/nkgarrett/osticket-prereqs/assets/156832893/56a6610d-cd34-4cda-a02f-491682a02b4b">
 <br>
 <br>
 <p>
 19. Congratulations! osTicket should be installed without any errors.
<br>
<br>
    <img width="577" alt="image" src="https://github.com/nkgarrett/osticket-prereqs/assets/156832893/e48f4c1d-d123-4d8f-a25b-8780333e181b">
 </p>

</p>
<br />

<p>

</p>
<p>

</p>
<br />
