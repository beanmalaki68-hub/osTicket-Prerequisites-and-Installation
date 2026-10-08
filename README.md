<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>


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

# Step 1 - Resource Group Creation

First, I started by creating a Resource Group within Microsoft Azure. Resource Groups help organize and manage the different resources created within Azure. This is important for businesses because they may have many different projects and teams using Azure, and Resource Groups allow related resources to be grouped together and managed separately. For example, a business could create a separate Resource Group for each project, making it easier to organize, manage, monitor, and eventually remove the resources associated with that project.

<h2>Video Walkthrough</h2>

https://youtu.be/e3He0nQEsnY

# Step Two - Virtual Machine Creation 
 
Then, I created a Virtual Machine (VM) within Microsoft Azure. This Virtual Machine will act as my computer, which I will use to install osTicket. Although Virtual Machines are not physical computers, they function like physical computers by using virtualized resources such as processing power, memory, storage, and networking from physical hardware in Microsoft's Azure data centers. In this case, I will remotely connect to this Virtual Machine and install and configure osTicket on it.

<h2>Video Walkthrough</h2>

https://youtu.be/5Uj9-WLCu1s

# Step 3 - Remoting into the Virtual Machine 

Then, I used Remote Desktop Protocol (RDP) to log into the Virtual Machine that I had just created. This is a useful tool for IT professionals to understand because there are many situations where a Help Desk professional may need to remotely access an end user’s device to troubleshoot and resolve an issue. Remote access allows the technician to work on the device without having to be physically present at the user’s location.

<h2>Video Walkthruogh</h2>

https://youtu.be/yIaEIG8M-ow

# Step 4 - Installing osticket zip file onto the Virtual Machine

Next, I used the link provided to me through CourseCareers to download the ZIP file onto the Virtual Machine. Since osTicket is a web-based application, it requires several components to run on the back end, such as a web server and a database. I downloaded the ZIP file because it contains the osTicket application files that I will use while configuring the components required to install and run osTicket.

<h2>Video Walkthrough</h2>

https://youtu.be/rOWTv8wkPdw

# Step 5 - Installing IIS & CGI

Then, I installed IIS and CGI. IIS (Internet Information Services) is the web server I will use to process requests made when accessing osTicket. I also installed CGI (Common Gateway Interface), which allows IIS to communicate with PHP, the programming language used by osTicket, so that PHP can process the request and generate a response.

<h2>Video Walkthrough</h2>

https://youtu.be/eRx2HAL9SKw

# Step 6 - Installing PHP Manager

After installing IIS and CGI, I then installed PHP Manager, which is a tool used to manage and configure PHP on IIS. PHP is the programming language that osTicket uses. CGI acts as the middleman between IIS and PHP, allowing IIS to communicate with PHP so that requests can be processed and responses can be returned to the user.

<h2>Video Walkthrough</h2>

https://youtu.be/fyP3Dpw8ic4

# Step 7 - Installing the Rewrite Component 

I then installed the Rewrite Module, which allows the IIS web server to rewrite or route URLs based on the application’s requirements and configuration.

<h2>Video Walkthrough</h2>

https://youtu.be/4BUkbTUN07k


# Step 8 - Creating a PHP file on the C: drive and extracting the PHP language onto the file

I then created a folder on the C: drive called PHP and extracted the PHP files into the folder I had just created. These files provide the PHP environment needed to run applications such as osTicket.

<h2>Video Walkthrough</h2>

https://youtu.be/xLx9BB0gkx8

# Step 9 - Installing the VC_Redist file

Next, I then downloaded and installed VC_redist, which provides runtime components that some Windows programs and software dependencies need in order to run properly. Installing it helps make sure that the necessary supporting components are available on my Virtual Machine as I set up the environment needed to run osTicket.

<h2>Video Walkthrough</h2>

https://youtu.be/T1GCAs1K1gc

# Step 10 - Installing the SQL Database

I then installed the SQL database, which will store the data that our osTicket system will use. This can include information such as users, tickets, groups, permissions, and other data needed for the osTicket system to function properly.

<h2>Video Walkthorugh</h2>

https://youtu.be/dEf6IU2gqG8

# Step 11 - Making our IIS webserver aware of PHP

Next, I logged into IIS with administrator privileges and registered the new PHP version. This allows IIS to locate the PHP installation and know which version of PHP to use when processing PHP applications. This is important because osTicket is built using PHP, so IIS needs to be properly configured to work with PHP in order for osTicket to function correctly.

<h2>Video Walkthrough</h2>

https://youtu.be/zWO79e33LG0


# Step 12 - "Installing osTicket" 

I extracted the osTicket files and placed them in C:\inetpub\wwwroot, which is the web root directory used by IIS. I then renamed the folder from “upload” to “osTicket” so it would be easier to identify and access. Finally, I restarted IIS so the web server could reload the changes and serve the osTicket application.This is important because it places the osTicket application files in the web root directory where IIS can access and serve them.

<h2>Video Walkthorugh</h2>

https://youtu.be/ZnwRAmJmumk


# Step 13 - Browsing to osTicket and enabling extensions 

I then went to IIS and browsed to osTicket to make sure that everything I had configured so far was working correctly. After that, I enabled the PHP extensions php_imap.dll, php_intl.dll, and php_opcache.dll. These extensions are important because they provide additional functionality that osTicket can use, including email communication, internationalization features, and improved PHP performance.

<h2>Video Walkthrough</h2>

https://youtu.be/ZI9ajvcD9jY


# Step 14 - Renaming Config file and changing permissions

Next, I located the sample configuration file and renamed it so that osTicket would recognize it as the main configuration file. I then changed the permissions on the file to give the necessary access for osTicket to configure and use the file during the installation process.

<h2>Video Walkthrough</h2>

https://youtu.be/_2B4JAtzC4o


# Step 15 - Setting up osTicket in brower and installing HeidiSQL

I continued the osTicket setup in the browser by giving the help desk a name and default email address. Then I used HeidiSQL to create the osTicket MySQL database, which will store the information used by the help desk system. Finally, I entered the database name and login information into the osTicket installer and clicked Install Now so osTicket could connect to the database and create what it needs to operate.

<h2>Video Walkthrough</h2>

https://youtu.be/VyMJJD70mtE


