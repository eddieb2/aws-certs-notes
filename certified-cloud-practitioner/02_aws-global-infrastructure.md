# <b>AWS Global Infrastructure</b>

<br>

---

## <b><i>SECTION 1</i>: Map Overview</b>

---

<br>

## AWS Global Infrastructure

AWS has multiple data centers all over the world.

This is so you, the customer, can access their services no matter where you are located around the globe.

<b>Key points:</b>

AWS Serves over a million active customers in more than 190 countries

### Currently there are:

-   61 Availability Zones (AZs)
-   22 Geographic Regions
-   A vast network of Edge Locations
    Availability Zones: are distinct locations within an AWS Region that are engineered to be isolated from failures in other Availability Zones.

Geographic Regions: a physical location around the world where AWS clusters data centers.

Edge Locations: where end users access services located at AWS.

<blockquote>References https://infrastructure.aws/</blockquote>

<br>

---

## <b><i>SECTION 2</i>: Regions</b>

---

<br>

## Regions

    A geographically Distinct Location, which has multiple datacentres(AZs).

<b>Every region is physically isolated from and independent of every other region in terms of location, power, water supply</b>

-   Each region has at least two Availability Zones (AZs) ​
-   AWS US-EAST-1 (North Virginia) is the largest region​
-   New services almost always become available first in US-EAST​
-   Not all AWS Services are available in all regions​
-   All your billing information appears in US-EAST-1 (North - Virginia)​
-   AWS is always looking to expand their foot-print so new
    regions could be added in the upcoming years.​

<br>

<blockquote>You can head over to AWS's Global Infrastructure page to learn more about Regions and see maps of their locations.</blockquote>

<br>

In the AWS Console you can change AWS Regions. Whatever AWS resources you launch will be in that region.​
Some AWS Services such as CloudFront operate in multiple regions and you’ll see the region change to Global​

<br>

---

## <b><i>SECTION 3</i>: Availability Zones</b>

---

<br>

## Availability Zones

    **Availability Zones are often referred to as AZs.
    **An AZ is a data centre owned and operated by AWS in which their service is run.

The use of AZ’s give customers the ability to operate production applications and databases that are more:

-   highly available
-   fault tolerant
-   scalable

Key Points:

-   Data Centres always run more than one AZ.
-   This allows users to practice high availability. Customers who care about the availability and performance of their applications want to deploy these applications across multi AZ's in the same region.
-   There are specific AWS services that require the use of more than one AZ to function properly.
-   Multi AZ- refers to distributing your instances across multiple availability zones so that they fail over.
-   The latency between AZs in a Region is extremely low. On average it is below 10 milliseconds.

<br>

---

## <b><i>SECTION 4</i>: Edge Locations</b>

---

<br>

## <b>Edge Locations</b>

### <b>Key Points</b>:

-   Edge locations allow users to send data and receive data from AWS faster.
-   An Edge Location is a data centre owned by a trusted partner of AWS
-   They have a direct connection to the AWS network.
-   These data centers are not used for computing or storage.
-   It's a faster way to connect to AWS where AWS may not have a data centre yet.
-   Services that would utilize Edge Locations would be:
    -   Cloud-Front- a CDN
    -   Route53- for DNS
    -   A.P.I. Gateway- a way of connecting your Lambda functions with an end point
    -   S3 - where you want to get your files uploaded to S3 a lot faster.
-   Allows for low latency
    Edge Cases typically outnumber Availability Zones(AZ).

<blockquote>If you check out the Regions and AZs map again you can see the Edge Locations represented as blue dots.</blockquote>

<br>

---

## <b><i>SECTION 5</i>: GovCloud</b>

---

<br>

## GovCloud

<b>Key Points</b>:

-   AWS GovCloud Regions allow customers to host sensitive Controlled Unclassified Information and other types of regulated workloads.
-   GovCloud Regions are only operate by employees who are U.S. citizens on U.S. soil.
-   Only accessible to U.S. entities and account state holders who pass a screening process.
-   Customers can architect secure cloud solutions that comply with: - FedRAMP High baseline - DOJ's Criminal Justice Information Systems (CJIS) Security Policy - U.S. International Traffic in Arms Regulations (TAR) - Export Administration Regulations (EAR) - Department of Defense (DoD) Cloud Computing Security Requirements Guide
    GovCloud Regions are currently only in the US.

You can view their regions on AWS Map of Regions and Edge Networks.
You can view more about GovCloud on the official AWS GovCloud page.
