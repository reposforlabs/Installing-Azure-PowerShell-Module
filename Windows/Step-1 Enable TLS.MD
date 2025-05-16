## ✅ Update PowerShellGet

1. **Run PowerShell as Administrator**

   Press  `Windows + S`, search  **PowerShell**
    
-   Right-click →  **Run as administrator**
    

----------
## ✅ 2A. **Check if TLS 1.2 is enabled in PowerShell session**

    [Net.ServicePointManager]::SecurityProtocol 

### 🔍 What to look for:

If the output includes `Tls12`, it means **TLS 1.2 is enabled**.

    Tls, Tls11, Tls12 

> ✅ This confirms TLS 1.2 is part of the allowed protocols for secure connections.

----------

## ✅ 2B. **Check if TLS 1.2 is enabled at the OS level (Windows Registry)**

While the above command checks **what PowerShell/.NET will use**, you can also check **system-wide support** via the registry.

### 🔎 View current registry settings:

    Get-ItemProperty -Path 'HKLM:\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client' -Name Enabled 

If it returns:

-   `Enabled : 1` → ✅ TLS 1.2 is enabled at the OS level for client-side apps
    
-   `Enabled : 0` or not found → ❌ It’s not enabled

## 3. **Enable TLS 1.2**

    [Net.ServicePointManager]::SecurityProtocol = [Net.ServicePointManager]::SecurityProtocol -bor [Net.SecurityProtocolType]::Tls12

