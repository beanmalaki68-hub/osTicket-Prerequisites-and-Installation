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

- Windows (Windows 11 Pro)

<h2>List of Prerequisites</h2>

- Azure Account/Subscription
- Internet Connection
- Remote Desktop installed 
- Funds or Free Subscription giving you the ability to create resources 

<h2>Installation Steps</h2>

<p>
<img width="1122" height="770" alt="Screenshot 2026-09-18 215100" src="https://github.com/user-attachments/assets/c443c48e-4821-4a20-9020-e360d68df849" />
</p>
<p>
In Microsoft Azure I first created a Windows 11 Virtual Machine to serve as the environment for my osTicket installation. I configured a the VM with 2 Virtual CPUs and named it osticket-vm. This VM will host the web server, PHP enviorment, MySQL database, and osTicket application. Also, credentials were configured during the lab but are intentionally excluded from this documentation for security reasons.
</p>
<br />

<p>
<img width="510" height="760" alt="Screenshot 2026-09-18 220115" src="https://github.com/user-attachments/assets/4a9b8c52-5440-435a-a324-778b6cbeebbe" />

</p>
<p>
I connected to the Windows virtual machine using Remote Desktop. All subsequent osTicket installation and configuration tasks were performed inside this VM.
</p>
<br />

<p>
<img width="1152" height="648" alt="OsTicket Installation Files" src="https://github.com/user-attachments/assets/cc18e892-868c-4ee2-af2a-32418f1a77fa" />

</p>
<p>
I downloaded the osTIcket Installation Files and unzipped it onto the Virtual Machines desktop. These files will be use throughout this lab to install osTicket and some of it's dependences. 
</p>
<br />


<p>
<img width="556" height="595" alt="Install IIS with CGI" src="https://github.com/user-attachments/assets/6882cc8b-d567-4496-9cf7-f3994c0fd2aa" />

</p>
<p> 
  I installed IIS (Internet Information Services) whit CGI (Common Gateway Interface) enabled. This will act as a web server allowing me to run the osTicket application
</p>
<br />

<p>
  <img width="1167" height="1019" alt="image" src="https://github.com/user-attachments/assets/57e2365f-9227-47da-b35b-8a634fd3e735" />

</p>
<p> 
After Installing IIS I installed PHP and its components (which osTicket uses to execute application functions) as well as my SQL (a backend database) I then registered PHP with IIS, allowing IIS to process PHP files that are required by the osTicket application. 
</p>
<br />

<p>

  
<img width="972" height="738" alt="image" src="https://github.com/user-attachments/assets/370d8da4-4029-4589-8dd7-13a83d6ff5cc" />


</p>
<p>
I extracted the osTicket application and placed its upload directory inside the IIS web root. I then renamed the directory to osTicket so the application could be accessed through the IIS website.
</p>
<br />

<p>
<img width="1773" height="1031" alt="image" src="https://github.com/user-attachments/assets/7b6e3d50-80f0-462f-9f51-9745770a2b73" />


</p>
<p>
I accessed the osTicket application through IIS using the default HTTP port. At this point, the osTicket installer detected the application environment
</p>
<br />

</p>
<img width="840" height="943" alt="image" src="https://github.com/user-attachments/assets/9199bbfe-ec2d-44b3-b400-564ba503784f" />

</p>
<p>
I used HeidiSQL to connect to the MySQL server and created a database named osTicket. This database will provide the data storage required by the osTicket application. I connected the osTicket application to the MySQL database which allows osTicket to store and retrieve application data from the database server.
</p>
<br />

</p>
<img width="1062" height="818" alt="image" src="https://github.com/user-attachments/assets/511ca35c-649b-474d-8529-f9b9f8e9da44" />

</p>
<p>
After connecting the osTicket application to my database I was able to successfully install osTicket.
</p>
<br />

## Summary

This lab documents the installation and configuration of **osTicket on a Windows Virtual Machine (VM) hosted in Microsoft Azure**. The lab included setting up Internet Information Services (IIS) with Common Gateway Interface (CGI), installing and configuring PHP and MySQL, configuring PHP extensions, deploying osTicket through IIS, creating the osTicket database with HeidiSQL, and connecting the application to the database. The installation was then verified by accessing both the staff login page and end-user portal. 
