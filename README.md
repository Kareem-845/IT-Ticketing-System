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
<img width="976" height="515" alt="Screenshot 2026-09-23 100941" src="https://github.com/user-attachments/assets/da43456e-6ce4-4987-a203-6ba4a2e490da" />


Step 5 - Install MySQL
A MySQL database server was installed on Windows Server 2019. A dedicated database was created for osTicket.

Step 6 - Download osTicket
The osTicket installation package was downloaded from the official site. The installation files were extracted and prepared for deployment through IIS. The files were placed under C:\inetpub\wwwroot\osTicket. This allows IIS to serve the application through the web browser.

Step 7 - Configure osTicket
The osTicket configuration file was prepared and the required permissions were configured. The osTicket web installer was then accessed through http://localhost/osTicket. The installer checked the server environment for the required PHP extensions and system components.

Step 8 - Configure the osTicket installation
The osTicket installation wizard was completed. The help desk was configured with the name IT Help Desk. An administrative account was also created for managing the help desk. The database connection information was entered into the osTicket installation wizard.

Step 8 - Access the osTicket Staff Panel
The osTicket staff panel was accessed after installation. 

The staff panel provides technicians access to:
View tickets
Assign tickets
Change ticket priority
Add internal notes
Communicate with users
Track ticket activity
Resolve tickets

Step 9 - Configure the IT Support Department

An IT Support department was created within osTicket. This department represents the technical support team responsible for handling user incidents. Additional departments were created, such as Hardware and Network Support. The primary department used for this lab was IT Support.

Step 10 - Create an IT Support Technician

An IT support technician account was created in osTicket. The technician was assigned to the IT Support department to simulate a service desk employee.

Step 11 - Create a test user
The existing Active Directory environment was used to simulate an employee. A domain user was created in Active Directory for this lab utilizing the Windows 10 workstation.

Step 12 - Submit an IT Ticket

The Windows 10 client was used to access the osTicket web interface.

Step 13 - Review the Ticket

An IT Technician logged in to the osTicket staff panel and reviewed the ticket submitted.

Step 14 - Assign and Prioritize the ticket

The ticket was assigned to the IT Support department. The priority was changed based on simulated impact.

