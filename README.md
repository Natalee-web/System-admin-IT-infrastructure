Local Web Server Setup (Apache via XAMPP)

---
Project Description
This project demonstrates the manual setup of a local Apache web server on a Windows environment. It covers service initialization, directory configuration, and the deployment of a custom HTML landing page. This setup is a foundational task for understanding how web servers handle HTTP requests and serve files from a local DocumentRoot.
Services Configured
Apache HTTP Server (v2.4): The primary service responsible for listening on Port 80 and processing web requests.

XAMPP Control Panel: The management interface used to initialize and monitor the Apache daemon.

Localhost (127.0.0.1): The loopback address used to access the server locally via a web browser.
C:/xampp/htdocs/
└── my_local_server/            
    ├── index.html               
    ├── assets/                  
    │   ├── css/                 
    │   ├── js/                  
    │   └── images/             
    └── logs/                   
1. Installation & Service Start
Installed the XAMPP stack for Windows.

Opened the XAMPP Control Panel and started the Apache module.

Verification: Confirmed the status turned green and assigned PID/Ports.

<img width="664" height="427" alt="server1" src="https://github.com/user-attachments/assets/cd067a27-0588-444b-b6bd-15e4e306c793" />

Manual Directory Setup
Using the terminal (Git Bash) or File Explorer, the project directory was created to isolate the website files.
<img width="1000" height="152" alt="server3" src="https://github.com/user-attachments/assets/af049b7f-bf61-4b1d-af1b-0a032ebf07d6" />


3. Web Content Deployment
Created an index.html file to test the server's ability to render HTML5 content.
4. Browser Verification
Accessed the server via the browser to ensure the DocumentRoot mapping is functional.

URL: http://localhost/my_local_server/

<img width="570" height="404" alt="server2" src="https://github.com/user-attachments/assets/1e9f2049-bd32-42af-a37c-e26ad4e05594" />


 Technical Summary
DocumentRoot: The server is configured to look at C:\xampp\htdocs\ by default. By creating a subfolder, we utilize Apache's ability to serve multiple local projects.

Permissions: Since this is a local Windows environment, standard user permissions were applied to the htdocs folder to allow seamless file editing.

Protocol: Uses standard HTTP over Port 80.
