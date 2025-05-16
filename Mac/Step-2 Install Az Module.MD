### ✅ **Launch PowerShell Core**

In your terminal, type:

``` bash
pwsh
```

----------

### ✅ **Install the Az Module**

Run the following command inside PowerShell:

``` bash
Install-Module -Name Az -Scope CurrentUser -Repository PSGallery -Force 
```

-   `-Scope CurrentUser`: Installs the module only for your user (no admin required).
    
-   `-Force`: Skips prompts (useful for smoother install).
    
-   `-Repository PSGallery`: Specifies the PowerShell Gallery as the source.
    

----------

### ✅**Trust the PSGallery (If Prompted)**

If you’re asked to trust the PowerShell Gallery as a source, type `Y` and press Enter.

----------

### ✅**Verify the Installation**

After installation, check it:

``` bash
Get-Module -Name Az -ListAvailable
```

You should see something like:

``` bash
Directory: /Users/yourusername/.local/share/powershell/Modules

ModuleType Version    Name                                ExportedCommands
---------- -------    ----                                ----------------
Script     11.5.0     Az                                  {Get-AzResource, New-AzResourceGroup, ...}
```

----------

### ✅**Login to Azure**

To log in to your Azure account:

``` bash
Connect-AzAccount
```
A browser window will open for you to authenticate.
