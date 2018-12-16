## Azure

[What are the benefits of severless applications?](#what-are-the-benefits-of-severless-applications)

[What is Azure Cloud Service?](#what-is-azure-cloud-service)

[What is a web role?](#what-is-a-web-role)

[What is Azure Functions?](#what-is-azure-functions)

[What is serverless computing?](#what-is-serverless-computing)

[What is Azure Resource Group?](#what-is-azure-resource-group)

[What is Kudu?](#what-is-kudu)

[What is a role instance?](#what-is-a-role-instance)

[What is a guest operating system?](#what-is-a-guest-operating-system)

[What is Azure Blob Storage?](#what-is-azure-blob-storage)

[How to include external dll into Azure Function?](#how-to-include-external-dll-into-azure-function)

[Is Azure Table Storage Nosql?](#is-azure-table-storage-nosql)

[What is an Azure subscription?](#what-is-an-azure-subscription)

[What is Azure ARM?](#what-is-azure-arm)

[Explain the Azure ARM Templates](#explain-the-azure-arm-templates)

[What is a cloud service role?](#what-is-a-cloud-service-role)

[What is Azure Redis Cache?](#what-is-azure-redis-cache)

[What is Azure Service Fabric?](#what-is-azure-service-fabric)

[How can I use applications with Azure AD that I’m using on-premises?](#how-can-i-use-applications-with-azure-ad-that-im-using-on-premises)

[What Is Azure Key Vault?](#what-is-azure-key-vault)

[What is a Blob Container?](#what-is-a-blob-container)

[How can you stop a VM using Power Shell?](#how-can-you-stop-a-vm-using-power-shell)

[How can you retrieve the state of a particular VM?](#how-can-you-retrieve-the-state-of-a-particular-vm)

[How can one create a VM in Azure CLI?](#how-can-one-create-a-vm-in-azure-cli)

[What do you know about Azure WebJobs?](#what-do-you-know-about-azure-webjobs)

[What is a worker role?](#what-is-a-worker-role)

[How can one create a Virtual Machine in Powershell?](#how-can-one-create-a-virtual-machine-in-powershell)

[How much storage can I use with a virtual machine?](#how-much-storage-can-i-use-with-a-virtual-machine)

[Is it possible to add an existing VM to an availability set?](#is-it-possible-to-add-an-existing-vm-to-an-availability-set)

[What is deployment environments?](#what-is-deployment-environments)

[What is Azure VPN?](#what-is-azure-vpn)

[What is the difference between Service Bus Queues and Storage Queues?](#what-is-the-difference-between-service-bus-queues-and-storage-queues)

[What are the differences between Subscription Administrator and Directory Administrator?](#what-are-the-differences-between-subscription-administrator-and-directory-administrator)

[What is a VNet?](#what-is-a-vnet)

[What are stateful and stateless microservices for Service Fabric?](#what-are-stateful-and-stateless-microservices-for-service-fabric)

[What is key vault in Azure?](#what-is-key-vault-in-azure)

[Do scale sets work with Azure availability sets?](#do-scale-sets-work-with-azure-availability-sets)

[What are Network Security Groups?](#what-are-network-security-groups)

[What are Update Domains?](#what-are-update-domains)

[What are Fault Domains?](#what-are-fault-domains)

[What is an Availability Set?](#what-is-an-availability-set)

[What are virtual machine scale sets in Azure?](#what-are-virtual-machine-scale-sets-in-azure)

[What is Azure MFA?](#what-is-azure-mfa)

[What are Cloud Service Roles and why do we use them?](#what-are-cloud-service-roles-and-why-do-we-use-them)

[What is Azure Table Storage?](#what-is-azure-table-storage)

[What is Azure Resource Manager and why we need to use one?](#what-is-azure-resource-manager-and-why-we-need-to-use-one)

[What is Azure Search?](#what-is-azure-search)

[What are Redis databases?](#what-are-redis-databases)

[Is it possible to create a Virtual Machine using Azure Resource Manager in a Virtual Network that was created using classic deployment?](#is-it-possible-to-create-a-virtual-machine-using-azure-resource-manager-in-a-virtual-network-that-was-created-using-classic-deployment)

[How to create a new storage account and container using Power Shell?](#how-to-create-a-new-storage-account-and-container-using-power-shell)

[ What is the meaning of application partitions?](#-what-is-the-meaning-of-application-partitions)

[What is Azure VNET?](#what-is-azure-vnet)

[What is the difference between “price,” “software price,” and “total price” in the cost structure for Virtual Machine offers in the Azure Marketplace?](#what-is-the-difference-between-price-software-price-and-total-price-in-the-cost-structure-for-virtual-machine-offers-in-the-azure-marketplace)

[How to create a Network Security Group and a Network Security Group Rule?](#how-to-create-a-network-security-group-and-a-network-security-group-rule)

[How are Azure Marketplace subscriptions priced?](#how-are-azure-marketplace-subscriptions-priced)

[Explain Azure NSG](#explain-azure-nsg)

[What VPN types are supported by Azure?](#what-vpn-types-are-supported-by-azure)

[What are special Azure Regions?](#what-are-special-azure-regions)


### What are the benefits of severless applications?

* Avoid managing servers
* Flexible scaling by demand
* Pay for time and resources it takes to execute your code



[[↑] Back to top](#Azure)
### What is Azure Cloud Service?

By creating a cloud service, you can deploy a multi-tier web application in Azure, defining multiple roles to distribute processing and allow flexible scaling of your application. A cloud service consists of one or more web roles and/or worker roles, each with its own application files and configuration. Azure Websites and Virtual Machines also enable web applications on Azure. The main advantage of cloud services is the ability to support more complex multi-tier architectures

###### Source

* https://mindmajix.com/azure-interview-questions

[[↑] Back to top](#Azure)
### What is a web role?

A web role provides a dedicated Internet Information Services (IIS) web-server used for hosting front-end web applications.

###### Source

* https://mindmajix.com/azure-interview-questions

[[↑] Back to top](#Azure)
### What is Azure Functions?

Azure Functions is a solution for easily running small pieces of code, or "functions," in the cloud. We can write just the code we need for the problem at hand, without worrying about a whole application or the infrastructure to run it and use language of our choice such as C#, F#, Node.js, Java, or PHP. Azure Functions lets us develop serverless applications on Microsoft Azure.



[[↑] Back to top](#Azure)
### What is serverless computing?

Serverless computing is the abstraction of servers, infrastructure, and operating systems. When you build serverless apps you don’t need to provision and manage any servers, so you can take your mind off infrastructure concerns. Serverless computing is driven by the reaction to events and triggers happening in near-real-time—in the cloud. 

As a fully managed service, server management and capacity planning are invisible to the developer and billing is based just on resources consumed or the actual time your code is running.



[[↑] Back to top](#Azure)
### What is Azure Resource Group?

Resource groups (RG) in Azure is an approach to group a collection of assets in logical groups for easy or even automatic provisioning, monitoring, and access control, and for more effective management of their costs. The underlying technology that powers resource groups is the Azure Resource Manager (ARM).

###### Source

* http://www.onlinetech.com/resources/references/how-to-use-azure-resource-groups-a-simple-explanation

[[↑] Back to top](#Azure)
### What is Kudu?

Every Azure App Service web application includes a "hidden" service site called **Kudu**.

Kudu Console for example is a debugging service for Azure platform which allows you to explore your web app and surf the bugs present on it, like deployment logs, memory dump, and uploading files to your web app, and adding JSON endpoints to your web apps, etc.




[[↑] Back to top](#Azure)
### What is a role instance?

A role instance is a virtual machine on which the application code and role configuration run. A role can have multiple instances, defined in the service configuration file.

###### Source

* https://mindmajix.com/azure-interview-questions

[[↑] Back to top](#Azure)
### What is a guest operating system?

The guest operating system for a cloud service is the operating system installed on the role instances (virtual machines) on which your application code runs.

###### Source

* https://mindmajix.com/azure-interview-questions

[[↑] Back to top](#Azure)
### What is Azure Blob Storage?

*Azure Blob storage* is Microsoft's object storage solution for the cloud. Blob storage is optimized for storing massive amounts of unstructured data, such as text or binary data. Azure Storage offers three types of blobs:
* **Block blobs** store text and binary data, up to about 4.7 TB. Block blobs are made up of blocks of data that can be managed individually.
* **Append blobs** are made up of blocks like block blobs, but are optimized for append operations. Append blobs are ideal for scenarios such as logging data from virtual machines.
* **Page blobs** store random access files up to 8 TB in size. Page blobs store the VHD files that back VMs.


###### Source

* https://docs.microsoft.com/en-us/azure/storage/blobs/storage-blobs-introduction

[[↑] Back to top](#Azure)
### How to include external dll into Azure Function?

* Add the assembly to the BIN directory using KUDU
* Include the assembly and code the Azure Function to use it
* Add the using declaration so that the methods within the DLL can be accessed. 

```cs
#r "D:\home\site\wwwroot\GreetingsAssemblyReference\bin\benjamin.dll"

using benjamin;
```



[[↑] Back to top](#Azure)
### Is Azure Table Storage Nosql?

**Azure Table storage** is a service that stores structured NoSQL data in the cloud, providing a key/attribute store with a schemaless design.

###### Source

* https://docs.microsoft.com/en-us/azure/vpn-gateway/vpn-gateway-vpn-faq

[[↑] Back to top](#Azure)
### What is an Azure subscription?

A Windows **Azure subscription** grants you access to Windows Azure services and to the Windows Azure Platform Management Portal. A Windows Azure subscription has two aspects: 
* The Windows Azure account, through which resource usage is reported
* Services are billed.

###### Source

* https://blogs.msdn.microsoft.com/arunrakwal/2012/04/09/create-windows-azure-subscription/

[[↑] Back to top](#Azure)
### What is Azure ARM?

The **Azure Resource Manager (ARM)** is the service used to provision resources in your Azure subscription. It was first announced at Build 2014 when the new Azure portal ( portal.azure.com) was announced and provides a new set of API's that are used to provision resources. The ARM is:

* Template-driven – Using templates to deploy all resources.
* Declarative – You declare the resources you want to have instead of imperative where you need to make rules.
* Idempotent – You can deploy the template over and over again without affecting the current state of resources.
* Multi-service – All services can be deployed using Azure Resource Manager, Website, Storage, VMs etc.
* Multi region - You can choose in which region you would like to deploy the resources.
* Extensible – Azure Resource Manager is extensible with more resource providers and thus resources.


###### Source

* https://azurestack.blog/2015/06/azure-resource-manager-templates-json/

[[↑] Back to top](#Azure)
### Explain the Azure ARM Templates

An Azure Resource Template is a JSON file used to deploy resources with Azure Resource Manager. It defines:
* Parameters
* Variables
* Resources - the actual resources that you are going to deploy or update
* Outputs

###### Source

* http://www.onlinetech.com/resources/references/how-to-use-azure-resource-groups-a-simple-explanation

[[↑] Back to top](#Azure)
### What is a cloud service role?

A cloud service role is comprised of application files and a configuration. A cloud service can have two types of roles:
* web role
* worker role

###### Source

* https://mindmajix.com/azure-interview-questions

[[↑] Back to top](#Azure)
### What is Azure Redis Cache?

*Redis* is an open source (BSD licensed), in-memory data structure store, used as a database, cache and message broker. **Azure Redis Cache** is based on the popular open-source Redis cache. It gives you access to a secure, dedicated Redis cache, managed by Microsoft, and accessible from any application within Azure. It supports data structures such as strings, hashes, lists, sets, sorted sets with range queries, bitmaps, hyperloglogs and geospatial indexes with radius queries.

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### What is Azure Service Fabric?

**Azure Service Fabric** is a distributed systems platform that makes it easy to package, deploy, and manage scalable and reliable micro-services. Service Fabric also addresses the significant challenges in developing and managing cloud applications. Developers and administrators can avoid complex infrastructure problems and focus on implementing mission-critical, demanding workloads that are scalable, reliable, and manageable. Service Fabric represents the next-generation middleware platform for building and managing these enterprise-class, tier-1, cloud-scale applications.

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### How can I use applications with Azure AD that I’m using on-premises?

*Azure AD* gives you an easy and secure way to connect to the web applications you choose. You can access these applications in the same way you access your SaaS apps in Azure AD, no need for a VPN to change your network infrastructure.

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### What Is Azure Key Vault?

**Key Vault** help you safeguard cryptographic keys and other secrets used by your applications whenever they are On-Premise or in the cloud. More and more services on Azure are now integrating Azure Key Vault as their secret/key source for things like deployments, data or even disk encryption.

###### Source

* https://www.codeisahighway.com/create-an-azure-key-vault-using-an-arm-template-api-version-2015-06-01-and-azure-powershell-v1-0-4/

[[↑] Back to top](#Azure)
### What is a Blob Container?

A container organizes a set of blobs, similar to a folder in a file system. All blobs reside within a container. A storage account can contain an unlimited number of containers, and a container can store an unlimited number of blobs.

###### Source

* https://docs.microsoft.com/en-us/azure/storage/blobs/storage-blobs-introduction

[[↑] Back to top](#Azure)
### How can you stop a VM using Power Shell?

```sh
Stop-AzureRmVM -ResourceGroupName myResourceGroupVM -Name "myVM" -Force
```

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### How can you retrieve the state of a particular VM?

```sh
Get-AzureRmVM `
 -ResourceGroupName myResourceGroup `
 -Name myVM `
 -Status | Select @{n="Status"; e={$_.Statuses[1].Code}}
```

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### How can one create a VM in Azure CLI?

```sh
az vm create ` --resource-group myResourceGroup ` --name myVM --image win2016datacenter ` --admin-username azureuser ` --admin-password myPassword12
```

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### What do you know about Azure WebJobs?

**WebJobs** is a feature of Azure App Service that enables you to run a program or script in the same context as a web app, API app, or mobile app. There is no additional cost to use WebJobs.

The Azure WebJobs SDK is a framework that simplifies the task of writing background processing code that runs in Azure WebJobs. It includes a declarative binding and trigger system that works with Azure Storage Blobs, Queues and Tables as well as Service Bus. You could also trigger Azure WebJob using Kudu API.

###### Source

* https://github.com/Azure/azure-webjobs-sdk/wiki

[[↑] Back to top](#Azure)
### What is a worker role?

Applications hosted within worker roles can run asynchronous, long-running or perpetual tasks independent of user interaction or input.

###### Source

* https://mindmajix.com/azure-interview-questions

[[↑] Back to top](#Azure)
### How can one create a Virtual Machine in Powershell?

```sh
# Define a credential object 
$cred = Get-Credential 
# Create a virtual machine configuration 
$vmConfig = New-AzureRmVMConfig -VMName myVM -VMSize Standard_DS2 |
` Set-AzureRmVMOperatingSystem -Windows -ComputerName myVM -Credential $cred | 
` Set-AzureRmVMSourceImage -PublisherName MicrosoftWindowsServer -Offer WindowsServer ` 
-Skus 2016-Datacenter -Version latest | Add-AzureRmVMNetworkInterface -Id $nic.Id
```

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### How much storage can I use with a virtual machine?

Each data disk can be up to 1 TB. The number of data disks which you can use depends on the size of the virtual machine.

Azure Managed Disks are the new and recommended disk storage offerings for use with Azure Virtual Machines for persistent storage of data. You can use multiple Managed Disks with each Virtual Machine. Managed Disks offer two types of durable storage options: Premium and Standard Managed Disks.

Azure storage accounts can also provide storage for the operating system disk and any data disks. Each disk is a .vhd file stored as a page blob.

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### Is it possible to add an existing VM to an availability set?

No. If you want your VM to be part of an availability set, you need to create the VM within the set. There currently no way to add a VM to an availability set after it has been created.

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### What is deployment environments?

Azure offers two deployment environments for cloud services: 
* a staging environment in which you can test your deployment before you promote it to 
* the production environment. 

The two environments are distinguished only by the virtual IP addresses (VIPs) by which the cloud service is accessed. In the staging environment, the cloud service’s globally unique identifier (GUID) identifies it in URLs (GUID.cloudapp.net). 

In the production environment, the URL is based on the friendlier DNS prefix assigned to the cloud service (for example, myservice.cloudapp.net).

###### Source

* https://mindmajix.com/azure-interview-questions

[[↑] Back to top](#Azure)
### What is Azure VPN?

A **VPN** gateway is a specific type of virtual network gateway that is used to send encrypted traffic between an Azure virtual network and an on-premises location over the public Internet. You can also use a VPN gateway to send encrypted traffic between Azure virtual networks over the Microsoft network.

###### Source

* https://docs.microsoft.com/en-us/azure/vpn-gateway/vpn-gateway-about-vpngateways

[[↑] Back to top](#Azure)
### What is the difference between Service Bus Queues and Storage Queues?

The *Azure Storage Queue* is simple and the developer experience is quite good. It uses the local Azure Storage Emulator and debugging is made quite easy. The tooling for Azure Storage Queues allows you to easily peek at the top 32 messages and if the messages are in XML or Json, you’re able to visualize their contents directly from Visual Studio Furthermore, these queues can be purged of their contents, which is especially useful during development and QA efforts.

The Azure Service Bus Queues are evolved and surrounded by many useful mechanisms that make it enterprise worthy! They are built into the Service Bus and are able to forward messages to other Queues and Topics. They have a built-in dead-letter queue and messages have a time to live that you control, hence messages don’t automatically disappear after 7 days.

Furthermore, Azure Service Bus Queues have the ability of deleting themselves after a configurable amount of idle time. This feature is very practical when you create Queues for each user, because if a user hasn’t interacted with a Queue for the past month, it automatically gets clean it up. Its also a great way to drive costs down. You shouldn’t have to pay for storage that you don’t need. These Queues are limited to a maximum of 80gb. Once you’ve reached this limit your application will start receiving exceptions.

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### What are the differences between Subscription Administrator and Directory Administrator?

By default, one is assigned the *Subscription Administrator* role when he/she signs up for Azure. A subscription admin can use either a Microsoft account or a work or school account from the directory that the Azure subscription is associated with. This role is authorized to manage services in the Azure portal. If others need to sign in and access services by using the same subscription, you can add them as co-admins.

Azure AD has a different set of admin roles to manage the directory and identity-related features. These admins will have access to various features in the Azure portal or the Azure classic portal. The admin’s role determines what they can do, like create or edit users, assign administrative roles to others, reset user passwords, manage user licenses, or manage domains.

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### What is a VNet?

VNet is a representation of your own network in the cloud. It logically isolates your instances launched in the cloud, from the rest of your resources.

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### What are stateful and stateless microservices for Service Fabric?

*Service Fabric* enables you to build applications that consist of microservices: 

* Stateless microservices (such as protocol gateways and web proxies) do not maintain a mutable state outside a request and its response from the service. Azure Cloud Services worker roles are an example of a stateless service. 

* Stateful microservices (such as user accounts, databases, devices, shopping carts, and queues) maintain a mutable, authoritative state beyond the request and its response.

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### What is key vault in Azure?

Microsoft **Azure Key Vault** is a cloud-hosted management service that allows users to encrypt keys and small secrets by using keys that are protected by hardware security modules (HSMs). Small secrets are data less than 10 KB like passwords and .PFX files.

###### Source

* https://searchwindowsserver.techtarget.com/definition/Microsoft-Azure-Key-Vault

[[↑] Back to top](#Azure)
### Do scale sets work with Azure availability sets?

Yes. A scale set is an implicit availability set with 5 fault domains and 5 update domains. Scale sets of more than 100 VMs span multiple placement groups, which are equivalent to multiple availability sets. An availability set of VMs can exist in the same virtual network as a scale set of VMs. A common configuration is to put control node VMs (which often require unique configuration) in an availability set and put data nodes in the scale set.

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### What are Network Security Groups?

A *network security group (NSG)* contains a list of Access Control List (ACL) rules that allow or deny network traffic to subnets, NICs, or both. NSGs can be associated with either subnets or individual NICs connected to a subnet. When an NSG is associated with a subnet, the ACL rules apply to all the VMs in that subnet. In addition, traffic to an individual NIC can be restricted by associating an NSG directly to a NIC.

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### What are Update Domains?

An *update domain* is a logical group of underlying hardware that can undergo maintenance or can be rebooted at the same time. As you create VMs within an availability set, the Azure platform automatically distributes your VMs across these update domains. This approach ensures that at least one instance of your application always remains running as the Azure platform undergoes periodic maintenance. The order of update domains being rebooted may not proceed sequentially during planned maintenance, but only one update domain is rebooted at a time.

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### What are Fault Domains?

A *fault domain* is a logical group of underlying hardware that share a common power source and network switch, similar to a rack within an on-premise data-centers. As you create VMs within an availability set, the Azure platform automatically distributes your VMs across these fault domains. This approach limits the impact of potential physical hardware failures, network outages, or power interruptions.

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### What is an Availability Set?

*An availability set* is a logical grouping of VMs that allows Azure to understand how your application is built to provide redundancy and availability. It is recommended that two or more VMs are created within an availability set to provide for a highly available application and to meet the 99.95% Azure SLA. When a single VM is used with Azure Premium Storage, the Azure SLA applies for unplanned maintenance events.

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### What are virtual machine scale sets in Azure?

Virtual machine scale sets are Azure compute resource that you can use to deploy and manage a set of identical VMs. With all the VMs configured the same, scale sets are designed to support true autoscale, and no pre-provisioning of VMs is required. So it’s easier to build large-scale services that target big compute, big data, and containerized workloads.

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### What is Azure MFA?

**Azure Multi-Factor Authentication (MFA)** is Microsoft's two-step verification solution. It delivers strong authentication via a range of verification methods, including phone call, text message, or mobile app verification.

###### Source

* https://docs.microsoft.com/en-us/azure/active-directory/authentication/multi-factor-authentication

[[↑] Back to top](#Azure)
### What are Cloud Service Roles and why do we use them?

In Azure, a *Cloud Service Role* is a collection of managed, load-balanced, Platform-as-a-Service virtual machines that work together to perform common tasks. Cloud Service Roles are managed by Azure fabric controller and provide the ultimate combination of scalability, control, and customizationThere are three types of roles in Microsoft Azure:

* **Web Role** – A web role is basically used to deploy a website, using languages supported by the IIS platform like, PHP, .NET etc. It is configured and customized to run web applications.
* **Worker Role** – A worker role is more like an help to the Web role, it used to execute background processes unlike the Web Role which is used to deploy the website.
* **VM Role** – The VM role is used by a user to schedule tasks and other windows services. This role can be used to customize the machines on which the web and worker role is running.

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### What is Azure Table Storage?

*Azure Table storage* is a service that stores structured NoSQL data in the cloud, providing a key/attribute store with a schemaless design. Because Table storage is schemaless, it's easy to adapt your data as the needs of your application evolve. Access to Table storage data is fast and cost-effective for many types of applications, and is typically lower in cost than traditional SQL for similar volumes of data.

###### Source

* https://docs.microsoft.com/en-us/azure/cosmos-db/table-storage-overview

[[↑] Back to top](#Azure)
### What is Azure Resource Manager and why we need to use one?

The **Azure Resource Manager (ARM)** is the service used to provision resources in your Azure subscription. ARM provides us a way to describe resources in a resource group using JSON documents (ARM Template). by using the ARM Template you have a fully repeatable configuration of a given deployment and this is extremely valuable for Production environments but especially so for Dev/Test deployments. By having a set template, we can ensure that anytime a new Dev or Test deployment is required (which happens all the time), it can be achieved in moments and safe in the knowledge that it will be identical to the previous environments.

###### Source

* https://www.codeisahighway.com/create-an-azure-key-vault-using-an-arm-template-api-version-2015-06-01-and-azure-powershell-v1-0-4/

[[↑] Back to top](#Azure)
### What is Azure Search?

*Azure Search* is a cloud search-as-a-service solution that delegates server and infrastructure management to Microsoft, leaving you with a ready-to-use service that you can populate with your data and then use to add search to your web or mobile application. 

Azure Search allows you to easily add a robust search experience to your applications using a simple REST API or .NET SDK without managing search infrastructure or becoming an expert in search.

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### What are Redis databases?

Redis Databases are just a logical separation of data within the same Redis instance. The cache memory is shared between all the databases and actual memory consumption of a given database depends on the keys/values stored in that database. For example, a C6 cache has 53 GB of memory. You can choose to put all 53 GB into one database or you can split it up between multiple databases.

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### Is it possible to create a Virtual Machine using Azure Resource Manager in a Virtual Network that was created using classic deployment?

This is not supported. You cannot use Azure Resource Manager to deploy a virtual machine into a virtual network that was created using classic deployment.

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### How to create a new storage account and container using Power Shell?


```sh
$storageName = "st" + (Get-Random)
New-AzureRmStorageAccount -ResourceGroupName "myResourceGroup" -AccountName $storageName -Location "West US" -SkuName "Standard_LRS" -Kind Storage
$accountKey = (Get-AzureRmStorageAccountKey -ResourceGroupName myResourceGroup -Name $storageName).Value[0]
$context = New-AzureStorageContext -StorageAccountName $storageName -StorageAccountKey $accountKey 
New-AzureStorageContainer -Name "templates" -Context $context -Permission Container
```

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
###  What is the meaning of application partitions?

*The application partitions* are a part of the Active Directory system and having said so, they are directory partitions which are replicated to domain controllers. Usually, domain controllers that are included in the process of directory partitions hold a replica of that directory partition. The attributes and values of application partitions is that you can replicated them to any specific domain controller in a forest, meaning that it could lessen replication traffic. 

While the domain directory partitions transfer all their data to all of the domains, the application partitions can focus on only one in the domain area. This makes application partitions redundant and more available.

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### What is Azure VNET?

An **Azure Virtual Network (VNet)** is a representation of your own network in the cloud. It is a logical isolation of the Azure cloud dedicated to your subscription.

###### Source

* https://docs.microsoft.com/en-us/azure/virtual-network/virtual-networks-faq

[[↑] Back to top](#Azure)
### What is the difference between “price,” “software price,” and “total price” in the cost structure for Virtual Machine offers in the Azure Marketplace?

* **Price** - refers to the cost of the Azure Virtual Machine to run the software. 
* **Software price** - refers to the cost of the publisher software running on an Azure Virtual Machine. 
* **Total price** - refers to the combined total cost of the Azure Virtual Machine and the publisher software running on an Azure Virtual Machine.

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### How to create a Network Security Group and a Network Security Group Rule?


```sh
# Create an inbound network security group rule for port 3389
$nsgRuleRDP = New-AzureRmNetworkSecurityRuleConfig -Name myNetworkSecurityGroupRuleRDP -Protocol Tcp
 -Direction Inbound -Priority 1000 -SourceAddressPrefix * -SourcePortRange * -DestinationAddressPrefix *
 -DestinationPortRange 3389 -Access Allow
 
# Create an inbound network security group rule for port 80
$nsgRuleWeb = New-AzureRmNetworkSecurityRuleConfig -Name myNetworkSecurityGroupRuleWWW -Protocol Tcp
 -Direction Inbound -Priority 1001 -SourceAddressPrefix * -SourcePortRange * -DestinationAddressPrefix *
 -DestinationPortRange 80 -Access Allow
 
# Create a network security group
$nsg = New-AzureRmNetworkSecurityGroup -ResourceGroupName myResourceGroup -Location EastUS
 -Name myNetworkSecurityGroup -SecurityRules $nsgRuleRDP,$nsgRuleWeb
```

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### How are Azure Marketplace subscriptions priced?

Pricing will vary based on product types. ISV software charges and Azure infrastructure costs are charged separately through your Azure subscription. Pricing models include:

* **BYOL Model**: Bring-your-own-license. You obtain outside of the Azure Marketplace, the right to access or use the offering and are not charged Azure Marketplace fees for use of the offering in the Azure Marketplace.

* **Free**: Free SKU. Customers are not charged Azure Marketplace fees for use of the offering.

* **Free Software Trial**: Full-featured version of the offer that is promotionally free for a limited period of time. You will not be charged Azure Marketplace fees for use of the offering during a trial period. Upon expiration of the trial period, customers will automatically be charged based on standard rates for use of the offering.

* **Usage-Based**: You are charged or billed based on the extent of your use of the offering. For Virtual Machines Images, you are charged an hourly Azure Marketplace fee. For Data Services, Developer services, and APIs, you are charged per unit of measurement as defined by the offering.

* **Monthly Fee**: You are charged or billed a fixed monthly fee for a subscription to the offering (from the date of subscription start for that particular plan). The monthly fee is not prorated for mid-month cancellations or unused services.

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
### Explain Azure NSG

A **network security group (NSG)** used to filter network traffic to and from Azure resources in an Azure virtual network and  includes rules that allow or deny traffic to a virtual network subnet, network interface, or both.

###### Source

* https://docs.microsoft.com/en-us/azure/vpn-gateway/vpn-gateway-about-vpngateways

[[↑] Back to top](#Azure)
### What VPN types are supported by Azure?

Azure supports two types of Point-to-site VPN options:

* Secure Socket Tunneling Protocol (SSTP). SSTP is a Microsoft proprietary SSL-based solution that can penetrate firewalls since most firewalls open the TCP port that 443 SSL uses.
* IKEv2 VPN.

###### Source

* https://docs.microsoft.com/en-us/azure/vpn-gateway/vpn-gateway-vpn-faq

[[↑] Back to top](#Azure)
### What are special Azure Regions?

Azure has some special regions that you may wish to use when building your applications for compliance or legal purposes. These special regions include:

* **US Gov Virginia** and **US Gov Iowa** - A physical and logical network-isolated instance of Azure for US government agencies and partners, operated by screened US persons. Includes additional compliance certifications such as FedRAMP and DISA.
* **China East** and **China North** - These regions are available through a unique partnership between Microsoft and 21Vianet, whereby Microsoft does not directly maintain the datacenters.
* **Germany Central** and **Germany Northeast** - These regions are available via a data trustee model whereby customer data remains in Germany under control of T-Systems, a Deutsche Telekom company, acting as the German data trustee.

###### Source

* https://www.quora.com/What-are-the-common-questions-asked-in-Microsoft-Azure-interview

[[↑] Back to top](#Azure)
