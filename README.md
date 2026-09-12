# IT-Ticketing-System

1.Lab Overview
This lab demonstrates the deployment and use of osTicket, an open source IT help desk ticketing platform. osTicket was deployed using Docker containers with a MySQL database and used to simulate a realistic IT support workflow. The lab focused on creating, managing, documenting, and resolving support tickets.

2.Objectives
The objectives of this lab were to :
Deploy osTicket on Windows Server 2019
Configure IIS as the web server
Configure PHP for use with IIS
Configure a MySQL compatible database for osTicket
Configure the osTicket help desk
Use the existing Active Directory environment to simulate users
Create and manage IT support tickets
Demonstrate ticket assignment and prioritization
Document troubleshooting activities
Resolve and close support incidents

3.Lab Environment
Device    Operating System      Role
Server    Windows Server 2019   Domain Controller, DNS, IIS, osTicket Server 
Client    Windows 10            User workstation

4.Lab Procedure

Step 1 - Verify Existing Environment
The Windows Server 2019 and Windows 10 virtual machines were started and verified before deploying the ticketing system.
The Windows 10 machine is joined to the Active Directory domain. Network connectivity was tested using the ping command.

Step 2 - Install IIS
Internet Information Systems was installed on Windows Server 2019 to provide the web server required by osTicket.

Step 3 - Verify IIS
After installation, IIS was tested opening a web browser on Windows Server 2019 and navigating to http://localhost.
<img width="756" height="570" alt="Screenshot 2026-09-08 130446" src="https://github.com/user-attachments/assets/5a520fa2-93c4-4eff-9dda-2736249cb07e" />

Step 4 - Install PHP
PHP was installed and configured for use with IIS. It allows the web server to execute the PHP code used by osTicket.The 
installation was configured through IIS using FastCGI.

