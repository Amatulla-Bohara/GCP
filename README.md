# Table of contents
- [Introduction-Google Cloud Fundamentals](#Introduction-Google-Cloud-Fundamentals)
- [Cloud Computing Overview](#Cloud-Computing-Overview)
- [IaaS & PaaS](#IaaS-&-PaaS)
- [The Google Cloud Locations](#Google-Cloud-Locations)
- [Environmental Impact](Environmental-Impact)
- [Security](#Security)

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
