Step 1 — Create Resource Group
az group create \
--name RG-network-lab \
--location centralindia

Step 2 — Create VNet
az network vnet create \
--resource-group RG-network-lab \
--name lab-vnet \
--address-prefix 10.0.0.0/16 \
--subnet-name web-subnet \
--subnet-prefix 10.0.1.0/24

Step 3 — Create App Subnet
az network vnet subnet create \
--resource-group RG-network-lab \
--vnet-name lab-vnet \
--name app-subnet \
--address-prefix 10.0.2.0/24

Step 4 — Create DB Subnet
az network vnet subnet create \
--resource-group RG-network-lab \
--vnet-name lab-vnet \
--name db-subnet \
--address-prefix 10.0.3.0/24