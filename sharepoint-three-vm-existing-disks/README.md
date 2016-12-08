# Create a new Sharepoint Farm with 3 VMs (from existing storage account disks)

This template creates three new Azure VMs, each with a public IP address and load balancer and a VNet, it configures one VM to be an AD DC for a new Forest and Domain, one with SQL Server domain joined and a third VM with a Sharepoint farm and  site, all VMs have public facing RDP. This template will only work if the resource group you are deploying to already contains a storage account with all existing disks for an already created (but somehow errored) SP 2013 Non-HA farm.

Click the button below to deploy

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FCCondeluci%2Fazure-sp-2013-nonHA-farm%2Fmaster%2Fsharepoint-three-vm-existing-disks%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2FCCondeluci%2Fazure-sp-2013-nonHA-farm%2Fmaster%2Fsharepoint-three-vm-existing-disks%2Fazuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

Notes: Sharepoint farm name must not contain spaces.
