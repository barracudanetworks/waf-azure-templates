# Barracuda Web Application Firewall for Azure - Custom in Availability Set

## Introduction
This Azure Resource Manager template will deploy a pair (or whatever number you request) of Barracuda Web Application Firewalls into your selected Virtual Network using the Availability Set method for resiliency

## Prerequisites
The solution does a check of the template when you use the provided scripts. It does require that [Programmatic Deployment](https://azure.microsoft.com/en-us/blog/working-with-marketplace-images-on-azure-resource-manager/) is enabled for the Barracuda Web Application Firewall BYOL or PAYG images. Barracuda recommends use of **D**, **D_v2**, **F** or newer series. 

You can enable programatic deployment via Powershell using the Cloud Shell feature in the portal. Below are two powershell examples for byol and hourly, please adapt as required to your version of powershell and byol or hourly license requirement.

`Get-AzMarketplaceTerms -Publisher "barracudanetworks" -Product "waf" -Name "byol" | Set-AzMarketplaceTerms -Accept`
`Get-AzureRmMarketplaceTerms -Publisher "barracudanetworks" -Product "waf" -Name "hourly" | Set-AzureRmMarketplaceTerms -Accept`

'az vm image terms accept --urn barracudanetworks:waf:byol:*'

## Deployment

The package provides a deploy.ps1 and deploy.sh for Powershell or Azure CLI based deployments. This can be peformed from the Azure Portal as well as the any system that has either of these scripting infrastructures installed. Or you can deploy from the Azure Portal using the provided link.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fbarracudanetworks%2Fwaf-azure-templates%2Fmaster%2FARMTemplates%2Fcontrib%2FCustom-WAF-HA-AS-1NIC-ELB%2Fazuredeploy.json" target="_blank"><img src="http://azuredeploy.net/deploybutton.png"/></a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Fbarracudanetworks%2Fwaf-azure-templates%2Fmaster%2FARMTemplates%2Fcontrib%2FCustom-WAF-HA-AS-1NIC-ELB%2Fazuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

## Deployed resources
Following resources will be created by the template:
- One Azure VNET with 2 subnets (1 for the WAF and a second for the web server)
- One external Basic Azure Load Balancer containing the deployed virtual machines with a public IP and services for HTTP and HTTPS
- Two Barracuda Web Application Firewall virtual machines
- Both WAF systems are deployed in an Availability Set



##Next Steps
After succesfull deployment you should be able to access the WAF via it's management GUI http://<LBPublicIP>:8001 and http://<LBPublicIP>:8002
