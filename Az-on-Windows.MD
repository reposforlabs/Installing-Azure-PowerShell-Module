## ✅ Step-by-Step Guide

### **1. Open Windows PowerShell as Administrator**

-   Press `Windows + S`, type **PowerShell**.
    
-   Right-click on **Windows PowerShell** > **Run as administrator**.
    

----------

### **2. Install the PowerShellGet Module (if needed)**

Before installing Azure PowerShell, ensure you have an updated version of PowerShellGet.

    Install-Module -Name PowerShellGet -Force -AllowClobber 

----------

### **3. Install Azure PowerShell Module**

Run the following command to install the Az module (the recommended Azure PowerShell module):

    Install-Module -Name Az -AllowClobber -Scope AllUsers 

> 🔹 `-AllowClobber` ensures that existing commands can be overwritten if necessary.  
> 🔹 `-Scope AllUsers` makes it available to all users on the system.

----------

### **4. Confirm the Installation**

After installation, you can import the module and check if it's working:

    Import-Module Az
    Get-Module Az -ListAvailable 

----------

### **5. Sign in to Azure**

Use the following command to log in:

    Connect-AzAccount

A sign-in window will appear. Enter your Azure credentials.

----------

## 🧪 Optional: Verify Installed Modules

    Get-InstalledModule -Name Az 

----------

## 🔄 Update Azure PowerShell in the Future

    Update-Module -Name Az 



