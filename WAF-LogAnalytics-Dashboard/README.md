# Microsoft Operational Management Suite

### Introduction

Using the Barracuda Web Application Firewall’s Azure Resource Manager (ARM) template you can create and configure a Log Analytics workspace in the Microsoft’s OMS. To send the log data to the OMS workspace, you must add the Microsoft Azure OMS server details in the Barracuda Web Application Firewall web interface.

### How to deploy
Refer to "Deploying the ARM Template" and "Configure the Barracuda Web Application Firewall to Integrate with the OMS Server and Export Logs" articles in Barracuda Campus.

### Templates available

createomsdashboard.json - If you already have OMS and wish to add a WAF Dashboard use this template
createomsworkspace_updated_apr_23_2018.json - If you don't have OMS or wish to create a new OMS instance then use this to create the workspace and dashboard


##### DISCLAIMER: ALL OF THE SOURCE CODE ON THIS REPOSITORY IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL BARRACUDA BE LIABLE FOR ANY CLAIM, DAMAGES, OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOURCE CODE. #####

