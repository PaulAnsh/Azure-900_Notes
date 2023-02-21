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
   
   Azure Stream Analytics:
   
     
   
    
     
   
   
   
     
     
