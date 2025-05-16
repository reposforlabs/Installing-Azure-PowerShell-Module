## ✅ Update PowerShellGet

### 1.  **Run PowerShell as Administrator**

-   Press  `Windows + S`, search  **PowerShell**
    
-   Right-click →  **Run as administrator**
    

----------

### 2.  **Enable TLS 1.2**

    [Net.ServicePointManager]::SecurityProtocol = [Net.ServicePointManager]::SecurityProtocol -bor [Net.SecurityProtocolType]::Tls12
