# arm-templates
Azure Workshop "ARM Templates"
---------------

Downloads
---------------
[VS Code](https://aka.ms/win32-x64-user-stable)\
[Git](https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/Git-2.23.0-64-bit.exe)\
[Azure CLI](https://aka.ms/installazurecliwindows)
[Azure Quick Start Templates](https://github.com/Azure/azure-quickstart-templates)\

Paths
---------------
```
C:\Program Files (x86)\Microsoft SDKs\Azure\CLI2\Lib\site-packages\azure\mgmt\apimanagement\models\
```

Git Commands
---------------
```
git --version
```
```
git config --global user.name "Vārds Uzvārds"
```
```
git config --global user.email vards@domains.lv
```
```
git config --list
```
```
"git.path": "C:\\Program Files\\Git\\bin\\git.exe",
"git.autofetch": true
```

Azure CLI Commands
---------------
```
az login
az group create --name Demo --location westeurope
az group delete --name Demo --yes
az group deployment validate --resource-group Learn-ARM --template-file 'C:\Users\azureadmin\Desktop\Demo.json'
az group deployment create --resource-group Learn-ARM --template-file 'C:\Users\azureadmin\Desktop\Demo.json'
az group deployment validate --resource-group Learn-ARM --template-file 'C:\Users\azureadmin\Desktop\Demo.json' --parameters 'C:\Users\azureadmin\Desktop\Demo.parameters.json'
az group deployment create --resource-group Learn-ARM --template-file 'C:\Users\azureadmin\Desktop\Demo.json' --parameters 'C:\Users\azureadmin\Desktop\Demo.parameters.json'
```

Azure DevOps Commands
---------------
```
az vm show --resource-group Learn-ARM --name Learn-ARM-VM --query hardwareProfile.vmSize --output table
```