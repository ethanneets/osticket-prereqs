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

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Server Requirements: Web Server, PHP Version, PHP Extentions
- File Permissions
- Mail Server: MAP/POP3/SMTP access
- Software Dependecies: A working web browser (for access)
- Download and Upload osTicket Files

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/WGqo7yw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
First off, to install IIS In windows you want to go into "programs and features". Scroll down to "Internet Information Services" and proceed to check the following: Web management tools, World Wide Web Services, Application Devolopment Features, Common HTTP Features,Health and Diagnostic, Performance Features, Security, and finally CGI these are all the prerequisites to installing the web server
</p>
<br />

<p>
<img src="https://i.imgur.com/iStkS1O.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next you are gonna install PHP manager and Rewrite Modlue both are requirments for OsTicket to run. Now you are gonna create the directory by making a new file in the C drive and naming it PHP. Then you are gonna unzip PHP manager folder into the new PHP folder and it will grant you all neccesary files. Then Install vc redistx86 and mySQL and in mySQL go ahead and launch the configuration Wizard in mySQL and proceed to create a password. Next you are gonna open IIS as a admin and register PHP by opening PHP Manager then you gonna want to reload the web server and now we are finally gonna install OsTicket.
</p>
<br />

<p>
<img src="https://i.imgur.com/6Se4Sle.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From the OsTicket installation folder you are gonna unzip the file and then copy the upload folder into the inetpub root folder. Then rename the folder to "OsTicket". Now you are gonna restart the server again, now in IIS go to sites and load the OsTicket site and it should pop up on your web browser. Notice how some of the extentions are not enabled so we are gonna have to go ahead and enable them by going back into PHP Manager and enable the ones needed to proceed. Hit refresh until all are enabled and now we need to rename a file in the OsTicket folder called "C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php" and change it to "To: C:\inetpub\wwwroot\osTicket\include\ost-config.php" in the same file you want to assign permissions so first you need to disable inhertitance and now youre gonna add new permissions to your liking. Now you can continute the setup by following the site, and proceed to install HeidiSQL and make a connection to your database within the application and once that is done you can finally press install!

</p>
<br />
