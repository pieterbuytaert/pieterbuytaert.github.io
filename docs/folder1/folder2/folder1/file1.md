
# Cloud Custodian service introduction 


Arxus uses the customer Azure Monitor and log analytics workspace to monitor resource diagnostic logs. An Arxus alert definition set is deployed to the workspace, monitoring Cloud Custodian enabled resources and notifying the Arxus Service Desk for high priority events. 
## Cloud Custodian Standard
The Cloud Custodian Standard service offering is enabled per supported resource, activating the Standard monitoring set for this resource. Additional included services or actions included with this service for a specific resource can be found in the Cloud Custodian Service Details section. 
## Cloud Custodian Extended 
The Cloud Custodian Standard service offering is enabled per supported resource, activating the Extended monitoring set for this resource on top of the standard set. Additional included services or actions included with this service for a specific resource can be found in the Cloud Custodian Service Details section. 

## Actions 
| Description | Action Type | Arxus | Customer |
|---|---|---|---|
|**<span style= "font-size:1.3em">Setup</span>** ||||
| Deploy Cloud Custodian Lighthouse offering from Azure Marketplace | Change  | CI  | RA  |
| Configure central Log Analytics workspace per subscription | Change  | RA  | CI  |
| Activation of Arxus Cloud Custodian Standard services on supported resources | Change  | R  | ACI  |
| Activation of Arxus Cloud Custodian Extended services on supported resources | Change  | R  | ACI  |
| Configure diagnostic settings to gather logs in customer log analytics workspace | Change  | RA  | CI  |
| Configure diagnostic settings to gather logs in customer log analytics workspace | Change  | RA  | CI  |
| Deploy Arxus monitor and alert definitions to log analytics workspace | Change  | RA  | CI  |
|**<span style= "font-size:1.3em">Monitoring actions</span>** ||||
| Alert on high priority health events | Included  | RA  | CI  |
| Alert on high priority Performance events | Included  | RA  | CI  |
| Creation of incident-ticket on high priority alert | Included  | RA  | CI  |


# Service Activities per Resource Type
| Description | Action Type | Arxus | Customer |
|---|---|---|---|
|**<span style= "font-size:1.3em">API Management service (microsoft.apimanagement/service) </span>** ||||
|_**Standard**_ ||||
| Alert on high priority API health events | Included  | RA  | CI  |
| Alert on high priority API Performance events | Included  | RA  | CI  |
| Creation of incident-ticket on high priority alert | Included  | RA  | CI  |
| Create, configure and publish API products  | Ready  | CI  | RA  |
| Deploy API Management resource | Ready  | RA  | CI  |
| Deploy network infrastructure hosting API Management | Ready  | RA  | CI  |
| Activate Arxus Cloud Custodian Standard | Change  | RA  | CI  |
| Arxus proposed modification for improvement of the API Management Resource Change | Change  | RA  | CI  |
| Configure API Management  | Change  | RA  | CI  |
| Create API Management Resource | Change  | RA  | CI  |
| Delete API Management Resource | Change  | RA  | CI  |
| On request modification of the API Management Resource | Change  | R  | ACI  |
| Troubleshoot backend application errors | Incident  | CI  | RA  |
| Troubleshoot backend server errors | Incident  | RA  | CI  |
| Troubleshoot Health Events | Incident  | RA  | CI  |
| Troubleshoot Performance Events | Incident  | RA  | CI  |
|**<span style= "font-size:1.3em">Azure Cache for Redis (microsoft.cache/redis) </span>** ||||
|_**Standard**_ ||||
| Creation of incident-ticket on high priority alert | Included  | RA  | CI  |
| Activate Arxus Cloud Custodian Standard | Change  | RA  | CI  |
| Arxus proposed modification for improvement of the Azure Cache for Redis Change | Change  | RA  | CI  |
| Configure Data Persistence for a premium Azure Cache for Redis | Change  | R  | ACI  |
| Configure firewall rules for Azure Cache for Redis | Change  | R  | ACI  |
| Configure Redis Clustering for a premium Azure Cache for Redis | Change  | R  | ACI  |
| Configure virtual network support for a Premium-tier Azure Cache for Redis instance | Change  | R  | ACI  |
| Configure zone redundancy and geo-replication for Azure Cahce for Redis resource | Change  | R  | ACI  |
| Create Azure Cache for Redis resource | Change  | RA  | CI  |
| Delete Azure Cache for Redis resource | Change  | RA  | CI  |
| On request modification of the Azure Cache for Redis resource | Change  | R  | ACI  |
| Setup replicas to standard/premium Azure Cache for Redis | Change  | R  | ACI  |
| Update Azure Cache for Redis resource to a different size and tier | Change  | R  | ACI  |
| Alert on high priority health events | Incident  | RA  | CI  |
| Alert on high priority Performance events | Incident  | RA  | CI  |
| Troubleshoot Azure Cache for Redis application errors | Incident  | CI  | RA  |
| Troubleshoot Health Events | Incident  | RA  | CI  |
| Troubleshoot Performance Events | Incident  | RA  | CI  |
|**<span style= "font-size:1.3em">Kubernetes service (microsoft.containerservice/managedclusters) </span>** ||||
|_**Standard**_ ||||
| Alert On High Priority Cluster Health Events | Included  | RA  | CI  |
| Alert On High Priority Node Health Events | Included  | RA  | CI  |
| Alert On High Priority Node Performance Health Events | Included  | RA  | CI  |
| Node OS / Kernel Update Management | Included  | RA  | CI  |
| Deploy a container architecture for Kubernetes. | Ready  | CI  | RA  |
| Deploy a Kubernetes Cluster. | Ready  | RA  | CI  |
| Deploy a network architecture for hosting Kubernetes. | Ready  | RA  | CI  |
| Resize Cluster Node SKU | Change  | RA  | CI  |
| AKS Cluster and worker nodes troubleshooting | Incident  | RA  | CI  |
| troubleshoot Node Health Events | Incident  | RA  | CI  |
| troubleshoot Node Performance Events | Incident  | RA  | CI  |
| AKS pods, containers, and controllers troubleshooting |   | CI  | RA  |
| Alert On High Priority Pod Performance Events |   | CI  | RA  |
| Build, automate, update and deploy container images, with or without a CI/CD pipeline |   | CI  | RA  |
| Kubernetes Update Managment |   | CI  | RA  |
|_**Extended**_ ||||
| Alert On High Priority Pod Performance Events | Included  | RA  | CI  |
| Custom Alerts on Prometheus Events | Included  | R  | ACI  |
| Kubernetes Update Management | Included  | RA  | CI  |
| Install and configure Prometheus pod monitoring | Ready  | R  | ACI  |
| Optimize forwarded Prometheus logs to Azure Log Analytics Workspace | Ready  | RA  | CI  |
|**<span style= "font-size:1.3em">Azure Database for PostgreSQL server (microsoft.dbforpostgresql/servers) </span>** ||||
|_**Standard**_ ||||
| Creation of incident-ticket on high priority alert | Included  | RA  | CI  |
| Deploy PostgreSQL Resource | Ready  | RA  | CI  |
| Activate Arxus Cloud Custodian Standard | Change  | RA  | CI  |
| Arxus proposed modification for improvement of the PostgreSQL Resource Change | Change  | RA  | CI  |
| Configure Backup and Restore support for PostgreSQL resource | Change  | R  | ACI  |
| Configure data-replication for PostgreSQL resource | Change  | R  | ACI  |
| Delete PostgreSQL Resource | Change  | RA  | CI  |
| Grant network access to resource via netwerk and firewall policies | Change  | R  | ACI  |
| Grant user access and rights to the PostgreSQL resource via accounts and roles | Change  | R  | ACI  |
| On request modification of the PostgreSQL Resource | Change  | R  | ACI  |
| Update PostgreSQL resource to a different size and tier | Change  | R  | ACI  |
| Alert on high priority health events | Incident  | RA  | CI  |
| Alert on high priority Performance events | Incident  | RA  | CI  |
| Troubleshoot Health Events | Incident  | RA  | CI  |
| Troubleshoot Performance Events | Incident  | RA  | CI  |
| Troubleshoot PostgreSQL database application errors | Incident  | CI  | RA  |
| Troubleshoot PostgreSQL database server errors | Incident  | RA  | CI  |
| Application performance tuning e.g. queries, indexing |   | CI  | RA  |
|**<span style= "font-size:1.3em">Azure Cosmos DB account (microsoft.documentdb/databaseaccounts) </span>** ||||
|_**Standard**_ ||||
| Alert on high priority disk and request unit performance events | Included  | RA  | CI  |
| Alert on high priority resource health events | Included  | RA  | CI  |
| Creation of incident-ticket on high priority alert | Included  | RA  | CI  |
| Configure Backup and Restore support for Cosmos DB resource | Ready  | R  | ACI  |
| Configure global distribution for Cosmos DB resource | Ready  | R  | ACI  |
| Create Cosmos DB Resource | Ready  | RA  | CI  |
| Configure network access for Cosmos DB resource | Change  | R  | ACI  |
| Delete Cosmos DB Resource | Change  | RA  | CI  |
| Move an Azure Cosmos DB account to another region | Change  | R  | ACI  |
| On request modification of the Cosmos DB Resource | Change  | R  | ACI  |
| Update Cosmos DB resource to a different size and tier | Change  | R  | ACI  |
| Troubleshoot Cosmos DB application errors | Incident  | CI  | RA  |
| Troubleshoot Health Events | Incident  | RA  | CI  |
| Troubleshoot Performance Events | Incident  | RA  | CI  |
|**<span style= "font-size:1.3em">VM Scale Set Autoscale Settings (microsoft.insights/autoscalesettings) </span>** ||||
|_**Standard**_ ||||
| Arxus proposed modification for improvement of the Autoscale Rules | Change  | RA  | CI  |
| Deletion of the Autoscale Rules | Change  | R  | ACI  |
| On request modification of Autoscale Rules | Change  | R  | ACI  |
| Alert on high priority health events | Incident  | RA  | CI  |
| Creation of incident-ticket on high priority alert | Incident  | RA  | CI  |
| Review of failed Autoscale actions | Incident  | RA  | CI  |
|**<span style= "font-size:1.3em">Key vault (microsoft.keyvault/vaults) </span>** ||||
|_**Standard**_ ||||
| Alert on high priority health and key request failure events | Included  | RA  | CI  |
| Alert on high priority Performance (latency and Saturaton) events | Included  | RA  | CI  |
| Creation of incident-ticket on high priority alert | Included  | RA  | CI  |
| Activate Arxus Cloud Custodian Standard | Change  | RA  | CI  |
| Arxus proposed modification for improvement of the Azure Key Vault Resource Change | Change  | RA  | CI  |
| Create Azure Key Vault Resource | Change  | RA  | CI  |
| Delete Azure Key Vault Resource | Change  | RA  | CI  |
| On request modification of the Azure Key Vault Resource | Change  | R  | ACI  |
| Troubleshoot Health Events | Incident  | RA  | CI  |
| Troubleshoot Performance (Latency, Saturation) Events | Incident  | RA  | CI  |
|**<span style= "font-size:1.3em">Front Door (microsoft.network/frontdoors) </span>** ||||
|_**Standard**_ ||||
| Monitor health events | Included  | RA  | CI  |
| Monitor performance events | Included  | RA  | CI  |
| deploy Frontdoor resource | Ready  | RA  | CI  |
| Arxus proposed modification for improvement | Change  | RA  | CI  |
| Delete resource | Change  | RA  | CI  |
| Modifications to the resource | Change  | R  | ACI  |
| Troubleshoot application unavailability | Incident  | CI  | RA  |
| Troubleshoot Health events | Incident  | RA  | CI  |
| Troubleshoot Health probe events | Incident  | CI  | RA  |
| Troubleshoot HTTP Errors | Incident  | CI  | RA  |
|**<span style= "font-size:1.3em">Load balancer (microsoft.network/loadbalancers) </span>** ||||
|_**Standard**_ ||||
| Alert on no healthy probes | Included  | RA  | CI  |
| Alert on some unhealthy probes | Included  | RA  | CI  |
| Create Load Balancer resource | Ready  | RA  | CI  |
| Arxus proposed modification for improvement | Change  | RA  | CI  |
| Delete resource | Change  | RA  | CI  |
| Modifications to the resource | Change  | R  | ACI  |
| Troubleshoot application unavailability | Incident  | CI  | RA  |
| Troubleshoot Health events | Incident  | RA  | CI  |
| Troubleshoot Health probe events | Incident  | CI  | RA  |
|**<span style= "font-size:1.3em">Service Bus Namespace (microsoft.servicebus/namespaces) </span>** ||||
|_**Standard**_ ||||
| Alert on high priority health events | Included  | RA  | CI  |
| Creation of incident-ticket on high priority alert | Included  | RA  | CI  |
| Custom activated: Alert on high priority deadletter events | Included  | R  | ACI  |
| Activate ServiceBus Namespace deadletter monitoring if requested | Ready  | R  | ACI  |
| Activate ServiceBus Namespace deadletter monitoring: Provide procedure for deadletter troubleshooting | Ready  | CI  | RA  |
| Create ServiceBus Namespaces Resource | Ready  | R  | ACI  |
| Activate Arxus Cloud Custodian Standard | Change  | RA  | CI  |
| Arxus proposed modification for improvement of the Service Bus Resource Change | Change  | RA  | CI  |
| Delete Service Bus Resource | Change  | R  | ACI  |
| On request modification of the Service Bus Resource | Change  | R  | ACI  |
| Troubleshoot deadletter events according to procedure | Incident  | R  | ACI  |
| Troubleshoot health events | Incident  | RA  | CI  |
|**<span style= "font-size:1.3em">SQL database (microsoft.sql/servers/databases) </span>** ||||
|_**Standard**_ ||||
| Alert on high priority health events | Included  | RA  | CI  |
| Alert on high priority Performance events | Included  | RA  | CI  |
| Creation of incident-ticket on high priority alert | Included  | RA  | CI  |
| Configure private endpoints Azure SQL database resource | Ready  | R  | ACI  |
| Deploy Azure SQL database resource | Ready  | R  | ACI  |
| Setup geo-replication for Azure SQL database | Ready  | R  | ACI  |
| Activate Arxus Cloud Custodian Standard | Change  | R  | ACI  |
| Configure Backup and Restore support for Azure SQL database | Change  | R  | ACI  |
| Delete Azure SQL Database Resource | Change  | RA  | CI  |
| Grant network access to resource via firewall policies | Change  | R  | ACI  |
| Granting user access and rights to the resource via accounts and roles | Change  | R  | ACI  |
| On request modification of the Azure SQL Database Resource | Change  | R  | ACI  |
| Update Azure SQL Database to a different size and tier | Change  | R  | ACI  |
| Troubleshoot database application/query errors | Incident  | CI  | RA  |
| Troubleshoot database server errors | Incident  | RA  | CI  |
| Troubleshoot Health Events | Incident  | RA  | CI  |
| Troubleshoot Performance Events | Incident  | RA  | CI  |
| Application performance tuning e.g. queries, indexing. |   | CI  | RA  |
|**<span style= "font-size:1.3em">Storage account (microsoft.storage/storageaccounts) </span>** ||||
|_**Standard**_ ||||
| Alert on availability issue | Included  | RA  | CI  |
| deploy Storage Account Resource | Ready  | RA  | CI  |
| Activate Arxus Cloud Custodian Standard | Change  | RA  | CI  |
| Arxus proposed modification for improvement of the Storage Account Resource Change | Change  | RA  | CI  |
| Delete Storage Account Resource | Change  | RA  | CI  |
| On request modification of the Storage Account Resource | Change  | R  | ACI  |
| Troubleshoot Health and availability Events | Incident  | RA  | CI  |