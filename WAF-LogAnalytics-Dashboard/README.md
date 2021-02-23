# Microsoft Log Analytics and Sentinel

### Introduction

Using the Barracuda Web Application Firewall’s Azure Resource Manager (ARM) templates you can create and configure a Log Analytics workspace with views or Workbooks.

To send the log data to the OMS workspace, you must add the Microsoft Azure OMS server details in the Barracuda Web Application Firewall web interface.

### How to deploy

You can copy and paste the raw json into the Azure portal to deploy a custom template or you can deploy from the Azure Portal using the provided link.

#### Deploy Log Analytics Workspace + Dashboards
<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fbarracudanetworks%2Fwaf-azure-templates%2Fmaster%2FWAF-LogAnalytics-Dashboard%2Fazuredeploy.json" target="_blank"><img src="http://azuredeploy.net/deploybutton.png"/></a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Fbarracudanetworks%2Fwaf-azure-templates%2Fmaster%2FWAF-LogAnalytics-Dashboard%2Fazuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

#### Deploy Log Analytics  Dashboards
<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fbarracudanetworks%2Fwaf-azure-templates%2Fmaster%2FWAF-LogAnalytics-Dashboard%2Fazuredeploy_existing_workspace.json" target="_blank"><img src="http://azuredeploy.net/deploybutton.png"/></a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Fbarracudanetworks%2Fwaf-azure-templates%2Fmaster%2FWAF-LogAnalytics-Dashboard%2Fazuredeploy_existing_workspace.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

### Templates available

azuredeploy.json - If you don't have OMS or wish to create a new OMS instance then use this to create the workspace and dashboard
azuredeploy_existing_workspace.json - If you already have OMS and wish to add a WAF Dashboard use this template
/workbooks/workbook.json - If you just want to deploy a workbook into something existing.


##### DISCLAIMER: ALL OF THE SOURCE CODE ON THIS REPOSITORY IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL BARRACUDA BE LIABLE FOR ANY CLAIM, DAMAGES, OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOURCE CODE. #####

