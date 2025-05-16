## ✅ Install `jq`

`jq` is available in the default Ubuntu repositories:

``` bash
sudo apt update
sudo apt install jq -y
```

Verify installation:

```bash
jq --version
 ```

----------

## ✅ Install PowerShell 7

Microsoft provides official packages for PowerShell. Follow these steps:

### **Download and register the Microsoft repository**

``` bash
# Install prerequisites 
sudo apt update
sudo apt install -y wget apt-transport-https software-properties-common 
# Import the Microsoft GPG key 
wget -q https://packages.microsoft.com/config/ubuntu/22.04/packages-microsoft-prod.deb 
# Register the Microsoft repository 
sudo dpkg -i packages-microsoft-prod.deb # Clean up  rm packages-microsoft-prod.deb
```

### ✅**Install PowerShell**

``` bash
sudo apt update
sudo apt install -y powershell
```

### ✅**Launch PowerShell**

``` bash
pwsh
``` 

This will launch the PowerShell 7 shell.

----------

## ✅ Verify Installation

Inside PowerShell:

``` PowerShell

$PSVersionTable.PSVersion
```

You should see something like `7.x.x`.
