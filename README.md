# Table of contents
- [Introduction-Google Cloud Fundamentals](#Introduction-Google-Cloud-Fundamentals)
- [Cloud Computing Overview](#Cloud-Computing-Overview)
- [IaaS & PaaS](#IaaS-&-PaaS)
- [The Google Cloud Locations](#Google-Cloud-Locations)
- [Environmental Impact](#Environmental-Impact)
- [Security](#Security)
- [OpenSource Ecosystem](#OpenSource-Ecosystem)
- [Pricing & Billing](#Pricing-&-Billing)
- [RESOURCES AND ACCESS IN CLOUD](#RESOURCES-AND-ACCESS-IN-CLOUD)
- [Google Cloud resource hierarchy](#Google-Cloud-resource-hierarchy)
- [Identity and Access Management (IAM)](#Identity-and-Access-Management-(IAM))
- [Service Accounts](#Service-Accounts)
- [Cloud Identities](#Cloud-Identities)
- [VIRTUAL MACHINES AND NETWORKS IN CLOUD](#VIRTUAL-MACHINES-AND-NETWORKS-IN-CLOUD)
- [Virtual private cloud network](#Virtual-private-cloud-network)
- [Compute Engine](#Compute-Engine)
- [Scaling virtual machines](#Scaling-cirtual-machines)

# Introduction-Google Cloud Fundamentals

### The goal of this course is to provide you with an overview of Google Cloud.

Google Cloud offerings can be broadly categorized as-
#### compute
#### storage
#### big data
#### machine learning 
#### application services for web, mobile, analytics and back-end solutions.

### By the end we should be able to, identify the purpose and value of

Google Cloud products and services,

choose among and use application deployment environments on Google Cloud, like App Engine, Google Kubernetes Engine, and Compute Engine,

choose among and use Google Cloud Storage options like Cloud Storage, Cloud SQL, Cloud Bigtable, and Firestore,

interact with Google Cloud services, and describe ways in which customers have used Google Cloud


# Cloud Computing Overview

The cloud is a hot topic these days, but what exactly is it? The US National Institute of Standards and Technology created the term cloud computing, although there's nothing US specific about it.

Cloud computing is a way of using information technology, IT that has these five equally important traits.

1. customers get computing resources that are on-demand and self-service.
  Through a web interface, users get the processing power, storage, and network they require without the need for human intervention.

2. customers get access to those resources over the Internet from anywhere they have a connection.
 
3. The cloud provider has a big pool of those resources and allocates them to users out of that pool. 
  That allows the provider to buy in bulk and pass the savings onto customers. Customers don't have to know or care about the exact physical location of     those resources.

4. The resources are elastic, which means they're flexible.
   If customers need more resources, they can get more and quickly. If they need less, they can scale back.
   
5. customers pay only for what they use or reserve as they go. If they stop using resources, they stop paying. 

#### The trend toward cloud computing started with the first wave known as co-location. 
Co-location gave users the financial efficiency of renting physical space instead of investing in data center real estate. 

#### Virtualized data centers of today, which are the second wave.
It share similarities with the private data centers and co-location facilities of decades past. 
The components of virtualized data centers match the physical building blocks of hosted computing; servers, CPUs, disks, load balances, and so on. But now they're virtual devices. 

With virtualization, enterprises still maintain the infrastructure which is also remains a user controlled and use a configured environment. 
Several years ago, Google realized that his business couldn't move fast enough within the confines of the virtualization model.

#### Google switched to a container-based architecture.
A fully automated, elastic third wave cloud that consists of a combination of automated services and scalable data. 
Services automatically provision and configured the infrastructure used to run applications.


# IaaS & PaaS

The move to virtualized data centers, introduced customers to two new types of offerings. 
1. Infrastructure as a service commonly referred to as IaaS 
2. platform as a service or PaaS. 
   
## IaaS-
IaaS offerings provide raw compute, storage and network capabilities, organized virtually into resources that are similar to physical data centers.
customers pay for the resources they allocate ahead of time.

## PaaS-
PaaS offerings, in contrast, bind code to libraries that provide access to the infrastructure that the application needs. This allows more resources to be focused on application logic.
customers pay for the resources they actually use.

#### As cloud computing has evolved, the momentum has shifted towards managed infrastructure and managed services.
Leveraging managed resources and services allows companies to concentrate more on their business goals and spend less time and money on creating and maintaining their technical infrastructure.
It allows companies to deliver products and services to their customers more quickly and reliably.

Serverless is yet another step in the evolution of cloud computing. It allows developers to concentrate on their code, rather than on server configuration, by eliminating the need for any infrastructure management.

Serverless technologies offered by google include cloud functions, which manages event driven code as a pay as you go service. 
Cloud Run, which allows customers to deploy their containerized microservices based application, in a fully managed environment.

Software as a service applications, aren't installed on your local computer. Instead, they run in the cloud as a service and are consumed directly over the internet by end users.
Popular google applications such as Gmail, Docs and Drive, that are part of Google Workspace, are all examples of SaaS.


# The Google CLoud Network

Google Cloud runs on Google’s own global network. It’s the largest network of its kind, and Google has invested billions of dollars over many years to build it. 
This network is designed to give customers the highest possible throughput and lowest possible latencies for their applications by leveraging more than 100 content caching nodes worldwide. These are locations where high demand content is cached for quicker access, allowing applications to respond to user requests from the location that will provide the quickest response time. 

Google Cloud’s infrastructure is based in five major geographic locations: North America, South America, Europe, Asia,. and Australia. Having multiple service locations is important because choosing where to locate applications affects qualities like 
availability
durability
latency
The latter of which measures the time a packet of information takes to travel from its source to its destination. 

Each of these locations is divided into several different regions and zones. 

### Regions represent independent geographic areas and are composed of zones. 
For example, London, or europe-west2, is a region that currently comprises three different zones. 

### A zone is an area where Google Cloud resources are deployed. 
For example, if you launch a virtual machine using Compute Engine it will run in the zone that you specify to ensure resource redundancy. 

You can run resources in different regions. This is useful for bringing applications closer to users around the world, and also for protection in case there are issues with an entire region, say, due to a natural disaster. 

Some of Google Cloud’s services support placing resources in what we call a multi-region. For example, Cloud Storage lets you place data within the Europe multi-region. That means it's stored redundantly in at least two geographic locations, separated by at least 160 kilometers within Europe like London and Belgium. 

Google Cloud currently supports 88 zones in 29 regions, although this number is increasing all the time. You can find the most up-to-date numbers at cloud.google.com/about/locations.


# Environmental Impact

The virtual world, which includes Google Cloud's network is built on physical infrastructure. And all those racks of humming servers use huge amounts of energy. 

Altogether, existing data centers use roughly 2% of the world's electricity. With this in mind, Google works to make their data centers run as efficiently as possible. 

Just like our customers, Google is trying to do the right thing for the planet. We understand that Google Cloud customers have environmental goals of their own and running their workloads on Google Cloud can be a part of meeting those goals.

Therefore, it's useful to note that Google's data centers were the first to achieve *ISO 14001* certification, which is a standard that maps out a framework for an organization to enhance its environmental performance through improving resource efficiency and reducing waste. 

As an example of how this is being done here is Google's data center in *Hameenlinna Finland*. This facility is one of the most advanced and efficient data centers in the Google fleet. It's cooling system, which uses seawater from the Bay of Finland, reduces energy use and is the first of its kind anywhere in the world. 

In our founding decade, Google became the first major company to be carbon neutral. In our second decade, we were the first company to achieve 100% renewable energy. By 2030, we aim to be the first major company to operate completely carbon free



# Security

The security infrastructure can be explained in progressive layers, 

1. starting from the physical security of our data centers, continuing on to how the hardware and software that's underlying infrastructure are secured, and finally, describing the technical constraints and processes in place to support operational security. 

### 1.1 We begin with the hardware infrastructure layer, which comprises three key security features. 

1.1.1. The first is hardware design and provenance. Both the server boards and the networking equipment in Google data centers are custom designed by google. Google also designs custom chips, including a hardware security chip that's currently being deployed on both servers and peripherals. 

1.1.2. The next feature is a secure boot stack. Google server machines use a variety of technologies to ensure that they're booting the correct software stack, such as cryptographic signatures over the BIOS, bootloader, kernel, and base operating system image. This layer's final feature is premises security. 

Google designs and builds its own data centers, which incorporate multiple layers of physical security protections. Access to these datacenters is limited to only a very small number of Google employees. 
Google additionally hosts some severs in third party data centers, where we ensure that there are google controlled physical security measures on top of the security layers provided by the data center operator.

### 1.2. Next, is a service deployment layer, where the key feature is encryption of inter-service communication. 
Google's infrastructure provides cryptographic privacy and integrity for remote procedure call RPC data on the network. Google services communicate with each other using RPC calls. 

### 1.3. Then we have the user identity layer. 
Google central identity service, which usually manifest to end users as the Google login page, goes beyond asking for a simple username and password. The service also intelligently challenges uses for addition, information based on risk factors such as whether they've logged in from the same device or a similar location in the past. Users could also employ secondary factors when signing in, including devices based on the universal second factor, U2F open standard. 

### 1.4. On the Storage Services layer, we find the encryption at rest security feature. 
Most applications at Google Access physical storage, in other words, file storage indirectly via Storage Services, And encryption using centrally managed keys is applied layer of these Storage Services. Google also enables hardware encryption support in hard drives and SSDs.

### 1.5.  The next layer up is the Internet communication layer, and this comprises two security features. 
Google services that are being made available on the Internet register themselves with an Infrastructure service called the google front-end, which ensures that all TLS connections or ended using a public-private key pair and an x.50 certificate from a certified authority CA, as well as following best practices such as supporting perfect forward secrecy. 
The GFE additionally applies protections against denial-of-service attacks. Also provided is denial-of-service DoS protection. The sheer scale of its Infrastructure enables google to simply absorb many DoS attacks. Google also has multi-tier, multi-layer DoS protections that further reduce the risk of any DoS impact on a service running behind the GFE.

### 1.6. The final layer is Google's operational security layer, which provides four key features. 

1. First, is intrusion detection. Rules and Machine Intelligence give Google's operational security teams warnings of possible incidence. Google conducts red team exercises to measure and improve the effectiveness of its detection and response mechanisms. 

2. Next is reducing insider risk. Google aggressively limits and actively monitors the activities of employees who have been granted administrative access to the infrastructure. 

3. Then there's employee U2Fuse, to guard against phishing attacks against google employees. Employee accounts require use of U2F compatible security keys. 

4. Finally, there are stringent software development practices. Google employs central source control and requires two-party review of new code. Google also provides developers with libraries that prevent them from introducing certain classes of security bugs. 

 Additionally, Google runs a vulnerability rewards program, where we pay anyone who's able to discover and inform us of bugs in our infrastructure or applications. You can learn more about Google's technical infrastructure security at cloud.google.com/ security/security-design.


# OpenSource Ecosystem

Some organizations are afraid to bring their workloads to the Cloud because they're afraid they'll get locked into a particular vendor. However, if for whatever reason, the customer decides that google is no longer the best provider for their needs, we provide them with the ability to run your applications elsewhere. 

Google publishes key elements of technology using open source licenses to create ecosystems that provide customers with options other than Google. 

For example, TensorFlow, an open source software library for machine learning developed inside Google is at the heart of a strong open source ecosystem. Google provides interoperability at multiple layers of the stack. 
Kubernetes and Google Kubernetes Engine give customers the ability to mix and match microservices running across different Clouds. 

Well, Google Cloud's Operations Suite, let's customers monitor workloads across multiple Cloud providers.


# Pricing & Billing 

Google was the first major cloud provider to deliver per-second billing for its infrastructure as a service compute offering compute engine. In addition, per-second billing is now also offered for users of 

#### Google Kubernetes Engine, our container infrastructure as a service 
#### Dataproc, which is the equivalent of the big data system Hadoop but operating as a service 
#### App Engine flexible environment VMs, a platform as a service. 

Compute Engine offers automatically applied sustained-use discounts which are automatic discounts that you get for running a virtual machine instance for a significant portion of the billing month. Specifically, when you run an instance for more than 25% of a month, Compute Engine automatically gives you a discount for every incremental minute you use for that instance. 

Custom virtual machine types allow Compute Engine virtual machines to be fine tuned with optimal amounts of vCPU and memory for the applications so that you can tailor your pricing for your workloads.

Our online pricing calculator can help estimate your costs. Visit cloud.google.com/products/calculator to try it out.

You can define budgets at the billing account level or at the project level. 
A budget can be a fixed limit or it can be tied to another metric, for example, a percentage of the previous month spent. To be notified when costs approach your budget limit, you can create an alert. For example, with a budget limit of $20,000 and an alert set at 90%, you'll receive a notification alert when your expenses reach $18,000. Alerts are generally set at 50%, 90%, and 100% but can also be customized. 

Reports is a visual tool in the Google Cloud Console that allows you to monitor expenditure based on a project or services.

Finally, Google Cloud also implements quotas which are designed to prevent the over consumption of resources because of an error or a malicious attack protecting both accounts owners and the Google Cloud community as a whole.

### There are two types of quotas
1. rate quotas 
2. allocation quotas

both are applied at the project level. 

1. Rate quotas reset after a specific time. For example, by default, the GKE service implements a quota of 1000 calls to it's API from each Google Cloud project every 100 seconds. After that 100 seconds, the limit is reset. 

2. Allocation quotas govern the number of resources you can have in your projects. For example, by default each Google Cloud project has a quota allowing it no more than five virtual private cloud networks. Although projects all start with the same quotas, you can change some of them by requesting an increase from Google Cloud support.


# RESOURCES AND ACCESS IN CLOUD

# Google Cloud resource hierarchy

Google Cloud’s resource hierarchy contains four levels, and starting from the bottom up they are: 

organization node
   |
folders
   |
projects
   |
resources

At the first level are resources. These represent virtual machines, Cloud Storage buckets, tables in BigQuery, or anything else in Google Cloud. 
Resources are organized into projects, which sit on the second level. 
Projects can be organized into folders, or even subfolders. These sit at the third level. 
And then at the top level is an organization node, which encompasses all the projects, folders, and resources in your organization. 

It’s important to understand this resource hierarchy because it directly relates to how policies are managed and applied when you use Google Cloud. Policies can be defined at the project, folder, and organization node levels. 

Some Google Cloud services allow policies to be applied to individual resources, too. Policies are also inherited downward. This means that if you apply a policy to a folder, it will also apply to all of the projects within that folder. 

Projects are the basis for enabling and using Google Cloud services, like managing APIs, enabling billing, adding and removing collaborators, and enabling other Google services. Each project is a separate entity under the organization node, and each resource belongs to exactly one project. 
Projects can have different owners and users because they’re billed and managed separately. 

Each Google Cloud project has three identifying attributes: 
a project ID
a project name
a project number

### Project ID 
It is a globally unique identifier assigned by Google that can’t be changed after creation. They’re what we refer to as being immutable. Project IDs are used in different contexts to inform Google Cloud of the exact project to work with. 

### Project Names
These are user-created. They don’t have to be unique and they can be changed at any time, so they are not immutable. 

### Project Number
Google Cloud also assigns each project a unique project number. It’s helpful to know that these Google-generated numbers exist.They’re mainly used internally by Google Cloud to keep track of resources. 

Google Cloud’s Resource Manager tool is designed to programmatically help you manage projects. It’s an API that can gather a list of all the projects associated with an account, create new projects, update existing projects, and delete projects. It can even recover projects that were previously deleted,and can be accessed through the RPC API and the REST API. 

### The third level of the Google Cloud resource hierarchy is folders. 
Folders let you assign policies to resources at a level of granularity you choose. The resources in a folder inherit policies and permissions assigned to that folder. A folder can contain projects, other folders, or a combination of both. You can use folders to group projects under an organization in a hierarchy. 
For example, your organization might contain multiple departments, each with its own set Google Cloud resources. Folders allow you to group these resources on a per-department basis. Folders also give teams the ability to delegate administrative rights so that they can work independently. As previously mentioned, the resources in a folder inherit policies and permissions from that folder. For example, if you have two different projects that are administered by the same team, you can put policies into a common folder so they have the same permissions. Doing it the other way--putting duplicate copies of those policies on both projects–could be tedious and error-prone.
If you needed to change permissions on both resources, you would now have to do that in two places instead of just one. 

### To use folders, you must have an organization node.
which is the very topmost resource in the Google Cloud hierarchy. Everything else attached to that account goes under this node, which includes folders, projects, and other resources. There are some special roles associated with this top-level organization node. For example, you can designate an organization policy administrator so that only people with privilege can change policies. You can also assign a project creator role, which is a great way to control who can create projects and, therefore, who can spend money. 

How a new organization node is created depends on whether your company is also a Google Workspace customer. If you have a Workspace domain, Google Cloud projects will automatically belong to your organization node. Otherwise, you can use Cloud Identity, Google’s identity, access, application, and endpoint management platform, to generate one. Once created, a new organization node will let anyone in the domain create projects and billing accounts, just as they could before. folders underneath it and put projects into it. Both folders and projects are considered to be “children” of the organization node.


# Identity and Access Management (IAM)

When an organization node contains lots of folders, projects, and resources, a workforce might need to restrict who has access to what. To help with this task, administrators can use Identity and Access Management, or IAM.

### With IAM
The administrators can apply policies that define who can do what on which resources. 

#### The who part of an IAM policy can be a Google account, a Google group, a service account, or a Cloud Identity domain.
#### The can-do what part of an IAM policy is defined by a role. 
An IAM role is a collection of permissions. For example, to manage virtual machine instances in a project, you must be able to create, delete, start, stop, and change virtual machines, so these permissions are grouped into a role to make them easier to understand and easier to manage. 

When a user, group, or service account is given a role on a specific element of the resource hierarchy, the resulting policy applies to both the chosen element and all the elements below it in the hierarchy. 

There are three kinds of roles in IAM: 
 #### Basic
 #### Predefined
 #### Custom
 
 ### The first role type is Basic. 
 Basic roles are quite broad in scope. When applied to a Google Cloud project, they affect all resources in that project. Basic roles include: Owner, Editor, Viewer, and Billing Administrator.
Project viewers can access resources but can't make changes. 
Project editors can access and make changes to a resource. 
Project owners can also access and make changes to a resource. In addition, project owners can manage the associated roles and permissions and set up billing. 
Often, companies want someone to control the billing for a project, but not be able to change the resources in the project. This is possible through a billing administrator role. 

A word of caution; if several people are working together on a project that contains sensitive data, basic roles are probably too broad. Fortunately, IAM provides other ways to assign permissions that are more specifically tailored to meet the needs of typical job roles. This brings us to the second type of role

### predefined roles

Specific Google Cloud services offers sets of predefined roles and they even define where those roles can be applied. Let's look at Compute Engine, for example. A Google Cloud product that offers virtual machines as a service. With Compute Engine, you can apply specific Predefined roles such as Instance Admin to Compute Engine resources in a given project, a given folder, or an entire organization. This then allows whoever has these roles to perform a specific set of defined actions. 

But what if you need to assign a role that has even more specific permissions? That's when you'd use :

### Custom role
Many companies use a least privileged model in which each person in your organization is given the minimal amount of privilege needed to do their job. 
For example, maybe you want to define an Instance Operator role to allow some users to stop and start Compute Engine virtual machines but not reconfigure them. 
Custom roles will allow you to define these exact permissions. Before you start creating Custom roles, please note two important details. 
First, you'll need to manage the permissions that define the Custom role you've created, because of this, some organizations decide they'd rather use the Predefined roles. 
Second, Custom roles can only be applied to either the project level or organization level. They can't be applied to the folder level.


# Service accounts

What if you want to give permissions to a Compute Engine virtual machine, rather than to a person? 

#### Well, that’s what service accounts are for. 

Let’s say you have an application running in a virtual machine that needs to store data in Cloud Storage, but you don’t want anyone on the internet to have access to that data–just that particular virtual machine. You can create a service account to authenticate that VM to Cloud Storage. 
Service accounts are named with an email address, but instead of passwords they use cryptographic keys to access resources. 

So, if a service account has been granted Compute Engine’s Instance Admin role, this would allow an application running in a VM with that service account to create, modify, and delete other VMs. 
Service accounts do need to be managed. For example, maybe Alice needs to manage which Google accounts can act as service accounts, while Bob just needs to be able to view a list of service accounts. 

Fortunately, in addition to being an identity, a service account is also a resource, so it can have IAM policies of its own attached to it. This means that Alice can have the editor role on a service account, and Bob can have the viewer role. This is just like granting roles for any other Google Cloud resource.


# Cloud Identity

When new Google Cloud customers start using the platform, it's common to log into the Google Cloud Console with a Gmail account and then use Google Groups to collaborate with teammates who are in similar roles. 

Although this approach is easy to start with, it can present challenges later because the team's identities are not centrally managed. This can be problematic If for example, someone leaves the organization. With the setup, there's no easy way to immediately remove a user's access to the team's cloud resources.

With a tool called Cloud Identity, organizations can define policies and manage their users and groups using the Google Admin Console. Admins can log in and manage Google Cloud resources using the same user names and passwords they already used in existing Active Directory or LDAP systems.

Using Cloud Identity also means that when someone leaves an organization, an administrator can use the Google Admin Console to disable their account and remove them from groups.

Cloud Identity is available in a free edition and also in a premium edition that provides capabilities to manage mobile devices.

If you're a Google Cloud customer who is also a Google Workspace Customer, this functionality is already available to you in the Google Admin Console.


# Intracting with Google Cloud

There are four ways to access and interact with Google Cloud.  
1. The Cloud Console
2. The Cloud SDK in Cloud Shell
3. The APIs
4. The Cloud Console Mobile App

### First is the Google Cloud Console
It is Google Cloud's graphical user interface or GUI that helps you deploy, scale, and diagnose production issues in a simple web-based interface.
With the Cloud Console-
##### you can easily find your resources
##### check their health
##### have full management control over them
##### set budgets to control how much you spend on them
##### The Cloud Console also provides a search facility to quickly find resources and connect to instances via SSH in the browser. 

### Second is through the Cloud SDK in Cloud Shell. 
The Cloud SDK is a set of tools that you can use to manage resources and applications hosted on Google Cloud. These include the 

##### gcloud tool-
which provides the main command line interface for Google Cloud products and services, 

##### gsutil -
which lets you access Cloud storage from the command line and 

##### bq-
a command line tool for BigQuery. 

When installed, all of the tools within the Cloud SDK are located under the bin directory. Cloud Shell provides command line access to Cloud resources directly from a browser. 
Cloud Shell is a Debian-based virtual machine with a persistent five gigabyte home directory, which makes it easy to manage Google Cloud Projects and Resources. With Cloud Shell, the Cloud SDK, gcloud command, and other utilit ies are always installed, available up to date, and fully authenticated. 

### The third way to access Google Cloud is through application programming interfaces or APIs. 
The services that make up Google Cloud offer APIs so that code you write can control them. 
The Cloud Console includes a tool called the Google APIs Explorer that shows which APIs are available and in which versions. You can try these APIs interactively, even those that require user authentication. 

Suppose you've explored an API and you're ready to build an application that uses it, do you have to start coding from scratch? No. Google provides Cloud Client Libraries and Google API Client Libraries in many popular languages to take a lot of the drudgery out of the task of calling Google Cloud from your code. Languages currently represented in these libraries are Java, Python, PHP, C#, Go, Node.js, Ruby, and C++. 

### Finally, the fourth way to access and interact with Google Cloud is with the Cloud Console Mobile App.
which can be used to start, stop, and use SSH to connect to Compute Engine instances and see logs from each instance.It also lets you stop and start Cloud SQL instances. 
Additionally, you can administer applications deployed in App Engine by viewing errors, rolling back deployments, and changing traffic, splitting. 
The Cloud Console Mobile app provides up-to-date billing information for your projects in billing alerts for projects that are going over budget.
You can set up customizable graphs showing key metrics, such as CPU usage, network usage, requests per second, and server errors. 
The mobile app also offers alerts and incident management. 
You can download the Cloud Console Mobile app at cloud.google.com/console-app.


# VIRTUAL MACHINES AND NETWORKS IN CLOUD

# Virtual Private Cloud Networking

Let's explore how Google Compute Engine works with a focus on virtual networking. Many users start with Google Cloud by defining their own virtual private cloud inside their first Google Cloud project. Or by starting with the default Virtual Private Cloud. 

### what is a Virtual Private Cloud?
A Virtual Private Clouds or VPC is a secure individual private cloud computing model hosted within a public cloud, like Google Cloud. On a VPC, customers can run code, store data, host websites and do anything else they could do in an ordinary private cloud. But this private cloud is hosted remotely by a public cloud provider.

#### This means that VPC's combine the scalability and convenience of public cloud computing with the data isolation of private cloud computing.

VPC networks connect Google Cloud resources to each other and to the internet. This includes segmenting networks. Using firewall rules to restrict access to instances and creating static routes to forward traffic to specific destinations. Here's something that tends to surprise a lot of new Google Cloud users. 

### Google VPC networks are global. 
They can also have subnets, which is a segmented piece of the larger network in any Google loud region worldwide. Subnets can span the zones that make up a region. This architecture makes it easy to define network layouts with global scope. Resources can even be in different zones on the same subnets.

The size of a sub net can be increased by expanding the range of IP addresses allocated to it. And doing so won't affect virtual machines that are already configured.

For example, let's take a VPC with one network that currently has one sub net defined in google cloud's US east one region. If the VPC has two Compute Engine VMS attached to it. It means their neighbors on the same sub net, even though they're in different zones. This capability can be used to build solutions that are resilient to disruptions, yet retain a simple network layout.

# Compute Engine 

### Google Cloud's IaaS solution-Compute Engine
With Compute Engine, users can create and run virtual machines on Google infrastructure. There are no upfront investments and thousands of virtual CPUs can run on a system that's designed to be fast and to offer consistent performance. 

Each virtual machine contains the power and functionality of a full-fledged operating system. This means a virtual machine can be configured much like a physical server by specifying the amount of CPU power and memory needed, the amount and type of storage needed, and the operating system. 

A virtual machine instance can be created via the Google Cloud Console, which is a web-based tool to manage Google Cloud Projects and Resources, or via the gcloud command-line tool. The instance can run Linux and Windows Server images provided by Google or any customized versions of these images. You can also build and run images of other operating systems and flexibly reconfigure virtual machines. 

A quick way to get started with Google Cloud is through the Cloud Marketplace, which offers solutions from both Google and third-party vendors. With these solutions, there's no need to manually configure the software, virtual machine instances, storage or network settings, although many of them can be modified before lunch if that's required. Most software packages in Cloud Marketplace are available at no additional charge beyond the normal usage fees for Google Cloud resources. 

Some Cloud Marketplace images charge usage fees, particularly those published by third parties with commercially licensed software. But they all show estimates of their monthly challenges before they're launched. At this point, you might be wondering about Compute Engine's pricing and billing structure. 
For the use of virtual machines, Compute Engine bills by the second with a one-minute minimum and sustained use discount start to apply automatically to virtual machines the longer they run. For each VM that runs for more than 25 percent of a month, Compute Engine automatically applies a discount for every additional minute. 

### Compute Engine also offers committed use discounts. 
This means that for stable and predictable workloads, a specific amount of vCPUs and memory can be purchased for up to a 57 percent discount off of normal prices in return for committing to a usage term of one year or three years. 

#### Then there are preemptible VMs. 
Let's say, you have a workload that doesn't require a human to sit and wait for it to finish, such as a batch job analyzing a large dataset. You can save money, in some cases up to 90 percent by choosing preemptible VMs to run the job. 

A preemptible VM is different from an ordinary Compute Engine VM in only one respect. Compute Engine has permission to terminate a job if its resources are needed elsewhere. Although savings are possible with preemptible VMs, you need to ensure that your job can be stopped and restarted. In terms of storage, Compute Engine doesn't require a particular option or machine type to get high-throughput between processing and persistent disks. That's the default and it comes to you at no extra cost. 

Finally, you'll only pay for what you need with custom machine types. Compute Engine lets you choose the machine properties of your instances, like the number of virtual CPUs and the amounts of memory by using a set of predefined machine types, or by creating your own custom machine types.


# Scaling virtual machine

In Compute engine we can choose the most appropriate machine properties for your instances, like the number of virtual CPUs and the amount of memory, by using a set of predefined machine types, or by creating custom machine types. To do this, Compute Engine has a feature called Autoscaling.

### Autoscaling

where VMs can be added to or subtracted from an application based on load metrics. The other part of making that work is balancing the incoming traffic among the VMs. Google’s Virtual Private Cloud (VPC) supports several different kinds of load balancing.
With Compute Engine, you can in fact configure very large VMs, which are great for workloads such as in-memory databases and CPU-intensive analytics, but most Google Cloud customers start off with scaling out, not up. The maximum number of CPUs per VM is tied to its “machine family” and is also constrained by the quota available to the user, which is zone-dependent. 

Specifications for currently available VM machine types can be found at cloud.google.com/compute/docs/machine-types





