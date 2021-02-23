# Introduction

The Barracuda Web Application Firewall for Azure is a scalable security solution that protects applications from targeted and automated attacks. Customers are able to:

1. Protect web applications from data breaches, defacement, OWASP Top-10 Attacks, application layer DDoS and other attack vectors
2. Receive automatic updates with defenses against new threats and vulnerabilities with real-time protection
3. Use strong authentication and access control capabilities to ensure security and privacy – and restrict access to sensitive applications or data
4. Prevent malicious uploads and leakage of sensitive data with built-in anti-virus scanner and data loss prevention abilities
5. Easily comply with standards like PCI-DSS, NIST SSL/TLS guidelines and regulations such as HIPAA

![alt](https://www.barracuda.com/assets/img/sections/programs/azure/img_app-security_diagram2.png)

## Navigating this Repository
In this repository you will find Azure Resource Manager (ARM) templates to assist you with deploying into Azure public cloud environments.


## Template Status
| Status | Name | In existing VNET | HighAvailability | ELB Basic | ELB Standard | Availabilty Set | Availability Zones | 1 NIC | 2 NIC | IPv6
|---|---|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:
| ![Build Status](https://dev.azure.com/gallen0262/cudasedevops/_apis/build/status/Quickstart-WAF-HA-AS-1NIC-ELB) | [Quickstart-WAF-HA-AS-1NIC-ELB](https://github.com/barracudanetworks/waf-azure-templates/tree/master/Quickstart-WAF-HA-AS-1NIC-ELB) | - | X | x | - | X | X | - | - | -
| ![Build status](https://dev.azure.com/gallen0262/cudasedevops/_apis/build/status/Custom-WAF-HA-AZ-1NIC-ELB-STD) | [Custom-WAF-HA-AZ-1NIC-ELB-STD](https://github.com/barracudanetworks/waf-azure-templates/tree/master/Custom-WAF-HA-AZ-1NIC-ELB-STD) | x | X | - | X | - | X | X | - | -
| ![Build status](https://dev.azure.com/gallen0262/cudasedevops/_apis/build/status/Custom-WAF-HA-AS-1NIC-ELB) | [Custom-WAF-HA-AS-1NIC-ELB](https://github.com/barracudanetworks/waf-azure-templates/tree/master/Custom-WAF-HA-AS-1NIC-ELB) | x | X | x | - | X | - | X | - | -
| ![Build status](https://dev.azure.com/gallen0262/cudasedevops/_apis/build/status/Custom-WAF-HA-AZ-1NIC-ELB-STD) | [Custom-WAF-HA-AZ-1NIC-ELB-STD](https://github.com/barracudanetworks/waf-azure-templates/tree/master/Custom-WAF-HA-AZ-1NIC-ELB-STD) | - | X | - | X | X | X | X | - | -
| | [WAF-LogAnalytics-Dashboard](https://github.com/barracudanetworks/waf-azure-templates/tree/master/WAD-LogAnalytics-Dashboard) | - | - | - |- | - | -| - | - | -

More templates can be found within the Contrib directory.


##### DISCLAIMER: ALL OF THE SOURCE CODE ON THIS REPOSITORY IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL BARRACUDA BE LIABLE FOR ANY CLAIM, DAMAGES, OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOURCE CODE. #####

