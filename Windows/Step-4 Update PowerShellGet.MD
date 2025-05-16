### ✅ **Run PowerShell as Administrator**

-   Press `Windows + S`, search **PowerShell**
    
-   Right-click → **Run as administrator**
    

----------

### ✅ **Check Current Version of PowerShellGet**

    Get-Module -Name PowerShellGet -ListAvailable 

----------

### ✅ **Install/Update to Latest PowerShellGet**

    Install-Module -Name PowerShellGet -Force -AllowClobber 

> `-Force` ensures it updates if already installed.  
> `-AllowClobber` prevents conflicts with existing versions.

----------

### ✅ **Restart PowerShell**

Once updated, **restart your PowerShell session** to start using the latest version.
