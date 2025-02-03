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

- Azure Virtual Machine
- Internet Information Services (IIS)
- PHP Manager
- Rewrite Module
- VC Redist
- MySQL
- Heidi SQL
- osTicket v1.15.8
- Link to downloads: https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6


<h2>Installation Steps</h2>

<p> 1.) Start by creating a virtual machine through Azure Portal https://portal.azure.com/. Choose Windows 10 Pro, version 22H2, as the operating system. Make sure your virtual machine has at least 2 vCPUs and 16GB of memory for optimal performance.

  2.) After setting up your virtual machine, connect to it using the public IP address assigned to it. Use the Remote Desktop Connection app to establish the connection.

 
  ![public ip address 2](https://github.com/user-attachments/assets/b6af105b-4d0f-4250-8d19-1f1c174b4900)

 3.) Once you have connected to your virtual machine you will want to go to your control panel. From the control panel open up programs. Select, Turn Windows features on and off.
</p>

 ![c panel](https://github.com/user-attachments/assets/4e7a3f8c-1261-4dd7-a8c5-0de789fa3674)
![turn windows on or off](https://github.com/user-attachments/assets/9c77099b-b59d-47ce-b024-229768194f12)




</p>
<br />

<p>
</p>
<p> 4.) You will want to install / enable IIS in Windows with CGI and Common HTTP Features

World Wide Web Services -> Application Development Features -> [X] CGI

![IIs](https://github.com/user-attachments/assets/9b987bc1-3350-4848-a15b-adc63e793e8b)

To make sure the IIS is installed / enabled go to a browser of your choice and search for 127.0.0.1 It should look something like this.

<p>

  ![IIS windows](https://github.com/user-attachments/assets/a72127f6-5bb2-419e-ac9e-603c516ea602)

5.) Now that the IIS is enabled, From the Installation Files, download and install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi) Go through the install wizard and complete the install.

6.) Next from the Installation Files, download and install the Rewrite Module (rewrite_amd64_en-US.msi)
![Screenshot_4](https://github.com/user-attachments/assets/b7c80b06-6741-4488-b7b4-a25a9a0fb816)

7.) Create a folder in the C drive called PHP.

8.) From the Installation Files, download PHP 7.3.8 (php-7.3.88-nts-Win32-VC15-x866.zip) and unzip the contents into C:\PHP
<p>

  ![Screenshot_6](https://github.com/user-attachments/assets/97517a45-f939-4563-b89f-a0890a0da9b9)

9.) Once you have downloaded and extracted the zip file into the PHP folder on the C drive, download and install the VC_redist.x86.exe from the installation files. Go through the setup wizard to finish setting up and installing the VC_redist.x86.exe.

![Screenshot_7](https://github.com/user-attachments/assets/f619d30e-b1a0-4977-807d-f9d0d33bf15f)

10.) Download and install MySQL 5.5.62 (mysql-5.5.62-win32.msi) Run the setup wizard: Typical Setup -> Launch Configuration Wizard (after install) -> Standard Configuration ->

username and password is root

![Screenshot_9](https://github.com/user-attachments/assets/ae5d9f7f-4cad-46dc-b174-c52b0a10a310)

</p>
<br />
