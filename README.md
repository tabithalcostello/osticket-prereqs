
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Microsoft Remote Desktop
- Internet Information Services (IIS)

<h2>Operating System Used </h2>

- Windows 10</b>

<h2>Synopsis</h2>

- Create a Virtual Machine 
- Install & Enable Internet Information Services (IIS)
- Download Installation Files
- Configure IIS
- Configure the osTicket Installer

<h2>Installation Steps</h2>

<p align="center">
<img src="https://i.imgur.com/HcOnrqb.png" height="50%" width="50%" alt="VM"/>
</p>
<p> Create Virtual Machine (VM) in Microsoft Azure with 2-4 virtual computer processing units (CPU). Then, connect to the VM with Microsoft Remote Desktop. 
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/dznSw6k.png" height="50%" width="50%" alt="Install IIS"/>
</p>
<p> In the VM's control panel, access Programs: Turn Windows Features On or Off. In the IIS's subfolder of World Wide Web Services' (WWS) subfolder of Application Development, check CGI. In the WWWS' subfolder of Common HTTP Features, make sure all the boxes have been checked (or X). 
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/IWxHXqU.png" height="50%" width="50%" alt="Installation Files"/>
</p>
<p> Download PHP Manager for IIS, IIS URL Rewrite Module, and PHP zip File. Create a directory C:\PHP. Extract PHP zip file, and insert in C:\PHP. Download Microsoft C++ 2015-2022 Redistributable and MySQL Server 5.5. 
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/utnjqwE.png" height="50%" width="50%" alt="MySQL"/>
</p>
<p> When installing MySQL Server, select Typical Setup and launch the Configuration Wizard. Select Standard Configuration and add your root password. 
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/JzPYRlt.png" height="50%" width="50%" alt="IIS"/>
</p>
<p> Open IIS and run as administrator. Register PHP with the php_cgi that was extracted earlier into the C:\PHP. Restart IIS. 
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/tVOW7mn.png" height="50%" width="50%" alt="osTicket"/>
</p>
<p> Download osTicket, Extract the "upload" folder and drop it into C:\inetpub\wwwroot. Rename the "upload" folder to "osTicket." Reload IIS, and Restart server (or Stop then Start server). 
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/KCm4IbZ.png" height="50%" width="50%" alt="Reboot IIS"/>
</p>
<p align="center"> In IIS Connections, go to osTicket, then click on Browse *:80 (http). 
</p>
<br />


<p align="center">
<img src="https://i.imgur.com/REogFsQ.png" height="50%" width="50%" alt="Initial osTicket Screen"/>
</p>
<p align="center"> If installed correctly, the osTicket Installer appears on a web page. 
</p>
<br />


<p align="center">
<img src="https://i.imgur.com/FhGQ4D4.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p> In IIS, access the PHP Manager. Enable the following extensions: php_imap.dll, php_intl.dll, and php_opcache.dll. Restart IIS. Refresh the webpage. Notice the changes in the features. 
</p>
<br />


<p align="center">
<img src="https://i.imgur.com/bkrPDPy.png" height="50%" width="50%" alt="Rename"/>
</p>
<p> Access the osTicket folder's subfolder: Include. Select "ost-sampleconfig.php" and rename it "ost-config.php." 
<br />

<p align="center">
<img src="https://i.imgur.com/BGW2YUH.png" height="50%" width="50%" alt="Permissions"/>
</p>
<p> In ost-config.php's Properties' Security section, Disable Inheritance, and add new permissions for the principal "Everyone" and select all the basic permissions. 
</p>
<br />

<p align="center">
<img src="" height="50%" width="50%" alt=""/>
</p>
<p> Return to the osTicket Installer in the web browser. Add Name, Default E-mail, 

</p>
<br />

<p align="center">
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
Description
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
Description
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
Description
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
Description
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
Description
</p>
<br />
