# Table of contents
- [Introduction-Google Cloud Fundamentals](#Introduction-Google-Cloud-Fundamentals)
- [Cloud Computing Overview](#Cloud-Computing-Overview)
- [IaaS & PaaS](#IaaS-&-PaaS)
- [The Google Cloud Locations](#Google-Cloud-Locations)
- [Environmental Impact](Environmental-Impact)

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









