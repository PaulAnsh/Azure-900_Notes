# Azure-900_Notes
Repo- Documenting my azure-900 notes. 

## Exam content:
     Cloud Concepts: 15-25%
     Azure Core Services: 30-35%
     Secuirty, Privacy, Compliance and Trust: 25-30%
     Pricing and support: 20-25%
     
     passing grade: 700/1000
     duration: 60 minutes

## Intro
  
Azure: It is a private and public platform used to build, deploy and manage applications.

Azure uses virtualization. Virtualization seprates the tight coupling betwee computer cpu and its operating system, using abstraction layer called Hypervisor. Hypervisor emulates all the functions of CPU and a real computer in a virtual machine. 

## Basics of how Azure works: 
  img: 
  
  
  
## Share Responsiblity Model: 
 img: 
 
 
 
 ## Cloud Models:
  
  It is deployment type of cloud resources:
   1. Private Cloud
   2. Public Cloud
   3. Hybrid Cloud
   
   
   Private Cloud: It is a cloud that is used by single entity. Finally, a procate clpud may be hosted from your dedicated datacenter offsite. Potenitally even by a        third partty that has dedicated that datacenter to your company. 
   
   Public Cloud: A public cloud is built, controlled, and maintained by a third-party cloud-provider. With public cloud, anyone that wants to purchase cloud services can access and use resources. 
   
   Hybrid Cloud: A htbrid cloud is a computing environment that uses both public and private cloud in an inter-connected environment. A hybrid cloud environment can be used to allow a private cloud to surge for increased, temporary demand by deploying public cloud resources. 
   
   Multi-Cloud: Using multiple cloud providers and dealing two or more public cloud providers and manage resources. 
   
   Azure Arc: It is a set of technology that helps manage your cloud environment. It helps with cloud environment, whether it's a public cloud solely on Azure, a private cloud in your datacenter, a hybrid config, or even a multi-cloud environment running on multiple cloud providers at once. 
   

## The Consumption-based model

   There are two types of expenses consider. Capital Expenditure (CapEx) and operational expediture (opEX). 
   
   CapEx:
   1. one time, up-front expenditure to secure resources. 
   2. eg: Building, Company vehicles, Building datacenter. 
   
   OpEx:
   1. Spending money on services or on products over time. 
   2. Renting convention center, leasing a company vehicle or siging cloud services. 
   
   Cloud computing falls under OpEX because cloud computing operates on a consumption-based model, with cloud computing, you don't pay for physical infrastructure, the electricity, the security, or anything else associated with maintaing a datacenter. 
   
 ## Benefits for consumption-based model
 
 1. No upfront costs.
 2. No need to purchase and manage costly infrastructre that users might not use. 
 3. The ability to pay for more resources when needed. 
 
 ## Cloud Benefits
     
 1. High Availabilty
 2. Fault Tolerance
 3. Scalabilty
 4. Global reach
 5. Agility
 6. Elasticity
 7. Customer latency capabilites
 8. Predictive Cost Consideration. 
 
 ## Core Azure Services: 
 
 Region Pairs: Region pair is used to replicate data in two regions. eg: us west and us east. 
 
Azure compute: Azure compute is a service which provides on-demand computing services for cloud based applications. Such as: Computing resources, for instance, processors, memory, storage, os, networking. Listed below are the services provided with Azure Compute Services.
Azure App Service
Azure Virtual Machines
Azure Container Instances
Azure Functions (or serverless computing)

1. Azure App service: Azure app service is used for deploying enterprise applications for web and mobile. It is easily scaled with complaint requirements, secuirty and performance assured that is managed by azure platform. It falls under Paas. 

  
  
## High Avalability:
      
   Your ability for your service to remain available by ensuring there is no single poiunt of failure. 
      
   Azure Load Balancer: allow you to evenly distribute traffic to multiple servers in datacenters. If a datacenter is down, LB will route traffic to only availble        datacenter with servers.
      
## High Scalabilty:
     
   Your ability to increase capacity based on the increasing demand of traffic, memory and computing power. 
     
## High Elasticity:
     
   Your ability to automatically increase or decrease capacity based on the current demand of traffic, memory and computing power. 
     
     scaling out- Add more servers of same size
     scaling in - Remove more servers of same size. 
     
## High Durability:
      
   Your ability ti recover from a disaster and to prevent the loss of data solutions that recover from a disater is know as Disaster recovery(DR). 

## Regions and Geo:
     
   A region is a group of mulitple datacenter(AZ). Azure has 58 regions across 140 countries. 
   A Geo is discreet market of two or more regions that preserves data residency and compliance boundries.
     
   Paired region: 
   Each reggion is paired with another region 300 miles away. (Only one region is updated at a time to ensure no outage)
     
   Azure Geo-redundant storage(GRS)- It replicates data to a secondary region automatically, ensuring that data is durable even in the event that primary region is        not recoverable. 
  
## Fault and Update Domain
     
   An AZ in an Azure region is a combination of a fault domain and update domain. 
     
   Fault domain: It is a logical grouping of hardware in server racks, to avoid a single point of failure within an AZ. It is a group of vm that share common power        source and network switch. 
   
   Update Domain: When azure applies updates to the underlying hardware and software, update domains ensures your resources do not go offline. 
   
   Avalability sets: A logical grouping that you can use in azure to ensure that vm's you place in the avalabiliy set are in different fault/update domains to avoid      downtime. 
   
## Computing Services:

   Azure Service Fabric: Tier-1 enterprise contianers as a service. Distributed systens platformsm runs in azure or on-premises. easy to package, deploy, and manage                            scalable and reliable microservices. 
   
  Azure Functions: Event-drive, serverless computre functions run code without provisioning ot managing servers. You pay only for the compute time you consume. 
     
   Azure Batch: Plans, schedules and executes your batch computer workloads across running 100+ jobs in parallel. Use spot vm's to save money (previously used low-                     priority vm's to save on compute). 
     
     
## Storage Services: 

   Azure blob storage: Object server less storage. Store very large files and large amount of unstructred files. Pay for what you store, unlimtied storage, no-            resiszing vol, file system protocols.      
   
   Azure Disk storage: A virtual volume, choose SSD or HDD, encryption by default, attach volume to vm's. 
   
   Azure file storage: A shared volume that you can access and manage like a file server. eg: SMB.
   
   Azure Queue Storage: Message queue a data store for queueing and reliable delivery messgae between application. 
   
   Azure Table storage: Wide-column NO SQL Database. A NOSQL store that hosts unstructred data independent of any schema. 
   
   Azure Data Box: Briefcase computer and storage designed, which is used to store and move terabytes or petabytes of data 
   
   Azure Archieve storage: A storage at cheap prize, which is used to storae data for longer period of time. 
   
   Azure data lake storage: A storage which is used to store unstructred or strucurted data at any scale in a centralized repo.
   
## Database services:

   Azure Cosmos DB: A fully managed NOSQL database, designed to be scale at 99.999% avalabilty. 
   
   Azure SQL database: Fully managed SQL database with auto scale, integral intelligence, and robust security.
   
   Azure database for MYSQL/PSQL/MariaDB: Fully managed and scalable with HA and secuity. 
   
   SQL server on VMs: Used to shift SQL server form on-premises to cloud. 
   
   Azure Synapse anlaytics: Fully managed data warehouse with integral security at every level of scale at no extra cost. 
   
   Azure Database Migration services: Migrate your database to cloud with no code changes to application.
   
   Azure cache for redis: Caches frequently used to reduce data and application latency.
   
   Azure table storage: No SQL database that hosts unstructured data independent of any schema. 
   
   
## Application Integration services:

   Services which are designed to help apps or services to talk to each other.
   
   Azure notification hub: Pub/Sub send push notifiacation to any platform from any back end. 
   
   Azure API: API gateway, quickly build and consume API's in the cloud. 
   
   Azure Service bus: It is a reliable cloud messaging as a service (MAAS) abd sumply hybrid integration. 
   
   Azure Stream Analytics: Serverless real-time analytics, from the cloud to the edge. 
   
   Azure Logic apps: It is used to schdule, automate and orchestrate tasks, business processes and workflows. 
   
   Azure API management: Hybrid, multi-cloud management platform for API'S across all enviroments. Put in front of existing API's to add additional functionality. 
   
   Azure Queue Storage: Messaging queue. A data store for queuing and reliably delivering message b/w applications. 
   

## Developer and mobile tools: 
     
   Azure SignalR service: Real time messaging easily add real-time web functionality to applications. 
   
   Azure app service: Easy to use service for developing and scaling web-applications with .net, Node.JS, Java, Python, and PHP. Developer focus on building web-apps,    and not worry about underline infrastructre. 
   
   Xamarin: Mobile app framework. Create powerful and scalable native mobile apps with .NET and Azure. 

## Azure Virtual network (Vnet):

- It is private network. In this we address the ip address, subnets, and the region we want it in.
 - IP addresses : we mention IP address in VNet so that it can assign the network form the pool we just selected.
- Subnet: We mention subnet because we need to group the resources who constantly work with each other and put them in one subnet. After doing that we can add security, default route for the subnets to work together      if we need them to.
- It also create a default route to allow the subnet to connect with the internet
  - We can also create a custom route if don’t want to use default route and wants to add the firewall with special security and instructions.
 - In default: Outbound traffic is allowed to the internet, but not all inbound traffic is allowed.
- If a resource need a inbound access to vnet, then you need assign a public IP address to allow that.
  - Need a name resolution service to translate between names and IP addresses.
- If you need resources in a VNET to communicate with each other using names : **Azure-provided name resolution (Automatically present when we create a VNET)**
- If you need to resolve the names of systems in another virtual network: **Azure DNS private zones (Only for private networks)**
- If the resources in VNet need to resolve the names of systems in an on-premises environment: **(Your own DNS server or Azure DNS)**
  
![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/627425ef-141a-4d9d-b66c-5e504c236399/Untitled.png)

**Connecting to other networks:**

VNET peering: You could set up an internet connection between the two, but a much faster and more secure way to do it is to use VNet peering. You just need to configure one peering connection in each direction between the two VNets, and then resources will be able to communicate with each other as if they’re on the same network.

- If the two VNet are in different region then we can use the **Global Vnet peering**

**To connect VNet with on-premises:** 

- Azure VPN : Need to deploy azure VPN gateway in virtual network to encrypt the VPN and allow the data to transfer. Need to install vpn device(Site-to-site(Local network gateway)) at the on-premises location as well to get the data.
    - If you want to connect individual devices, such as mobile phones, to your virtual network, then you can set up point-to-site connections. This method works differently from the site-to-site method because there’s no VPN device on the user’s side. Instead, you have to install a certificate on each mobile device. The certificate is used to authenticate with the Azure VPN Gateway. In most cases, you can use the same VPN Gateway for both site-to-site and point-to-site connections. In fact, you can only have one VPN Gateway in each VNet, so you have to use the same one. The only situation where you can’t support both site-to-site and point-to-site connections from the same gateway is when you need to configure a different type of routing for each.
- **Azure express route: I**f you don’t want your connection to go over the internet or you need more bandwidth, then you can set up a direct connection using Azure ExpressRoute. Be aware that this is a much more expensive solution, though.

# Private endpoints:

- Some Azure resources, such as Azure SQL Database instances and Azure Storage containers, can’t be put in a virtual network directly, but there is an indirect way to bring them into a VNet. The solution is called a private endpoint. It’s simply a private IP address in a virtual network that’s connected to an Azure resource that’s outside of the VNet.
- I should mention that not all Azure resources can be connected to a private endpoint. A resource has to be hosted by a service that supports something called Private Link. This is what’s actually used to connect your private endpoint to the service.

# **Azure storage:**

- It is scalable
- Durable
- Managed service
- Accessible over web.
- Encrypted
- It has 4 categories: Blob, Files, Queues, Tables.

- **Blob:** Binary large object, in order to store files in blob, we have to make a container( container here  is not the application one, we have to use container(folder) to put files into it.) They are not organized. If you just need a place to put files, whether they’re documents or videos or logs or anything else, then you should use Blob storage, which is by far the **cheapest** of all the storage types.
    - There are three access tiers in blob storage:
    1. Hot: For frequent accessed data
    2. Cool: For infrequent access of data
        
        Lower storage cost but higher cost for read and writes. Data must be in cool tier for at least 30 days
        
    3. Archive: For rarely accessed data. May take up to 15 hours to access data. 5x cheaper than cool tier for storage but much more expensive for reads. Data needs to be there for at least 180 days. 
- We can move data with blob tiers anytime we want. But if we move data before the data we will be charged early deletion fees.
- **File storage:** It has the sort of hierarchical structure you’d expect in a filesystem**.** In fact, it’s SMB-compliant, so you can use it as a Windows file share. This makes it easy to move an on-premises file server to Azure. Even better, you can make this file share globally accessible over the web, if you want. To do that, users need a shared access signature token, which allows access to particular data for a specific amount of time. It is **expensive** then blob.
- **Queue storage:** Queue storage is a very different option. It’s intended for passing messages between applications. One application pushes messages onto the queue and another application asynchronously retrieves those messages from the queue, one at a time, and processes them.
- **Table storage:** I find Table storage to be the most surprising type of Azure Storage. It’s a NoSQL datastore with storage costs that are about the same as File storage and with way cheaper transaction costs. I think Microsoft realized what a good deal this is too, because they now have a premium version of Table storage that’s part of their Cosmos DB service.
- **Disk storage:** I should also mention that there’s another type of Azure Storage. It’s what’s used for the disks that are attached to virtual machines. But these disks are created when you create a VM, so you don’t need to create them yourself in Azure Storage. That’s why you’ll only see options for blobs, files, queues, and tables in your storage accounts.

**Locally-redundant storage (or LRS) is replicated across racks in the same data center. This means that if there’s a disaster at that data center, your data could be lost. Although this is highly unlikely, you should only use locally-redundant storage if you can easily reconstruct your data.**

**Zone-redundant storage (or ZRS) is replicated across three zones within one region, so if an entire zone goes down, your data will still be available.**

**Geo-redundant storage (or GRS) is replicated across two regions, so even if an entire region goes down, your data will still be available. However, in the event of a regional disaster, you’d have to perform a geo-failover before you could access your data in the secondary region.**

[Data redundancy - Azure Storage](https://learn.microsoft.com/en-us/azure/storage/common/storage-redundancy)

**If you need to upload lots of files, then it would be faster to use AZ Copy, which is a command-line utility that runs on Windows, macOS, and Linux. It lets you copy files and folders to or from a storage account, and it even lets you copy them between Azure and other cloud providers, such as AWS.**

**If you’re migrating from an on-premises environment to Azure, then you should consider using Azure Migrate and Azure Data Box. Azure Migrate does a lot more than copy data. First, it discovers your on-premises servers, web apps, and databases. Then it assesses them, telling you the size and cost of the equivalent Azure services. Finally, it helps you do the migration.**

**If you need to send a large amount of data during the migration, the solution is to use Azure Data Box. Here’s how it works. Microsoft ships a Data Box storage device to your datacenter. Then you copy your data to the device and ship it back to Microsoft. When they receive it, Microsoft will transfer the data from the device to your Azure storage account. You can also use Data Box to do the reverse, that is, export your data from Azure to your datacenter if you need to at some point in the future. Due to the time and expense involved with Azure Data Box, you would typically use it only if you need to transfer more than 40 terabytes of data.**

## Azure Active Directory:

Identity and access management system. It allows to create user accounts for on-prem.

In cloud: AD is used access cloud applications and resources. 

if you already have an on-premises Active Directory implementation, you don’t have to recreate all of your users and groups in Azure Active Directory. Instead, you can synchronize your accounts between the two systems using **Azure AD Connect.** This’ll create the accounts on Azure for you and keep them in sync when changes are made to the accounts in Active Directory. It will allow you to use single sign-on (or SSO), which means that users only need to log in once to access both their on-premises environment and their Azure environment. You can also use SSO to access Microsoft 365.

## **RBAC (Role-Based Access Control):**

 ****

Azure Active Directory can authenticate users, meaning it identifies who they are, but it doesn’t know what they should be allowed to do in Azure. In other words, it doesn’t handle **authorization. That’s managed by a separate system called role-based access control (or RBAC).**

## ****Zero Trust and Defense in Depth on Azure:****

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/cd9ad056-9b1d-42d1-a65a-75a7624eed7c/Untitled.png)

## **Managing the cost:**

**TCOC(Total cost of ownership calculator):** The Azure Total Cost of Ownership(***TCO***) Calculator is used to estimate the cost savings you can achieve by migrating your application workloads to Microsoft Azure. 

**Subscription and cost:** Before you can use Azure, you need to have a subscription. It’s used by Microsoft for billing purposes. Whenever you create a resource in Azure, it will be assigned to a subscription, so Microsoft will know how to bill for that resource. It’s possible to have multiple subscriptions, but each Azure resource can only be assigned to one subscription.

Additional:

- You can not put a resource group in more than one resource group.
- you can move a resource from one resource group to another. also can move resource form one sub to another.
- Resources don’t need to be in the same region as the resource group they’re in.
- When you delete a resource group, all of the resources in it get deleted, too. This is a very useful way of making sure you delete all of the resources related to a particular application or project.
- Azure provides three types of platform logs that can help with troubleshooting and auditing. Resource logs (formerly known as diagnostic logs) contain information about things that happened within an Azure resource, such as accessing a database. Activity logs contain information at the subscription level about activities that were performed on a resource from the outside, such as shutting down a database instance. Azure Active Directory logs contain information about activities specifically related to Azure Active Directory, such as recent logins and new users added.
- When a user accidentally modifies or deletes a resource, such as a virtual machine, it can have catastrophic consequences, so Microsoft provides a handy way to prevent this from happening. An administrator can apply a resource lock to important resources.
- There are two types of locks: Delete and Read-only. A Delete lock, of course, prevents a resource from being deleted. A read-only lock prevents a resource from being deleted or modified, so it’s more restrictive than a Delete lock. If two different administrators add locks to the same resource, then the most restrictive lock is applied. Even an administrator can’t delete a locked resource, so they have to delete the lock (or locks) before they can delete the resource.
- **If you want to apply a lock to all of the resources in a resource group, you only have to apply the lock to the resource group itself, and all of the resources in it will inherit the lock. You can even do this at the subscription level for all resources in a subscription.**
- To enforce a wide variety of governance policies, you can use the Azure Policy service. For example, suppose your company has a European division that is legally required to store its data only in European data centers. You could create a policy that only allows SQL Database instances to be created in European regions and assign that policy to the resource group for that division of the company. You’d also need to create similar policies for other data storage services, such as SQL Data Warehouse and Data Lake Storage.
- Now suppose you need to assign the same policies to a number of different resource groups or subscriptions. To make it easier, you can group related policies into what’s called an initiative and then assign that initiative to various subscriptions, resource groups, and management groups.
- Speaking of management groups, what are they? If your organization has a lot of subscriptions, you’ll likely want to apply the same policies or policy initiatives to many of them. This would normally require applying them to each subscription individually, but there’s an easier way. You can put your subscriptions in management groups. Then when you apply a policy or a role assignment to a management group, it will be inherited by all of the subscriptions in that management group.
- the Service Trust Portal is focused specifically on compliance. For example, it has links to Azure audit reports for regulatory standards like SOC, FedRAMP, and ISO27001. These will be helpful if your organization is going through these compliance audits. There’s also a link to a site called “Compliance Manager”. This is a great tool that helps you achieve compliance. It creates assessments for different Microsoft services. It shows how compliant your organization is and how compliant Microsoft is for a particular area.
   
   
   
     
     
