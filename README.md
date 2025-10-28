

<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> 

<h2>List of Prerequisites</h2>

- Enable Internet Information Services (IIS) and CGI on Windows
- Install PHP Manager for IIS
- Install URL Rewrite Module
- Set up PHP directory
- Install Visual C++ Redistributable (VC_redist)
- Install MySQL and configure a database

<h2>Installation Steps</h2>

<p>

<img width="1389" height="782" alt="image" src="https://github.com/user-attachments/assets/c6d62378-858c-4db5-9647-636df9f22887" />
<img width="1388" height="782" alt="image" src="https://github.com/user-attachments/assets/0630607e-24fb-41c7-a91e-cb4193bfe8a9" />
</p>
<p>
Register PHP in IIS
Open PHP Manager within IIS and register the PHP executable path:

C:\PHP\php-cgi.exe

After registration, reload IIS by stopping and starting the server to apply the changes.
</p>
<br />

<p>
<img width="1389" height="781" alt="image" src="https://github.com/user-attachments/assets/494451fc-025d-4afc-aaee-297652ec6b30" />
</p>
<p>
Go to sites -> Default -> osTicket
On the right, click “Browse *:80”

Note that some extensions are not enabled
Go back to IIS, sites -> Default -> osTicket
Double-click PHP Manager
Click “Enable or disable an extension”
Enable: php_imap.dll
Enable: php_intl.dll
Enable: php_opcache.dll
Refresh the osTicket site in your browser, observe the changes

<br />

<p>
<img width="1386" height="779" alt="image" src="https://github.com/user-attachments/assets/a280cde6-d1c5-4e38-acb7-45c31835710a" />

</p>
<p>
Continue Setting up osTicket in the browser
  
*For Database settings, we need to install Heidi SQL*
</p>
<br />


<p>
<img width="1391" height="784" alt="image" src="https://github.com/user-attachments/assets/6e1695aa-732d-4d38-946c-e8821a2fb950" />
<img width="1386" height="782" alt="image" src="https://github.com/user-attachments/assets/4d91f1b8-be39-4680-8cdf-a2efa785840f" />

</p>
<p>
Install Heidi SQL
Create and connect to the new session
</p>
<br />


<p>
<img width="1389" height="778" alt="image" src="https://github.com/user-attachments/assets/8fda960a-faaf-47e2-8942-9b46a81ea70b" />
<img width="1391" height="780" alt="image" src="https://github.com/user-attachments/assets/971272bb-389b-4cc1-aa1a-a39b758aa657" />
</p>
<p>
Create a database called "osTicket"
</p>
<br />



<p>
<img width="1389" height="781" alt="image" src="https://github.com/user-attachments/assets/0683fdf2-999e-44e6-8ccc-93387aa5c913" />
</p>
<p>
Continue setting up osTicket in the browser
  
  MySQL Database: osTicket
  
  MySQL Username: root
  
  MySQL Password: root

</p>
<br />



<p>
<img width="1389" height="783" alt="image" src="https://github.com/user-attachments/assets/0505ab9f-3f47-4f7d-93fe-37c16fe77a04" />


</p>
<p>
osTicket installation completed successfully!
</p>
<br />



<p>
<img width="1388" height="780" alt="image" src="https://github.com/user-attachments/assets/3a777ee3-c07a-40aa-ba67-c5f6dcae1161" />


</p>
<p>
After completing the installation, open HeidiSQL and refresh the osTicket database.
  
You should now see all the newly created tables and data structures that support the osTicket system.
</p>
<br />




