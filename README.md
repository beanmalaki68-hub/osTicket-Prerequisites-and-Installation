<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>


https://github.com/user-attachments/assets/fb1cece7-7732-4b71-a7f8-ef257011061a



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

