
# Sitecore 9 Machine Prerequisites Check with PowerShell

PowerShell script that help verify that you've got machine prerequisites covered before installing **Sitecore 9**.
Based on [Sitecore 9 Installation Guide](https://dev.sitecore.net/Downloads/Sitecore_Experience_Platform/90/Sitecore_Experience_Platform_90_Initial_Release.aspx) and [Sitecore Compatibility Table](https://kb.sitecore.net/articles/087164)

**Run as an Administrator:** >>     *.\IsThisSitecore9Ready.ps1*

## Checks:
 - Hardware requirements (Core and Memory check) 
 
 - Operating System compatibility (Windows Server 2012 R2 (64-bit) / 2016 (32-bit/64-bit) / Windows 10 (32-bit/64-bit) / Windows 8.1 (32-bit/64-bit)
 - System Folder Permissions (The script **will set IIS_IUSRS Modify permissions** to folders defined in section **2.3.1 File System Permissions** of the [Sitecore 9 Installation Guide](https://dev.sitecore.net/Downloads/Sitecore_Experience_Platform/90/Sitecore_Experience_Platform_90_Initial_Release.aspx) ) 
 - IIS version (8.5+)
 - .NET Framework (4.6.2+). SQL Server 2014 SP2 or 2016 SP1 
 - JavaRuntime (and confirms JAVA_HOME path Windows EnvironmentVariable is set)
 - Checks and registers SIF (SitecoreInstallFramework and SitecoreFundamentals)

![IsThisSitecore9Ready.ps1 results](https://i.imgur.com/2jXjO0l.png)
