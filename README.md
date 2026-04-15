# AWS_SAA-C03

## Course Fundamentals and AWS Accounts
### The basics
1) AWS Accounts 
2) Single Factor or Multi Factor Authentication 
3) IAM and IAM Access Keys 

### Cloud, Networking and Technical Fundamentals 
OSI (Open Systems Interconnection) Model Introduction and 7 Layers
<img width="748" height="421" alt="image" src="https://github.com/user-attachments/assets/c6d114c5-689d-40a2-b997-cf9fc4da3c6b" />

1) Layer 1 - Physical - handles the physical (wavelengths or voltages) transmission and the reception onto and from the physical medium. It uses binary numbers that can be recognized by network interface cards and transmitted through a physical medium like network cable.
2) Layer 2 - Data Link - provides frames. Sending information over layer 2 network. It uses layer 1 to transmit and receive raw data, but it's adding on top of this the MAC addresses which allow for machine-to-machine communication. In addition, it is adding media access control.
   If we are only using layer 1, it will not work as there will always be collision. But layer 2, checks for the carrier first before it instructs layer 1 to transmit.
   This is encapsulation - the taking of some data, and wrapping it in something else (inside a frame for layer 2). 

   Mac address - hardcoded into a device’s network interface card (NIC) by its manufacturer. not software assigned. 
   










## AWS Fundamentals 
### Public Internet Zone, AWS Private Services and AWS Public Zone 
1) Public Internet Zone - this is the public internet, or the environment outside AWS. 
2) AWS Private Zone - this is private / internal-use only zone. it is isolated and can be configured if needed. 
3) AWS Public Zone - refers to AWS resources that are accessible from the internet.


## AWS Global Infrastructure


### AWS Region 
### AWS Edge Locations 

For example, 
Netflix might run its infrastructure in multiple regions worldwide, but store their data in lots of edge locations allowing it to be delivered at faster speeds and lower latency.

### Some AWS services are either regional or global. 
For example, EC2 is regional service. IAM or Route 53 is global service (no option to select a region in the management console). 

### Region 3 benefits: 
1) Geographic separation - isolated fault domain
2) Geopolitical Separation - different governance
3) Location Control - Performance

### Regions and Availability Zones (AZ)
Inside regions, there could be multiple Availability Zones. 
You can design solutions which distribute components across multiple availability zones. 
If you have 6 availability zones in Sydney, and 2 AZ is impacted/fails then 4 out of 6 servers remain operational. It is a way of building resilience. 

### How to define Service Resilience 
1) Global resilient service - Works across multiple regions worldwide even if 1 region fails because it is not dependent on a single region (e.g. IAM and Route 53). Designed to survive regional failures. 

2) Region resilient service - Works across multiple Availability Zones (AZs) within one region. If 1 AZ fails, then other AZs in that region can continue. But if the whole region fails, then the service will fail. Designed to survive AZ failures. (e.g. S3, RDS, Load Balancers)

3) AZ resilient service - Runs in one Availability Zone. Only protected within one AZ (least resilient). High chance of failure (e.g. Single EC2 instance, basic setups)

### VPC (Virtual Private Cloud) 
- Virtual Network inside AWS (a private network inside Amazon Web Services where you launch and manage your resources securely.)
- A VPC is within



 
