Generate Azure VM size availability matrix
==========================================

            
Description

This PowerShell script allows you to export a matrix of the availability of VM sizes per location in Microsoft Azure. The availability matrix will be in CSV format and gives you clear insight on which VM sizes are available in which Azure location. Note
 that the script is built for Azure Resource Manager (ARM).


Importing the CSV into Excel gives you the ability to filter based on location, cores, memory, etc.


![Image](https://github.com/azureautomation/generate-azure-vm-size-availability-matrix/raw/master/VMSize-Matrix.png)

Prerequisites

This script needs the Azure PowerShell cmdlets to be installed, which can be downloaded here: [https://azure.microsoft.com/en-us/downloads/](https://azure.microsoft.com/en-us/downloads/). Additionally, a Microsoft Azure account
 is needed to retrieve the data.

Usage

The only mandatory parameter, is the 'Path', which defines where to export the CSV file. To export the CSV with all default options, run the script with the -Path parameter as follows (the script will ask for Azure credentials):

Export-AzureVmSizes.ps1 -Path ./VMSize.csv

To get help about the script, use the Get-Help command:

Get-Help Export-AzureVmSizes.ps1 -Full
Code

 

 

        
    
TechNet gallery is retiring! This script was migrated from TechNet script center to GitHub by Microsoft Azure Automation product group. All the Script Center fields like Rating, RatingCount and DownloadCount have been carried over to Github as-is for the migrated scripts only. Note : The Script Center fields will not be applicable for the new repositories created in Github & hence those fields will not show up for new Github repositories.
