### ✅ Install the Azure PowerShell Module

Once in PowerShell (`pwsh` prompt):

``` powershell

Install-Module -Name Az -Scope CurrentUser -Repository PSGallery -Force
```

> If prompted to trust the PSGallery repository, type `Y` and press Enter.

----------

### ✅ Verify Installation

``` PowerShell

Get-Module -ListAvailable Az
```

You can now log in to Azure with:

``` PowerShell
Connect-AzAccount
```

----------
### ✅  **Sign in to Azure**

Use the following command to log in:

``` PowerShell
Connect-AzAccount

----------

### 🔁 To Exit PowerShell:

``` PowerShell
exit
```
