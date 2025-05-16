
----------
## ✅ **Check if TLS 1.2 is enabled in PowerShell session**

    [Net.ServicePointManager]::SecurityProtocol 

### 🔍 What to look for:

If the output includes `Tls12`, it means **TLS 1.2 is enabled**.

    Tls, Tls11, Tls12 

> ✅ This confirms TLS 1.2 is part of the allowed protocols for secure connections.

----------

## ✅ **Enable TLS 1.2**

    [Net.ServicePointManager]::SecurityProtocol = [Net.ServicePointManager]::SecurityProtocol -bor [Net.SecurityProtocolType]::Tls12

