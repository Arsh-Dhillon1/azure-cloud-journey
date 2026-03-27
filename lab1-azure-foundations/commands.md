//Creating Users
# Command to create a user in Entra ID
az ad user create --display-name "Dipesh Prabhakar" --user-principal-name dipeshprabhakar@<MY_TENANT>.onmicrosoft.com --password "HIDDEN" --force-change-password-next-sign-in true
# Command to show user details in Entra ID
az ad user show --id bonzodog@<MY_TENANT>.onmicrosoft.com

# Output
{
  "displayName": "Bonzo Dog",
  "userPrincipalName": "bonzodog@<MY_TENANT>.onmicrosoft.com",
  "id": "REDACTED-USER-OBJECT-ID"
}

//Creating Group
az group create --name azure-lab-rg --location eastus // Creates new Azure resource group
az group list --output table // To verify the resource group
az group delete --name azure-lag-rg --no-wait --yes // Delete the created Resource Group