#### Welcome to ASP.NET Core Application Deployment.

***Prerequisite***
- Install ASP.NET Core as you required
- Install [Windows Hosting Bundle](https://download.visualstudio.microsoft.com/download/pr/df69e0b0-7666-43f2-9a1d-5c239f0a5d70/ecd33d20405bbc0f9caf30983dd255bf/aspnetcore-runtime-6.0.30-win-x64.exe) as you required
- Making Inbound policies as you expected

##### Let's get started
***Step-01***
- Install Web Server (IIS) from Server Manager (Add Roles & Features). If you are use windows then install IIS from Control panel.

***Step-02***
- Making website named 'websiteName' under 'Sites' menu in IIS
- Binding 'http/https', 'IP' & assign 'port' number. Select 'SSL certificate' then press ok.
- Configure the application pool from 'Application Pools' menu

***Step-03***
- Making build code to publish & configure database in MSSQL server
- Deploy the code on 'C:\inetpub\wwwroot\websiteName'
- Select 'Authentication' option & click on 'Edit Permissions' Go to 'security' tab. Find IIS_IUSRS & give full permission.
- Install [Windows Hosting Bundle](https://download.visualstudio.microsoft.com/download/pr/df69e0b0-7666-43f2-9a1d-5c239f0a5d70/ecd33d20405bbc0f9caf30983dd255bf/aspnetcore-runtime-6.0.30-win-x64.exe)
- Go to browser http://192.168.3.100:58623/ or http://localhost:58623/

***Step-04***
- Windows Defender Firewall > Advanced Settings
- Make an Inbound policy for web application.
- Make an Inbound policy for MSSQL Server.