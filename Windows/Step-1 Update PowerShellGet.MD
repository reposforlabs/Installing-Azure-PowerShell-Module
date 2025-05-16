## ✅ Update PowerShellGet

### 1. **Run PowerShell as Administrator**

-   Press `Windows + S`, search **PowerShell**
    
-   Right-click → **Run as administrator**
    

----------

### 2. **Check Current Version of PowerShellGet**

    Get-Module -Name PowerShellGet -ListAvailable 

----------

### 3. **Install/Update to Latest PowerShellGet**

    Install-Module -Name PowerShellGet -Force -AllowClobber 

> `-Force` ensures it updates if already installed.  
> `-AllowClobber` prevents conflicts with existing versions.

----------

### 4. **Restart PowerShell**

Once updated, **restart your PowerShell session** to start using the latest version.
