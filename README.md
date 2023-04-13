# Virtual Machine from Azure Snapshot Solution

This solution will create a new Azure Virtual Machine using an existing Azure Snapshot.

## Assumptions

The following resources should already exist in your Azure subscription before deploying this ARM template:

- Virtual Network
- Snapshot

## Deployment Options

### Try with Azure Portal

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fjamasten%2FAzureVirtualMachineFromSnapshot%2Fmain%2Fsolution.json)
[![Deploy to Azure Gov](https://aka.ms/deploytoazuregovbutton)](https://portal.azure.us/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fjamasten%2FAzureVirtualMachineFromSnapshot%2Fmain%2Fsolution.json)

### Try with PowerShell

```powershell
New-AzResourceGroupDeployment `
    -ResourceGroupName '<Azure Resource Group>' `
    -TemplateUri 'https://raw.githubusercontent.com/jamasten/AzureVirtualMachineFromSnapshot/main/solution.json'
```

### Try with CLI

````cli
az deployment group create \
    --resource-group '<Azure Resource Group>' \
    --template-uri 'https://raw.githubusercontent.com/jamasten/AzureVirtualMachineFromSnapshot/main/solution.json'
````
