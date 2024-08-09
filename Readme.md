### Welcome to ASP.NET Core Application Deployment on Windows Server.

**Prerequisite**
- Install [ASP.NET Core](https://dotnet.microsoft.com/en-us/download/dotnet/6.0) as you required
- Install [Windows Hosting Bundle](https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-aspnetcore-6.0.32-windows-x64-installer) as you required
- Making Inbound policies as you expected

##### Let`s get started

**Step-01**
- Install Web Server (IIS) from Server Manager (Add Roles & Features). If you are using Windows then install IIS from the Control panel.

**Step-02**
- Make a website named `WebsiteName` under the `Sites` menu in IIS
- Binding `http/https`, and `IP` & assign `port` number. Select `SSL certificate` then press ok.
- Configure the application pool from the `Application Pools` menu

**Step-03**
- Making build code to publish & configure database in MSSQL server
- Deploy the code on `C:\inetpub\wwwroot\WebsiteName`
- Select the `Authentication` option & click on `Edit Permissions` Go to the `Security` tab. Find `IIS_IUSRS` & give full permission.
- Install Windows Hosting Bundle
- Go to browser http://IP:58623/ or http://localhost:58623/
- Restart the Server

**Step-04**
- Windows Defender Firewall > Advanced Settings
- Make an Inbound policy for web applications.
- Make an Inbound policy for MSSQL Server.

#### 👍 👍 👍 Done! Have a Good Day 👍 👍 👍
