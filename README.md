# Multiple-Workloads-running-on-Multi-Cloud-Ecosystem-
In the landscape of cloud computing, there are multiple cloud service providers that offer ever growing services such as IaaS, PaaS and SaaS to the consumers. The ability to deploy and manage multi-cloud systems (i.e., applications on multiple clouds) allows the extraction of the idiosyncrasies of each cloud solution and hence optimising the cost, performance and availability of the applications and services. This paper gives an overview survey of multi-cloud which is a combination of multiple cloud computing services to form a single heterogeneous architecture by concurrently using separate cloud providers e.g. Amazon Web Services and Google Cloud Platform for Infrastructure (IaaS), Platform (PaaS) and/or Software (SaaS). In the scope of this project, we deploy a multi-cloud Ecosystem using two cloud providers so that we can use different services for different workloads. We deploy a Load balancer that balances the workloads across different cloud providers.

# We use the following steps in the proper order to make sure the services deployed are working correctly

●	Deploying virtual private cloud (VPC) networks 

●	Create (virtual machine) VM instances

●	Create apps instance on the VMs

●	Create VPN gateways

●	Create IPsec tunnels

●	Deploy Load Balancer


# We use the following best practices guidelines when deploying the multi-cloud solution.

●	Place both VPCs in an intended region or zone on both AWS and GCP

●	Build a custom VPC networks with a user-specified logically isolated network blocks in AWS and GCP

●	Deploy VM instances in each VPC networks

●	Create VPN gateways in both VPC network for two IPsec tunnels

●	For AWS define VPN gateways with two tunnels (active & standby) for redundancy & availability.

●	Configure Static routes pointing to tunnel interface for GCP CIDR

●	Configure Static routes pointing to tunnel interface for AWS CIDR

●	Test the connections on both the tunnels using ping and traceroute command.

●	Check the logs on GCP

●	Configure load balancer on AWS environment and run the specified tests

●	Build a web application to upload files on S3 with the help of Facebook App

●	AWS load balancer redirect the requests to either instances which are in virtual private cloud based on the round robin 
algorithm

●	Monitoring charts  are captured within cloud watch software

●	When running low capacity we can add one more server which will handle the new requests. Load balancer will be able to 
redirect towards that new instance.

●	If any of the server gets shut down then we can redirect the requests to the active servers

Benchmarks are set for these types of ecosystems using tools like Jmeter for testing the efficiency of load balancer), Gluster test for testing how consistent and synchronised files are distributed between two clouds. Ettercap test for pen testing cloud networks and verifying leakage of information to an unauthorized third party. “Ifconfig” command is used to check the virtual ip translation. VPN test is done by pinging the particular instance. Testing performance and availability can be done on the following parameters- stress, load, performance, compatibility and latency.
# We reached to the Conclusion that:

●	Multi-cloud architecture drives improved and new levels of flexibility, scalability and reliability, allowing  to focus on evolving trends in business.

●	Multi-cloud technologies are still new and quickly evolving, there is not much data available in terms of architectural deployment of various instance on multi-cloud

●	A lot of dependencies on the cloud provider in regards to what can be achieved and deployed on multi-cloud

●	multi -cloud is a cost effective solution and we can pay as we grow

●	We can divide our service requests between different servers in our Virtual Private Cloud using Load balancer

Please have a look at the screenshots file to verify in order to have a successfull Multi-Cloud Network
