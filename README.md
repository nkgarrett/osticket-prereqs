<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

Open this: https://drive.google.com/drive/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6
These are the installation files that will be used to install osTicket and some of the dependencies.

Install / Enable IIS in Windows WITH
CGI and Common HTTP Features
- World Wide Web Services -> Application Development Features ->
[X] CGI
[X] Common HTTP Features

AND IIS Management Console
- Internet Information Services -> Web Management Tools -> IIS Management Console
	[X] IIS Management Console

Download/Install PHP Manager for IIS

Download/Install Rewrite Module

Create the directory C:\PHP

Download/Install PHP 7.3.8 and unzip contents into C:\PHP

Download/Install VC_redist.x86.exe

Download/Install MySql 5.5.62
- Typical Setup ->
- Launch Configuration Wizard (after install) ->
- Standard Configuration ->
- Example Password: Password1

Open IIS as an Admin

Register PHP from within IIS

Reload IIS (Open IIS, Stop and Star the server)
- Download/Install osTicket
- Extract and copy “upload” folder to c:\inetpub\wwwroot
- Within c:\inetpub\wwwroot, Rename “upload” to “osTicket”

Reload IIS (Open IIS, Stop and Start the server)

Go to sites -> Default -> osTicket
- Click "Browse *.80" on the right

Enable extensions that are off
- Go back to IIS, sites -> Default -> osTicket
- Double-click PHP Manager
- Click “Enable or disable an extension”
	- Enable: php_imap.dll
	- Enable: php_intl.dll
	- Enable: php_opcache.dll
- Refresh the osTicket site to view updates

Rename: ostsample-config.php to ost-config.php
- From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php
- To: C:\inetpub\wwwroot\osTicket\include\ost-config.php

Assign Permissions: ost-config.php
- Disable inheritance -> Remove All
- New Permissions -> Everyone -> All

Download and install HeidiSQL
- Open Heidi SQL
- Create a new session, root/Password1
- Connect to the session
- Create a database called “osTicket”

Continue Setting up osticket in the browser
- MySQL Database: osTicket
- MySQL Username: root
- MySQL Ex. Password: Password1
- Click “Install Now!”

<h2>Installation Steps</h2>

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

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
