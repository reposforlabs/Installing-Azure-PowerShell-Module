## 🔄 Update NuGet Provider in PowerShell

PowerShell uses **NuGet** as a package provider to install modules from the PowerShell Gallery.

### ✅ Check Current NuGet Version

    Get-PackageProvider -Name NuGet 

### ✅ Update NuGet

    Install-PackageProvider -Name NuGet -Force -Scope AllUsers 

> If prompted to trust the repository, enter `Y` to continue.
