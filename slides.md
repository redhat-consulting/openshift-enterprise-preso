## OpenShift
#### Platform as a Service by Red Hat
Created by Eric Sauer | Red Hat Consulting


### Bio

 - 5 years at Red Hat
 - Based in Raleigh
 - 3 years JBoss & Middleware Automation Consulting
 - 2 years OpenShift/Cloud Consulting & FDE work


### Agenda

 - Lab 1: OpenShift Application Deployment
 - OpenShift Technical Overview
 - Lifecycle of an Application
 - Lab 2: Development Cycle
 - OpenShift Projects
 - OpenShift in the Enterprise


### Agenda (if we have time)
 - Customer Stories
 - Roadmap & OpenShift v3
 - Questions/Discussions
 Note: Kick off provisioning



## Lab 1: OpenShift Application Deployment


### Instructions:
 1. Sign in to openshift.redhat.com
 2. Select '-> Create your first application now'
 3. Scroll down to 'Other Types' and select 'Node.js 0.10'
 1. Name your app 'myfirstapp', and use your username as the domain.
 1. In the 'Git URL' box, enter:
 ```
 https://github.com/redhat-consulting/openshift-enterprise-preso.git
 ```
 1. Select 'Create Application'


### Instructions cont'd:
 - Click through to show your application
 - Click on your application URL to view your newly created app



## OpenShift Technical Overview
 - OpenShift is a PaaS
 - Built on RHEL
 - Can run in any infrastructure
 - Can run any Middleware Technology
 - Made up of a Control Layer (Broker) and Container Layer (Nodes)

See [Intractive Diagram](https://www.openshift.com/walkthrough/how-it-works)


### What is PaaS?
  - Traditional/Legacy Infrastructure Model
  - PaaS Model


### What is PaaS?  
##### Traditional/Legacy Infrastructure Model

  - Developer has an idea
  - Decide on Infrastructure Needs
  - Request servers/VMs
  - Wait...
  - Request Network Connectivity
  - Wait....
  - Install/Configure OS, Middleware, etc.
  - Write code
  - Deploy code
  - Test
  - Request code promotion
  - Wait...
  - etc.


### What is PaaS?  
##### PaaS Infrastructure Model

  - Developer has an idea...
  - Creates an application environment and instantly begins writing and deploying code
  - Automated testing
  - Automated code promotion


### Built on RHEL

 - Uses lots of Core RHEL
  - SELinux, Cgroups, SSH
  - Apache httpd, haproxy
 - Soon to come:
  - Docker, Kubernetes


### Can Run on Any Infrastructure

 - Bare Metal
 - VMWare
 - RHEV
 - OpenStack
 - EC2


### Can Run 'Any' Middleware Technology

 - [Supported Technologies](https://www.openshift.com/products/technologies)


### Control and Management Layer

 - Broker/Master
 - Responsible for:
  - DNS
  - Authentication/Authorization
  - Application State


### Container Layer

 - Nodes
 - Responsible for:
  - Hosting Application Containers



## Lifecycle of an Application

 - Create an App
 - Select Technologies
 - Deploy Code
 - Automated Build/Test/Publish
 - Scale

See [Interactive Diagram](https://www.openshift.com/walkthrough/developer-workflow)



## Lab 2: Development Cycle


### Prerequisite

Install RHC Tools: [Instructions here](https://access.redhat.com/documentation/en-US/OpenShift_Online/2.0/html/Client_Tools_Installation_Guide/index.html)

Windows Users: Make sure you install the Git Bash tooling


### Instructions:
 1. Set up RHC Tools
 ```bash
 rhc setup
 ```
 2. View Your Applications
 ```bash
 rhc domain-show
 ```
 3. Clone Your Application Code
 ```bash
 rhc git-clone
 ```


### Instructions cont'd
 4. Check that your code downloaded
 ```bash
 cd ./myfirstapp
 ls
 git status
 ```
 5. Make code changes (try index.html or slides.md)
 6. Push Code
 ```bash
 git commit -a -m"Felt like coding today"
 git push
 ```


### Instructions cont'd
Done!

Refresh Your Application


### A Little Tangent about Git

 - Common confusion among customers
 - Application containers are "stateless"
 - Git in An App Container is for Transport Only
 - Not meant to be hosted version control



## OpenShift Projects
 - OpenShift Origin
 - OpenShift Online
 - OpenShift Enterprise


### OpenShift Origin

 - Community Project
 - Constant code drops
 - Fork it on [Github](https://github.com/openshift/origin-server)!
 - See [OpenShift.org](http://openshift.org) for more details


### OpenShift Online

 - Public Offering of OpenShift
 - Origin + Custom Code
 - Run by a Red Hat Operations Team in conjunction with Engineering


### OpenShift Enterprise

 - Our On-Premise PaaS
 - "Private Cloud"
 - 3 week release cycle (will slow down)



## OpenShift in the Enterprise

 - Application Workflows
 - Release and Deployment
 - HA
 - Common Challenges
 - How to Position Customers for Cloud


### Application CI Workflow

 - Whiteboard Diagram


### Release and Deployment

 - [Diagram](https://docs.google.com/drawings/d/1Lpdija2oCXBsXl4ziY0GXzmIZ1-Ej23gOYxcjNXg65Q/edit?usp=sharing)


### HA

 - HA is Accomplished with An External Routing Layer
  - F5
  - Nginx
 - [Diagram](https://docs.google.com/drawings/d/13X-kMFUI6hR0UH7qDY2ottgipM1KUbtNce-2RI9gcX0/edit?usp=sharing)


### Common Challenges

 - Integration
 - Culture
 - Education


### How to Position Customers for Cloud

 - Sell the stateless application story
 - Encourage Automation
 - Discourage 'special snowflake' applications
 - Adopt agile methodologies in Project Teams



## End
#### Questions? Comments?
