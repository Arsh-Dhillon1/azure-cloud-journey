az group create --name azure-lab-rg --location eastus // Creates new Azure resource group
az group list --output table // To verify the resource group
az group delete --name azure-lag-rg --no-wait --yes // Delete the created Resource Group