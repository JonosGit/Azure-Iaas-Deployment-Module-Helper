# Iaas-Deployment-Helper-Module
Azure PowerShell Deployment Helper Module

Version 2.0 Beta

This Zip contains a module and module defination file that can be imported by extracting the Zip and placing the extracted folder created by the Zip in one of the three supported PowerShell 3.x and above Module locations.
For Example:

C:\Program Files\WindowsPowerShell\Modules\azpsinfrahelper

This Module Requires Azure PowerShell 2.x and above. 
Before executing Ipmort-module extract the zip to a temporary directory.

Locate the azpsinfrahelper.psm1 file and using the PowerShell ISE modify the following 2 global parameters, one for your Azure Profile location, the other for the Azure Region you wish to deploy in. Once updated save file with you changed.
Param(
$Location = 'WestUs',
$Profile = "C:\Temp\azureprofile.json"
	)

Now Open a new PS1 session as a local administrator on the machine and run 'Import-Module azpsinfrahelper'.

Once complete you can get to the core functions by typing:
'Get-azNetinfo', 'Install-Ext', 'New-AzNSG', 'New-AzVnet','New-AzVM','New-AzResGrp','New-AzStorage'