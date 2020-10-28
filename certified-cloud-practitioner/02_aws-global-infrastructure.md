# **_AWS Global Infrastructure_**

<br>

---

## **_SECTION 1: Overview_**

---

<br>

## AWS Global Infrastructure

The AWS Global Infrastructure is globally distributed hardware and datacenters that are physically networked together to act as one large resource for the end customer.

This is so you, the customer, can access their services no matter where you are located around the globe.

**_The AWS Global Infrastructure is made up of the following resources:_**

### Currently there are:

-   24 Launched Regions
-   77 Availability Zones
-   97 Direct Connection Locations
-   216 Points of Presence
-   1 Local Zone

**_Availability Zones:_** are distinct locations within an AWS Region that are engineered to be isolated from failures in other Availability Zones.

> References https://infrastructure.aws/

<br>

---

## **_SECTION 2: Regions_**

---

<br>

## Regions

    A geographically Distinct Location, which has multiple datacentres(AZs).

**_Every region is physically isolated from and independent of every other region in terms of location, power, water supply_**

-   Each region has at least two Availability Zones (AZs) ​
-   AWS US-EAST-1 (North Virginia) is the largest region​
-   New services almost always become available first in US-EAST​
-   Not all AWS Services are available in all regions​
-   All your billing information appears in US-EAST-1 (North - Virginia)​
-   AWS is always looking to expand their foot-print so new
    regions could be added in the upcoming years.​

<br>

> You can head over to AWS's Global Infrastructure page to learn more about Regions and see maps of their locations.

<br>

In the AWS Console you can change AWS Regions. Whatever AWS resources you launch will be in that region.​
Some AWS Services such as CloudFront operate in multiple regions and you’ll see the region change to Global​

<br>

---

## **_SECTION 3: Availability Zones_**

---

<br>

## Availability Zones

    Availability Zones are often referred to as AZs. An Availability Zone (AZ) is a physical location made up of one or more datacenters.​ A datacenter is a secured building that contains​ hundreds or thousands of computers. Datacenters within a region will be isolate from​ each other (different buildings). But they will​ be close enough to provide low-latency (< 10ms).​

A region will generally contain 3 Availability Zones​.

The use of AZ’s give customers the ability to operate production applications and databases that are more:

-   Highly available
-   Fault tolerant
-   Scalable

Key Points:

Its common practice to run workloads in at least​ 3 AZs to ensure services remain available in case ​one or two datacenters fail (High Availability).

-   A subnet is associated with an Availability Zone.​ So to launch an AWS resource into a specific AZ you need to launch your resource in a subnet that resides in that AZ.

<br>

---

## **_SECTION 4: Edge Locations_**

---

<br>

## **_Points of Presence_**

    Intermediate locations between an AWS Region and the end user, and this location could be a datacenter or collection of hardware.​

-   For AWS a Point of Presence is a data center owned by AWS or is a trusted partner that is utilized by AWS Services related for content delivery or expediated upload.​

<u>**_Edge Locations_**</u> - are datacenters that hold cached (copy) on the most popular files (eg. web pages,images and videos) so that the delivery of distance to the end users are reduce

<u>**_Regional Edge Locations_**</u> - are datacenters that hold much larger caches of less-popular files to reduce a full round trip and also to reduce the cost of transfer fees.​

**_The following AWS Services use PoPs for content delivery or expediated upload:_**

<u>**_AWS CloudFront_**</u> - is a Content Delivery Network (CDN) service that:​

-   You point your website to CloudFront so that it will route requests to nearest Edge Location cache​

-   Allows you to choose an origin (such as a web-server or storage) that will be source of cached​

-   Caches the contents of what origin would returned to various Edge Locations around the world​

<u>**_AWS S3 Transfer Acceleration_**</u> - allows you to generate a special URL that can be used by end users to upload files to a nearby Edge Location. Once a file is uploaded to an Edge Location, it can move much faster within the AWS Network to reach S3.​

<u>**_AWS Global Accelerator_**</u> - can find the optimal path from the end user to your web-servers. Global Accelerators are deployed within Edge Locations so you send user traffic to an Edge Location instead of directly to your web-application.​

<br>

---

## **_SECTION 5: GovCloud_**

---

<br>

## GovCloud

**_Key Points_**:

-   AWS GovCloud Regions allow customers to host sensitive Controlled Unclassified Information and other types of regulated workloads.
-   GovCloud Regions are only operate by employees who are U.S. citizens on U.S. soil.
-   Only accessible to U.S. entities and account state holders who pass a screening process.
-   Customers can architect secure cloud solutions that comply with: - FedRAMP High baseline - DOJ's Criminal Justice Information Systems (CJIS) Security Policy - U.S. International Traffic in Arms Regulations (TAR) - Export Administration Regulations (EAR) - Department of Defense (DoD) Cloud Computing Security Requirements Guide
    GovCloud Regions are currently only in the US.

You can view their regions on AWS Map of Regions and Edge Networks.
You can view more about GovCloud on the official AWS GovCloud page.

<br>

---

## **_SECTION 6: DirectConnect Locations_**

---

<br>

Direct Connect Locations - are trusted third-party datacenters that you can establish a dedicated high speed, low-latency connection from your on-premise to the AWS network.​

DirectConnect connections are always established through a third-party provider. These APN (Amazon Partner Network) Partners can help you establish network circuits between an AWS Direct Connect location and your datacenter, office, or colocation environment, or assist you in constructing a hybrid environment.

<br>

---

## **_SECTION 7: Local Zones_**

---

<br>
