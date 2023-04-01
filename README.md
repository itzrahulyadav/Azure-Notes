<h1 align="center"> Azure-Notes <img src = "https://user-images.githubusercontent.com/65400893/218178929-58b12284-b0f2-4c98-af2a-a1f897d93cd6.svg" widht = "50px" height= "50px" margin-top = "5px"/></h1>

<p align="center">Notes to prepare for Azure certification exams</p>



# Azure fundamentals 

### Cloud computing

Cloud computing is defined as the on-demand delivery of IT resources like networking,compute,storage over the internet with pay as you
go pricing.


In simple terms cloud is a computer that is located somewhere else which can be accessed via the internet.

<br>
### Types of cloud service offerings

- IaaS(Infrastructure as a Service) --- In this offering CSP(cloud service providers) provide building blocks like networking,storage and compute.CSP manages all the physical infrastructure like staff,hardware and datacenter.For example AWS ec2,Azure VM,GCP compute engine etc.
- PaaS(Platform as a Service) --- Customer is responsible for deployment and management of the apps .CSP manages the servers,hardware and OS.For example Azure app service.
- SaaS(Software as a Service) --- Customer just configures the features.CSP is responsible for management and service availability.For example MS office 354,salesforce etc.


<br>
### Cloud deployment model:

-  Public Cloud -- When everything runs on your cloud provider's datacenter.
-  Private Cloud -- When the company uses its own datacenter and everything is owned and managed by the company itself.
-  Hybrid Cloud -- It is the combination of public and private cloud.Companies use some servers in their own data center and some in the 
   private cloud.
   example: A company may run everything on their data center but use cloud providers for their data backup.
 
 <br>
 ### Advantages of cloud computing.
 
 1.  Scalabilty: The ability of a system to handle growth of users or work.
 2.  Elasticity: The ability of a system to automatically grow and shrink based on app demand
 3.  Agility: The ability to react quickly to change in demand,without manual intervention.
 4.  Economies of Scale: The ability to do things more efficiently or at lower-cost per unit when operating at a larger scale
 5.  Capital Expenditure(CapEx): The money spent on physical infrasturcture up front.
 6.  Operational Expenditure(OpEx): It means spending money on services and being billed later.
 7.  Cloud reduces the CapEx expenditure and increases the OpEx.
 8.  (Consumption based model)Pay-as-you-go: You are only charged for what you use and for how long you use it.


### Other benefits of cloud Computing.
-  Fault Tolerance:Failure of components.
-  High Availability: The ability to keep services up and running for long periods of time.
-  Disaster Reconvery: The ability to recover from an event which has taken down a cloud service.For example: Data center failure .We can Azure use site recovery to bring instances quickly.

<br>
### Shared responsibility model

-  On-premesis
      -  It is 100% customers responsibility
      -  Everything is own by the customer and is solely responsible for everything.

- IaaS
    -  Everything upto the virtualization layer is taken care of by the cloud service provider.
    -  Customer is responsible for everything above the virtualization layer like Guest OS,data,application,patching of the OS etc.

- PaaS
   -  Customer is only responsible for only data and applications.
   -  All other things will be the responsibilty of the cloud service provider which is Azure in this case.


- Saas
  -  Customer is only responsible for their data.
  -  Everything is taken care of by CSP.

<br>
### Azure Architecture components

-  Azure Geography
    -  A discrete market,typically containing two or more regions,that preserves data residency and compliance boundaries.
    
-  Azure Regions
    -  A set of data centers connected through low-latency networks.
    
-  Region Pairs
    -  A relationship between two azure regions within the same geographic regions for the purpose of diseaster recovery purpose.
    -  This are chosen by Microsoft,we cannot configure them.
    
-  Availability Zones
    -  Collection of one more data centers
    -  This are independent and have their own power,network and cooling.
    
    
### Other architecuture components

-  Management Groups👇🏻
      -  Subscriptions👇🏻
           -  Resource Groups👇🏻
                 -  Resources
                 
1. Management Groups
This provide the level of scope above subscriptions.It can contain multiple subscriptions.

2. Subscriptions
It is used to isolate resources between departments,projects etc.

3. Resource Groups
Resource Groups are containers that hold related resources together.This are used to group resources that share a common purpose.

4. Resources 
Resources are services/offerings offered by Azure.
example: A virtual machine,virtual network etc.

<br>

##  Azure core Services
                 
### 💻__Compute__
The following are some of the most popular compute services provided by Azure

#### Azure VMs

-  Virtual servers on the cloud.
-  No need to purchase hardware.

#### App Service

-  An HTTP based service for hosting web applications ,REST APIs and mobile back ends.

#### Azure Container Instance (ACI)

-  It is a service used to run docker container on demand in a managed,serverless environment.
-  No orchestration is needed.

#### Azure Kubernetes Services (AKS)

-  A hosted kubernetes service for kubernetes clusture.
-  We need to manage the clusters.
-  It is a free service,we only need to pay for nodes not for masters.

#### Windows Virtual Desktop

-  A desktop and app virtualization service that runs in Microsoft Azure.


### 🌐__Network__

The following are the network services provided by Azure

#### Virtual Network(VNet)
-  Our own logically isolated private network in Azure.
-  It consist of subnets.
-  We can connect this with our own on-premise data center using `Site-to-Site VPN`
-  It allows to enable hybrid model.
-  Resources in different VNets can't connect to each other by default.

#### VPN Gateway

-  It is the core component of hybrid cloud.
-  It is used to send traffic between Azure VNets and on-premises location over the intenet.

#### VNET Peering

-  It is used to connect two or more virtual networks (VNets) in Azure.

#### ExpressRoute

-  Connects our on-premises networks into Azure over a private-connection without using the internet.
-  Traffic does not traverse the internet.
-  more secure

### Database storage

Types of storage in azure

1. Blob storage
2. Disk storage
3. File storage
4. Storage tiers

#### Blob storage

- Storage optimised for storing massive amounts of unstructured data.

#### File storage

- Fully managed file shares in Azure accessible via SMB or NFS

#### Disk storage

- Azure managed disks are block-level storage volumes that are managed by azure and used with azure VMs

#### Storage tiers

- Azure storage hot,cool and archieve access tiers to store blob object data in a cost-effective manner.

- We can use lifecycle management policies to automate tiers

#### Table storage

- A service that stores structured NoSql data in azure,including a schemaless key/attribute store

#### Queue storage

- A service for storing large numbers of messages,accessible from anywhere via authenticated http or https calls.

### Databases

Azure provides with following types of databases:

1. Cosmos DB
2. Mysql
3. PostgreSQL
4. Ms SQL
5. Sql managed instance

#### Cosmos DB

- fully managed noSql database
- features ultra-low response latency,and apis for several popular languages and db platforms
- fast global access and data convergence
- It can work as sql ,mongodb,gremlin,cassandra and spark as well.

#### MS sql

- fully managed paas database engine that handles most management functions such as upgrading,patching,backups and monitoring.

#### PostgreSQL

- a relational database service in the microsoft cloud based on the postgreSQL community edition.

#### MY Sql

- A paas relational database service in the Microsoft cloud based on the MySQL community edition.

#### 








    
